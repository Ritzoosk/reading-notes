
# Reading 05
## html book 
## Chapter 5: “Images” (pp.94-125)
- store images on site
> ```html
<img src="images/quokka.jpg" alt="A family of
 quokka" title="The quokka is an Australian
 marsupial that is similar in size to the
 domestic cat." />
 ```

- Block elements always appear
on a new line.
- Inline elements sit within a
block level element and do not
start on a new line. 
- 
>REDUCING IMAGE SIZE
You can reduce the size of
images to create a smaller
version of the image. decreasing load times
- 300 pdi is standard print image quality
- computer display is limited to 72 ppi
- vector images scale well since they are geometrically generated.


## Chapter 11: “Color” (pp.246-263)
- 
# Colors ch11 pg 247 pdf 245
- specify via RBG
  - rgb(100,100,90)
- Hex
  - For example: #ee3e80
- Color names
  - DarkCyan

### background color
> body {
background-color: rgb(200,200,200);}
h1 {
background-color: DarkCyan;}
h2 {
background-color: #ee3e80;}
p {
background-color: white;}

- RGB (102,205,170) (red,grn,blu) (###,###,###)
- HEX  #66cdaa 66=102red, cd=105grn, aa=170blu 

### Opacity
- The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).
> p.one {
background-color: rgb(0,0,0);
opacity: 0.5;}
p.two {
background-color: rgb(0,0,0);
background-color: rgba(0,0,0,0.5);}

- RGBA
- HSL color, Hue, Saturation, Lightsness
- CSS3: HSL & HSLA

- 

## Chapter 12: “Text” (pp.264-299)

- Font family
```css
body {
 font-family: Georgia, Times, serif;}
 h1, h2 {
 font-family: Arial, Verdana, sans-serif;}
 .credits {
 font-family: "Courier New", Courier,
 monospace;}
```
- Size
>pixels
Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.
>percentages
The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.
If you create a rule to make all
text inside the <body> element
to be 75% of the default size (to
make it 12px), and then specify
another rule that indicates the
content of an element inside the
<body> element should be 75%
size, it will be 9px (75% of the
12px font size).

>ems
An em is equivalent to the width
of a letter m.


```javascript
function sumThisUp() {
var arrayOfNumbers = [1,10,15,20]
var intNum = 5
for (var i = 0; i < arrayOfNumbers.length ; i++){
intNum + arrayOfNumbers[i]

}
}
```
```javascript
 for ( var iA=0 ; iA < arrayOfAns.length ; iA++){
    if (userGuess7 === arrayOfAns[iA]){
      alert('Nice! That is one of them!')
      i=0;
      frendLvl++;
      break;
    }else(i == 0)
    // console.log('last try')
      break;
```