# Reading 03
## HTML BOOK
### Chapter 3: “Lists” (pp.62-73)
- all list items
- <ol> ordered list (numbered)
- <li> list item
- <ul> unordered list (bullets or symbols)
- <dl> Definition Lists
- <dt>  (the definition term)
- <dd> The definition
- nesting lists pg 68

### Chapter 13: “Boxes” (pp.300-329)
- Box dim
```css div.box {
height: 300px;
width: 300px;
background-color: #bbbbaa;}
p {
height: 75%;
width: 75%;
background-color: #0088dd;}
```
-  min max width

```css td.description {
min-width: 450px;
max-width: 650px;
text-align: left;
padding: 5px;
margin: 0px;}
```
- min max height
```css h2, p {
width: 400px;
font-size: 90%;
line-height: 1.2em;}
h2 {
color: #0088dd;
border-bottom: 1px solid #0088dd;}
p {
min-height: 10px;
max-height: 30px;}
```
- overflow, hide or scroll
```css p.one {
overflow: hidden;}
p.two {
overflow: scroll;}
```
- border the perimeter line

- margin how close it gets to other elements
```css p {
width: 200px;
border: 2px solid #0088dd;
padding: 10px;}
p.example {
margin: 20px;}
```
- padding how close the content are to the border
```css p {
width: 275px;
border: 2px solid #0088dd;}
p.example {
padding: 10px;}
```
- border-width
```css p.one {
border-width: 2px;}
p.two {
border-width: thick;}
p.three {
border-width: 1px 4px 12px 4px;}
```
- color
```css p.one {
border-color: #0088dd;}
p.two {
border-color: #bbbbaa #111111 #ee3e80 #0088dd;}
```
- centering content
```css body {
text-align: center;}
p {
width: 300px;
padding: 50px;
border: 20px solid #0088dd;}
p.example {
margin: 10px auto 10px auto;
text-align: left;}
```

> inline
This causes a block-level
element to act like an inline
element.
block
This causes an inline element to
act like a block-level element.
inline-block
This causes a block-level
element to flow like an inline
element, while retaining other
features of a block-level element.
none
This hides an element from the
page. In this case, the element
acts as though it is not on the
page at all (although a user could
still see the content of the box if
they used the view source option
in their browser).

- hiding boxes
```css li {
display: inline;
margin-right: 10px;}
li.coming-soon {
visibility: hidden;}
```

## JS BOOK
### Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)
- ARRAYS!
```javascript var colors;
colors ['white', 'black', ' custom'];
var el document.getElementByld('col ors');
el . textContent = col ors[O]; 
```
- array constructor
```java var colors
new Array('white ' ,
'black',
'custom');
var el = document.getElementByid( ' colors' );
el.innerHTML = colors.item(O); 
```
- getting and changing values
```java II Create the array
var colors = ['white',
'black' ,
'custom'];
II Update the third item in the array
colors[2] = 'beige ' ;
II Get the element with an id of col ors
var el = document .getElementByid(' colors') ;
II Replace with third item from the array
el .textContent = colors[2];
```
### Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)
- cases
```java switch (level) {
case 'One ':
title= 'Level 1 ' ;
break;
case 'Two':
tit 1 e = ' Level 2 ' ;
break;
case ' Three' :
title = 'Level 3' ;
break ;
default :
title= 'Test';
break; 
}
```
- switch
```java var msg;
var level = 2;
II Message
11 Level
/I Determine message based on level
switch (level) {
case 1:
msg = 'Good luck on the first test ' ;
break;
case 2:
msg = 'Second of three - keep going!';
break;
case 3:
msg = ' Final round, al most there!';
break;
default :
msg = 'Good l uck!';
break;
var el = document.getEl ementByld('answer');
el .textContent = msg; 
```
- Falsy values 
 * false
 * 0
 * ''  NaN
 * empty value
 * var with no value assigned

 - Truthy
  * true
  * 1
  * 'carrot' string with content
  * Num calculations
  * '0' as a string
  * 'false' as a string

- 
