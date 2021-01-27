# Persistence
- INI files
- XML 
- Cookies are small but can still slow processing
- userData 64k
- Local Shared Objects (Flash)

## HTML5 Storage
- supported by all major browsers
- to check:
```javascript
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

- based on key value pairs
- treatted as assoc. array

```javascript
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```
- or just use bracket notation

```javascript
var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;

```

- to iterate through all keys

```javascript
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```
>If you call key() with an index that is not between 0–(length-1), the function will return null.

```javascript
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```

>Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports.

```javascript
function handle_storage(e) {
  if (!e) { e = window.event; }
}
```

- storage event object
```javascript
function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}
```