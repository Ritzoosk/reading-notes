# HTML

## Chapter 7: “Forms” (p.144-175)
- 
```html
<form action="http://www.example.com/subscribe.php"
method="get">
<p>This is where the form controls will appear.
 </p>
</form>
```
- Input
>The <input> element is used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating.

- max length, name , size pg 152
- password pg 153

- text area
><form action="http://www.example.com/comments.php">
<p>What did you think of this gig?</p>
 <textarea name="comments" cols="20" rows="4">Enter
 your comments...</textarea>
</form>

- radio button circle dot pg 155
- check box
- drop down
- multi selection
- input type file pg159
- hidden input
>This example also shows a
hidden form control. These form
controls are not shown on the
page (although you can see them
if you use the View Source option
in the browser). They allow web
page authors to add values to
forms that users cannot see.
For example, a web page author
might use a hidden field to
indicate which page the user was
on when they submitted a form


## Chapter 14: “Lists, Tables & Forms” (pp.330-357)
- bullet point styles
- img for bullets
- positioning the marker
- list shorthand
- table properties
>width to set the width of the
table
padding to set the space
between the border of each table
cell and its content
text-transform to convert the
content of the table headers to
uppercase
letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers
text-align to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows
:hover to highlight a table row
when a user's mouse goes over it

```css
body {
font-family: Arial, Verdana, sans-serif;
color: #111111;}
table {
width: 600px;}
th, td {
padding: 7px 10px 10px 10px;}
th {
text-transform: uppercase;
letter-spacing: 0.1em;
font-size: 90%;
border-bottom: 2px solid #111111;
border-top: 1px solid #999;
text-align: left;}
tr.even {
background-color: #efefef;}
tr:hover {
background-color: #c3e6e5;}
.money {
text-align: right;}
```
- borders on empty cells pg 339
- styling buttons

# JS

## Chapter 6: “Events” (pp.243-292)
- binding event to an element pg251 html event
  - pg252 tradtional event handlers
  - DOM lvl 2 listeners p254

   ![Event Image](201/img/evnt 2.PNG )

   ```javascript
   var star = '*';
    for (i = 0; i<= 4;i++){
      var printString = '';
      for (j = 0; j<= i;j++){
        printString += star;

      }
    console.log(printString);
    }
   ```