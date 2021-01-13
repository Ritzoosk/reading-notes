# Reading Notes 2
# HTML
## Chapter 2: “Text” (pp.40-61)
><h1>This is a Main Heading</h1>
<h2>This is a Level 2 Heading</h2>
<h3>This is a Level 3 Heading</h3>
<h4>This is a Level 4 Heading</h4>
<h5>This is a Level 5 Heading</h5>
<h6>This is a Level 6 Heading</h6>

- Paragraphs
><html>
HTML chapter-02/paragraphs.html <p>
To create a paragraph, surround
the words that make up the
paragraph with an opening <p>
tag and closing </p> tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.
Paragraphs
<p>A paragraph consists of one or more sentences
 that form a self-contained unit of discourse. The
 start of a paragraph is indicated by a new
 line.</p>
<p>Text is easier to understand when it is split up
 into units of text. For example, a book may have
 chapters. Chapters can have subheadings. Under
 each heading there will be one or more
 paragraphs.</p>

- p tags start the next item on a new line
- bold 
> <b>

## Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)
- CSS adds styling to the HTML framework or mark up
> p {font-family: Arial;} (targets p tag)
- target... then... {} (cury brackets)
### "index.html"
> <!DOCTYPE html>
<html>
<head>
 <title>Using External CSS</title>
 <link href="css/styles.css" type="text/css"
 rel="stylesheet" />
</head>
<body>
 <h1>Potatoes</h1>
 <p>There are dozens of different potato
 varieties. They are usually described as
 early, second early and maincrop.</p>
</body>
</html>

### CSS
>body {
 font-family: arial;
 background-color: rgb(185,179,175);}
h1 {
 color: rgb(255,255,255);}

> If you specify the font-family
or color properties on the
<body> element, they will apply
to most child elements. This is
because the value of the
font-family property is
inherited by child elements. It
saves you from having to apply
these properties to as many
elements (and results in simpler
style sheets).

# JS BOOK
## Chapter 2: “Basic JavaScript Instructions” (pp.53-84)
- Script
> var today= new Date{);
var hourNow = today.getHours{) ;
var greeting;
if (hourNow > 18) {
greeting= 'Good evening';
else if (hourNow > 12) {
greeting= 'Good afternoon';
else if (hourNow > O) {
greeting 'Good morning';
else {
greeting 'Welcome';
document.write(greeting) ; 

- /* multi line comment*/
- // normal comment
- setting variables var 'var name'
- = is assignment operator
- Data types Num, Strings, booleans
- storing vars
> var price;
var quantity;
var total;
price = 5;
quantity = 14;
total = price * quantity;
c02/j s/numeri c-vari ab 1 e .j s
var el = document.getElementByid( ' cost ');
el .textContent = '$' +total; 

- strings can use single or dbl quotes

## Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)
- decisions
> if ("condition"){do this
  }else{do this}
- ==  compare
- != not equal
- comparing expressions
> var scorel = 90;
var score2 = 95;
var highScorel = 75;
var highScore2 = 95;
II Round 1 score
II Round 2 score
II Round 1 high score
II Round 2 high score
II Check if scores are higher than current high scores
var comparison= (score!+ score2) > (highScorel + highScore2);
II Write the message into the page
var el = document.getElementByid( 'answer');
el .textContent ='New high score:'+ comparison;

- &&  both evaluate. only tru and tru = true all else false
- ||  or if one is true statment is true
>var scorel = 8; II Round 1 score
var score2 = 8; II Round 2 score
var passl 6; II Round 1 pass mark
var pass2 = 6; II Round 2 pass mark
II Check whether user passed both rounds , store result in variable
var passBoth = (scorel >= passl) && (score2 >= pass2);
II Create message
var msg = 'Both rounds passed: ' + passBoth;
II Write the message i nto the page
var el = document.getElementBy!d( 'answer') ;
el.textContent = msg; 

- 