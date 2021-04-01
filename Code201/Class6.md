# Object Literal :

In plain English, an object literal is a comma-separated list of name-value pairs inside of curly braces.Those values can be properties and functions. Here’s a snippet of an object literal with one property and one function.

~~~
var greeting = {
    fullname: "Michael Jackson",
    greet: (message, name) => {
        console.log(message + " " + name + "!!");
    }
}
~~~

Object literal should be used if you want to create objects on the go with no intention of copying values to another object or maybe mapping one object to another.

## JavaScript HTML DOM :
With the HTML DOM, JavaScript can access and change all the elements of an HTML document.

## The HTML DOM (Document Object Model) :
When a web page is loaded, the browser creates a Document Object Model of the page. The HTML DOM model is constructed as a tree of Objects:
![DOM](https://www.w3schools.com/js/pic_htmltree.gif)

With the object model, JavaScript gets all the power it needs to create dynamic HTML:
~~~
- JavaScript can change all the HTML elements in the page
- JavaScript can change all the HTML attributes in the page
- JavaScript can change all the CSS styles in the page
- JavaScript can remove existing HTML elements and attributes
- JavaScript can add new HTML elements and attributes
- JavaScript can react to all existing HTML events in the page
- JavaScript can create new HTML events in the page
~~~

### What is the DOM?
The DOM is a W3C (World Wide Web Consortium) standard.

The DOM defines a standard for accessing documents:

*“The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document.”*

The W3C DOM standard is separated into 3 different parts:
1. Core DOM - standard model for all document types
2. XML DOM - standard model for XML documents
3. HTML DOM - standard model for HTML documents