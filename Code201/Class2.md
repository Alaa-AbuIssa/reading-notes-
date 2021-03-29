## HTML Headings
We use headings in HTML to provide valuable information by highlighting important topics and the structure of the document.

## How we write the heading??
![heading](https://www.theblogstarter.com/wp-content/uploads/2017/11/html-headings.png)

**And it shows up like this**
![show up](https://www.tutorialrepublic.com/lib/images/html/html-headings.png)

## HTML Paragraghs
Textual content in web pages is divided into HTML paragraphs. Web browsers add a margin (white space) after and before a paragraph automatically to separate them from one another.

To define a section of text as an HTML paragraph, you should use a pair of < p > tags:
![sections](https://ictacademy.com.ng/wp-content/uploads/2017/10/demo.png)

If we want to make a word inside the paragraph bold we should use < b > tag and put the word that we want to make it bold between the < b > and < /b > and also if we want to make it italic we just put the word between < i > and < /i >. *other formatting elements were designed to display special types of text:*
- Important text
- Italic text
- Emphasized text
- Marked text
- Smaller text
- Deleted text
- Inserted text
- Subscript text
- Superscript text
Using the formating text is very important in providing an idea to the user.

## To design your texts and adding some colors to it we use CSS, what is CSS??
Cascading Style Sheets is a style sheet language used for describing the presentation of a document written in a markup language like HTML.
![CSS](https://media.geeksforgeeks.org/wp-content/cdn-uploads/CSS-1024x341.png)

## How does CSS works?
CSS brings style to your web pages by interacting with HTML elements. Elements are the individual HTML components of a web page—for instance a paragraph—which in HTML might look like this:

< p >This is my paragraph!< /p > If you wanted to make this paragraph appear pink and bold to people viewing your web page through a web browser, you’d use CSS code that looks like this:

p { color:pink; font-weight:bold; } In this case, “p” (the paragraph) is called the “selector”—it’s the part of CSS code specifying which HTML element the CSS styling will effect. In CSS, the selector is written to the left of the first curly bracket. The information between curly brackets is called a declaration, and it contains properties and values that are applied to the selector. Properties are things like font size, color, and margins, while values are the settings for those properties. In the example above, “color” and “font-weight” are both properties, and “pink” and “bold” are values. The full bracketed set of

{ color:pink; font-weight:bold; } is the declaration, and again, “p” (meaning the HTML paragraph) is the selector. These same basic principles can be applied to change font sizes, background colors, margin indentations, and more. For instance. . .

body { background-color:lightblue; } . . .would make your page’s background light blue, or. . .

p { font-size:20px; color:red; } . . .will create a 20 point font paragraph with red letters.

## There are three ways of inserting a style sheet:
1- **External CSS** : With an external style sheet, you can change the look of an entire website by changing just one file! Each HTML page must include a reference to the external style sheet file inside the element, inside the head section.

2- **Internal CSS** : An internal style sheet may be used if one single HTML page has a unique style. The internal style is defined inside the < style > element, inside the head section.

3- **Inline CSS** : An inline style may be used to apply a unique style for a single element. To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

### To make our web-site interact with the user we should use JavaScript.

## So, What is JavaScript??
JavaScript is high-level, often just-in-time compiled, and multi-paradigm. It has curly-bracket syntax, dynamic typing, prototype-based object-orientation, and first-class functions. **So, JavaScrips is a group of statements that gives instructions and here is some of those statements :**
- JavaScript Comments : JavaScript comments can be used to explain JavaScript code, and to make it more readable. JavaScript comments can also be used to prevent execution, when testing alternative code.

- JavaScript Variables : JavaScript variables are containers for storing data values.

- JavaScript Arrays : JavaScript arrays are used to store multiple values in a single variable.

- JavaScript Expressions : An expression is any valid unit of code that resolves to a value.

- JavaScript Operators : JavaScript operators are used to assign values, compare values,perform arithmetic operations, and more.

-JavaScript Strings : JavaScript strings are used for storing and manipulating text.

## Decisions and Loops :
To make decisions we should use conditional statements that included in the JavaScript code assist with decision making, based on certain conditions. The condition specified in the conditional statement can either be true or false. The conditional statements execute the associated piece of code only if the condition is true.

## In JavaScript we have the following conditional statements:
1- Use *if* to specify a block of code to be executed, if a specified condition is true.

2- Use *else* to specify a block of code to be executed, if the same condition is false.

3- Use *else if* to specify a new condition to test, if the first condition is false.

4- Use *switch* to specify many alternative blocks of code to be executed.
![JS](https://miro.medium.com/max/925/1*dax3Mf7KuL1rQ5-RKjN6_A.png)

**To complet the conditinal statments we should use comparison operators so what is Comparison Operators :??** 
Comparison operators are used in logical statements to determine equality or difference between variables or values.

|   *The comparison symbol*	                | *the statements* | *the result*   |
| :---                                      |    :----:        |          ---:  |
| == is equal to                            |    x == 8	       |     false      |
| === is equal value and equal type         |    x === 5	   |     true       |       
| != is not equal	                        |    x != 8	       |     true       |
| !== is not equal value or not equal type	|    x !== 5	   |     false      |
| this > is greater than	                |    x > 8	       |     false      |
| < is less than	                        |    x < 8	       |     true       |
| this >= is greater than or equal to	    |    x >= 8	       |     false      |
| <= is less than or equal to	            |    x <= 8	       |     true       |


## the last thing - if you want to read more about the topic ; below you will find a helpful webpage :
[W3School](https://www.w3schools.com/html/html_scripts.asp)
