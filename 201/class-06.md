# Reading 06
## js book 
## Chapter 3: “Object Literals” (pp.100-105)
- In object a variables become properties
- In object func= method
>Like variables and named functions,
properties and methods have a
name and a value. In an object,
that name is called a key
- Create an object "var hotel = {}"
- accessing an objecet "var name = hotel.name;"
>
```javascript
var hote l = {
name: 'Quay',
rooms: 40,
booked : 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var el Name = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms.textContent = hotel .checkAvailability(); 
```


## Chapter 5: “Document Object Model” (pp.183-242)
- DOM is made of object
> You will hear people call the DOM an
Application Programming Interface (API).
User interfaces let humans interact with
programs; APls let programs (and scripts)
talk to each other. The DOM states what
your script can "ask the browser about the
current page, and how to tell the browser
to update what is being shown to the user. 
- DOM tree -  a series of branches and nodes all containing
- Each node contains properties and methods
- Nodes types:
> ATTRIBUTE NODES:
The opening tags of HTML elements can carry
attributes and these are represented by attribute
nodes in the DOM tree.
Attribute nodes are not children of the element thar
carries them; they are part of that element. Once
you access an element, there are specific JavaScript
methods and properties to read or change that
element's attributes. For example, it is common to
change the values of cl ass attributes to trigger new
CSS rules that affect their presentation. 

> Text node: Once you have accessed an element node, you
can then reach the text within that element. This is
stored in its own text node.
Text nodes cannot have children. If an element
contains text and another child element, the child
element is not a child of the text node but rather
a child of the containing element. (See the <em>
element on the first <l i > item.) This illustrates how
the text node is always a new branch of the DOM
tree, and no further branches come off of it. 

- COMMANDS: (access)
>get ElementByld()
Uses the value of an element's
id attribute (which should be
unique within the page).
See p195 
>querySelector()
Uses a CSS selector, and returns
the first matching element.
See p202 
>getElementsByTagName()
Selects all elements that have the
specified tag name ..
See p201 
- once accessed you can do things with that node

- Queries can return one node or a whole list
> II Select the element and store it in a variable.
var el = document.getElementByid('one');
- item() methodreturns an individual node
> 
```javascript
var elements = document.getElementsByClassName('hot')
if (elements.length>= 1) {
var firstltem = elements.item(O);
} 
```
- you can access individual nodes with brackets, similar to array
- you can select nodes by several methods
- By element
- Tag Name
- Using CSS selector
- 
- looping through a node list:
> var hotltems = document .querySelectorAl l (' li . hot') ;