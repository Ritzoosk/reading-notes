# Reading 04
## HTML BOOK
### Chapter 4: Ch.4 “Links” (pp.74-93)
- 
```html
<a href="http://www.imdb.com">IMDB</a>
```
- href is the url IMDB is the text the user will click
- anchor tags alow you to link out to other sites
- linking back you your pages you can use the shorter relative URL
- parents, grandparents etc pg82 pdf89
- email links
>```html
 <a href="mailto:jon@example.org">Email Jon</a> 
 ```
- open in a new window target _blank

```html 
<a href="http://www.imdb.com" target="_blank">
Internet Movie Database</a> (opens in new window) 
```
- Example:
```html 
<html>
<head>
 <title>Links</title>
</head>
<body>
 <h1 id="top">Film Folk</h1>
 <h2>Festival Diary</h2>
 <p>Here are some of the film festivals we
 will be attending this year.<br />Please
 <a href="mailto:filmfolk@example.org">
 contact us</a> if you would like more
 information.</p>
 <h3>January</h3>
 <p><a href="http://www.sundance.org">
 Sundance Film Festival</a><br />
 Park City, Utah, USA<br />
 20 - 30 January 2011</p>
 <h3>February</h3>
 <p><a href="http://www.tropfest.com">
 Tropfest</a><br />
 Sydney, Australia<br />
 20 February 2011</p>
 <!-- additional content -->
 <p><a href="about.html">About Film Folk</a></p>
 <p><a href="#top">Top of page</a></p>
</body>
</html>
```

### Chapter 15: “Layout” (pp.358-404)
- block level vs. inline
- parents contain child elements
- z-index controls whats on top
- float allows other elements to "flow" around it in a determined direction

```css
body {
width: 750px;
font-family: Arial, Verdana, sans-serif;
color: #665544;}
h1 {
background-color: #efefef;
padding: 10px;}
p {
width: 450px;}
 ```
```html
<body>
<h1>The Evolution of the Bicycle</h1>
<p>In 1817 Baron von Drais invented a walking
 machine that would help him get around the
 royal gardens faster...</p>
</body>
 ```
 - position:absolute
> When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page. (They act like it is not
there.) 

- Fixed
>It positions the element in
relation to the browser window.
Therefore, when a user scrolls
down the page, it stays in the
exact same place. It is a good
idea to try this example in your
browser to see the effect.

- Columns without floats
>Many web pages use multiple
columns in their design. This
is achieved by using a <div>
element to represent each
column. The following three CSS
properties are used to position
the columns next to each other: 

```html
<h1>The Evolution of the Bicycle</h1>
<div class="column1of2">
<h3>The First Bicycle</h3>
<p>In 1817 Baron von Drais invented a walking
 machine that would help him get around the
 royal gardens faster: two same-size ...</p>
</div>
<div class="column2of2">
<h3>Bicycle Timeline</h3> ...
</div>
 ```
```css
.column1of2 {
float: left;
width: 620px;
margin: 10px;}
.column2of2 {
float: left;
width: 300px;
margin: 10px;}
```

## JS BOOK
### Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)
- functions is a group of steps
- its reuseable
- you can pass info into it and return info out of it
```javascript
function getSize (width, height, depth) {
var area = width * height;
}
var volume = width * height * depth;
var sizes= [area , volume];
return sizes;
var areaOne = getSize (3, 2, 3)[0];
var volumeOne = getSize (3, 2, 3)[1]; 
```
### 6 Reasons for Pair Programming
- Less mistakes! more eyes!
- stay engaged!
- seeing others work flow and methods
- better coding vocab = better interview vocab
- common practice in industry
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