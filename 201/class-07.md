# Reading Class 07
## Dom article
- PROPERTIES: KEY VALUE
 - check in inspector to see value stored correctly
 - generating random numbers
 - calculation from tables
 >The dailyLikes() method on EpicFailVideo's prototype is assigned a function with no parameters. This method starts by defining two variables called viewers and percentage.

- 
# HTML
## Chapter 6: “Tables” (pp.126-145)
- tables stoe data organized
```html
<table>
 <tr>
 <td>15</td>
 <td>15</td>
 <td>30</td>
 </tr>
 <tr>
 <td>45</td>
 <td>60</td>
 <td>45</td>
 </tr>
 <tr>
 <td>60</td>
 <td>90</td>
 <td>90</td>
 </tr>
</table>
```
- tr = table row
- td = table data
- th = heading
- spaning 
```html
<table>
 <tr>
 <th></th>
 <th>9am</th>
 <th>10am</th>
 <th>11am</th>
 <th>12am</th>
 </tr>
 <tr>
 <th>Monday</th>
 <td colspan="2">Geography</td>
 <td>Math</td>
 <td>Art</td>
 </tr>
 <tr>
 <th>Tuesday</th>
 <td colspan="3">Gym</td>
 <td>Home Ec</td>
 </tr>
</table>
```

- span rows
```html
<table>
 <tr>
 <th></th>
 <th>ABC</th>
 <th>BBC</th>
 <th>CNN</th>
 </tr>
 <tr>
 <th>6pm - 7pm</th>
 <td rowspan="2">Movie</td>
 <td>Comedy</td>
 <td>News</td>
 </tr>
 <tr>
 <th>7pm - 8pm</th>
 <td>Sport</td>
 <td>Current Affairs</td>
 </tr>
</table>
```
- long tables 
```html
<table>
 <thead>
 <tr>
 <th>Date</th>
 <th>Income</th>
 <th>Expenditure</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <th>1st January</th>
 <td>250</td>
 <td>36</td>
 </tr>
 <tr>
 <th>2nd January</th>
 <td>285</td>
 <td>48</td>
 </tr>
 <!-- additional rows as above -->
 <tr>
 <th>31st January</th>
 <td>129</td>
 <td>64</td>
 </tr>
 </tbody>
 <tfoot>
 <tr>
 <td></td>
 <td>7824</td>
 <td>1241</td>
 </tr>
 </tfoot>
</table>
```

# JS
## Chapter 3: “Functions, Methods, and Objects” (pp.106-144)
- this means its in the obj already
- constructor function is CAPITAL
- set var = new "ConstructorFunc"(pass, in, stuff)
- ConFunc then stores params in obj ay keys
```javascript
function Hotel (name, rooms, booked) {
this.name = name;
this.rooms = rooms;
this.booked = booked;
this.checkAvailability = function()
return this.rooms - this.booked;
} ;
var quayHotel
var parkHotel
new Hotel('Quay', 40, 25);
new Hotel( ' Park', 120, 77);
var details!= quayHotel .name + ' rooms : ';
detailsl += quayHotel.checkAvailability();
var elHotell = docurnent.getElementByid('hotell');
elHotell.textContent =details!;
var details2 = parkHotel .name+ ' rooms: ';
detai ls2 += parkHotel.checkAvailability();
var e1Hotel2 = document.getEl ementByid('hotel2');
elHotel2.textContent = details2; 
```
- literal notation vs. constructor notation
- this. referrs to suff in the obj
- array is an obj with numbered keys
- 

```javascript


function contentCreator(elementType, content){

  var element = document.createElement (elementType);

  element.textContent = content;

  return element;
}

var paragraph = contentCreator('p','some text');

var divElement = document.getElementId('content-box');

divElement.appendChild(paragraph);

//EXAMPLE OOP//
var seattle={


}
//constructor
function Store(){

  this.name = 'seattle';
  this.hours = [6,7,8]
}

Store.prototype.speak = function(){


}

var seattle = new Store();
```

