## HTML Tables :
HTML tables allow web authors to arrange data into rows and columns.

Defining an HTML Table :
An HTML table is defined with the `<table>` tag.

Each table row is defined with the `<tr>` tag. A table header is defined with the `<th>` tag. By default, table headings are bold and centered. A table data/cell is defined with the `<td>` tag.

Example :
~~~
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
~~~

### HTML Table - Adding a Border :
If you do not specify a border for the table, it will be displayed without borders.

A border is set using the CSS border property:

Example:
~~~
table, th, td {
  border: 1px solid black;
}
~~~

### HTML Table - Collapsed Borders :
If you want the borders to collapse into one border, add the CSS border-collapse property:

Example:
~~~
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
~~~

### Functions, Methods, and Objects 
Creating a JavaScript Object
Using the JavaScript Keyword new:

~~~
var person = new Object();
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue";
~~~

### Updating an object
~~~
var person = { firstName: "John", lastName: "Doe", age: 50, eyeColor: "blue" };

var x = person;
x.age = 10; // This will change both x.age and person.age
delete person lastname // this will delete the person lastname proberty
~~~

### Creatin many objects with constructor
~~~
function Vehicle(name, maker) {
   this.name = name;
   this.maker = maker;
}
let car1 = new Vehicle(’Fiesta’, 'Ford’);
let car2 = new Vehicle(’Santa Fe’, 'Hyundai’)
console.log(car1.name);    //Output: Fiesta
console.log(car2.name);    //Output: Santa Fe
~~~

### What is this?
The JavaScript this keyword refers to the object it belongs to.

It has different values depending on where it is used:

* In a method, this refers to the owner object.
* Alone, this refers to the global object.
* In a function, this refers to the global object.
* In a function, in strict mode, this is undefined.
* In an event, this refers to the element that received the event.
* Methods like call(), and apply() can refer this to any object.

### Arrays are objects
Objects are an unordered map from string keys to values, arrays are an ordered list of values (with integer keys). That’s the main difference. They’re both non-primitive, as they’re composed of multiple values, which also implies pass-by-reference in JavaScript.

Arrays are also a kind of object, though, so you can attach extra properties to them, access their prototype and so on.

In your revised example, you’re only taking advantage of the fact that an array is actually an object, i.e. you can set any property on them. You shouldn’t do that. If you don’t need an ordered list of values, use a plain object.

### Browser object model
The Browser Object Model (BOM) is used to interact with the browser.

The default object of browser is window means you can call all the functions of window by specifying window or directly.
![BOM](https://static.javatpoint.com/images/javascript/bom.jpg)

|      Method      |  Description
|------------------|----------------------------------------------------------------------------------------|
|    alert()	   |displays the alert box containing message with ok button.                               |
|    confirm()	   |displays the confirm dialog box containing message with ok and cancel button.           |
|    prompt()	   |displays a dialog box to get input from the user.                                       |
|    open()	       |opens the new window.                                                                   |
|    close()	   |closes the current window.                                                              |
|    setTimeout()  |performs action after specified time like calling function, evaluating expressions etc. |
|                  |                                                                                        |

Example:

~~~
//Example of alert() in javascript
function msg() {
  alert("Hello Alert Box");
}

//Example of confirm() in javascript
function msg() {
  var v = confirm("Are u sure?");
  if (v == true) {
    alert("ok");
  } else {
    alert("cancel");
  }
}
~~~

### Global object
In JavaScript, there’s always a global object defined. In a web browser, when scripts create global variables, they’re created as members of the global object.

#### Strings Object
The String object lets you work with a series of characters; it wraps Javascript’s string primitive data type with a number of helper methods.

As JavaScript automatically converts between string primitives and String objects, you can call any of the helper methods of the String object on a string primitive.
~~~
var val = new String(string);
~~~

### String Properties


|      Property    |  Description
|------------------|-------------------------------------------------------|
|    constructor   | Returns the string’s constructor function             |
|    length	       | Returns the length of a string                        |
|    prototype	   | Allows you to add properties and methods to an object |

### Number object
JavaScript has only one type of number.

Numbers can be written with, or without, decimals:
~~~
var x = 3.14;     // A number with decimals
var y = 34;       // A number without decimals
var x = 123e5;    // 12300000
var y = 123e-5;   // 0.00123
~~~

### Math Object
The Math object allows you to perform mathematical tasks.

Math is not a constructor. All properties/methods of Math can be called by using Math as an object, without creating it:
~~~
var x = Math.PI;            // Returns PI
var y = Math.sqrt(16);      // Returns the square root of 16
~~~

### Date Object
The Date object is used to work with dates and times.

Date objects are created with new Date().

There are four ways of instantiating a date
~~~
var d = new Date();
var d = new Date(milliseconds);
var d = new Date(dateString);
var d = new Date(year, month, day, hours, minutes, seconds, milliseconds);
~~~