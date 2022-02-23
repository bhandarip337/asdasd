    
    <input type="button" value="Print / Make PDF" onclick="window.print()">

<div align="center">

[**_``Go Back``_**](../README.md)
    
<a onclick="window.print()">
    
    [**_``Print as pdf``_**]
    
</a>
    
# JavaScript

</div>

## Introduction
----------------------

``JavaScript`` is a lightweight, cross-platform, and interpreted scripting language used to make webpages interactive (e.g., having complex animations, clickable buttons, popup menus, etc.). It is well-known for the development of web pages, many non-browser environments also use it. JavaScript can be used for ``Client-side`` developments as well as ``Server-side`` developments. JavaScript contains a standard library of objects, like ``Array``, ``Date``, and ``Math``, and a core set of language elements like ``operators``, ``control structures``, and ``statements``. 
SSS
* **``Client-side:``** It supplies objects to control a browser and its ``Document Object Model (DOM)``. Like if client-side extensions allow an application to place elements on an HTML form and respond to user events such as ``mouse clicks``, ``form input``, and ``page navigation``. Useful libraries for the client-side are ``AngularJS``, ``ReactJS``, ``VueJS`` and so many others.
    
* **``Server-side:``** It supplies objects relevant to running JavaScript on a server. Like if the server-side extensions allow an application to communicate with a database, and provide continuity of information from one invocation to another of the application, or perform file manipulations on a server. The useful framework which is the most famous these days is ``node.js``.

## Need of Client Side Scripting Language
-------------------------------------------

Using a client-side script for interactivity in a Web application usually provides the appearance of better performance than using a server-side script to implement the same functionality because the client-side script does not incur the delay of a round trip between the client and the server, making the Web application more responsive. This is crucial for a dynamic user experience in a Web application. As an extreme example, imagine that a developer wants to limit input to a text box to only numbers. Each time the user hits a key, the character entered must be examined and thrown away if it's not a number or cursor movement key. Imagine the delay if the application had to wait for a round trip between the client and server and redraw the page for each keystroke. Obviously, such a feature would never be practical in a Web application if it were not for client-side scripting. Client-side scripting allows many features to be easily incorporated in Web applications that would otherwise be impractical.

In addition, client-side scripting offers the benefit of off-loading part of the computational demands of an application from the server to the client. The client-side computer is usually wasting most of its processing potential, idly waiting for the user to do something. Web servers, on the other hand, are usually taxed to their limit, serving hundreds or thousands of concurrent users.

The two main benefits of client-side scripting are:

* The user’s actions will result in an immediate response because they don’t require a trip to the server.
* Fewer resources are used and needed on the web-server.

## Formatting and Coding Convetions
-------------------------------------

Coding conventions are **style guidelines for programming**. They typically cover:

* Naming and declaration rules for variables and functions.
* Rules for the use of white space, indentation, and comments.
* Programming practices and principles.

Coding conventions secure quality:

* Improves code readability.
* Make code maintenance easier.

### **Variable Names**

The name of a variable must begin with a letter and ``camelCase`` is used to initialize variables or functions which means the first letter should be a small letter and if another word is added after the first word then the first letter of that word should be capitalized.

```JS
let fullName = "Prashant Bhandari";
```

### **Indentation and function**

JavaScript coding conventions say that use two spaces to indent JavaScript code, and never use trailing whitespaces. For functions, use ``camelCase`` and to define a function use the keyword function:

```JS
function myFunc(){
  var x=0;
}
```

### **Spaces, all brackets**

Always leave spaces between operators such as ``(= + – * /)`` and ``commas``:

```JS
let name = fName + lName;
const myArray = ["cat", "mouse", "dog"];
```

### **Object guidelines**

For using objects, the coding standards include the following points:

* The starting bracket should be placed on the same line as the object name.
* Between an object’s property and its value is a colon and a space.
* String values are covered with double quotations.
* Numeric values are simply written and quotes are not used.
* A comma is used after every property value pair except the last one
* After the object closing bracket, add a semicolon.
* Objects that have fewer properties can be compressed and written on the same line by having spaces between properties.

```JS
let person = {
  firstName: "Jackie",
  lastName: "Chan",
};
//can also be written in compress form
let person = {firstName:"Jackie", lastName:"Chan"};
```

### **Statement Guidelines**

A simple statement like initializing a variable that ends on a single line should have a semicolon at the end of the line:

```JS
let name = "Jackie Chan";
```

For a compound sentence, leave a space and place an opening bracket after which then fill in the rest of the sentences in that opening bracket. Once all the statements are finished, put a closing bracket. It should be noted that in a compound sentence we don’t put a semicolon at the end of it:

```JS
for (i = 0; i < 3; i++) {
  a *= i;
}
```

### **Line Length**

Standard coding and conventions say that lines length greater than 80 should be written on another line by breaking the original line so that the code becomes more readable:

```JS
document.getElementById("example").innerHTML =
"Example!";
```
### **File Extensions**

Javascript coding standards and conventions say that the ``HTML`` file should have a ``.html`` extension, the ``CSS`` file should have a ``.css`` extension and the ``Javascript`` file should have a ``.js`` extension.

### **Loops and Conditions**

After a control statement’s identification, and after every comma use whitespace. The conditional statements coding conventions and standards code is given below:

```JS
if (condition1 || condition2) {
  // some statements
}
else if (condition3 && condition4) {
  // some other statements
}
else {
  // default statements
}
```

For loop follow the below code:

```JS
for (let i = 0; i < 5; i++) {
  x += i;
}
```

### **Comments**

Block comments are avoided according to coding standards and conventions and line comments are used. Comments are put in the left margin and ``//`` are put in the start.

```JS
// an example
let name = "Ram";
```

## JavaScript Files
-------------------------

A JavaScript file is a text file containing ``JavaScript`` code that is used to execute JavaScript instructions in webpages. It may include functions that open and close windows, validate form fields, enable rollover images, or create dropdown menus.JavaScript file must be saved by ``.js`` extension.

## Comments
-------------

JavaScript comments can be used to explain JavaScript code, and to make it more readable. JavaScript comments can also be used to prevent execution, when testing alternative code.

### **Single Line Comments**

Single line comments start with ``//``.

Any text between ``//`` and the end of the line will be ignored by JavaScript (will not be executed).

This example uses a single-line comment before each code line:

```JS
// Change heading:
document.getElementById("myH").innerHTML = "My First Page";
// Change paragraph:
document.getElementById("myP").innerHTML = "My first paragraph.";
```

### **Multi-line Comments**

Multi-line comments start with ``/*`` and end with ``*/``.

Any text between ``/*`` and ``*/`` will be ignored by JavaScript.

This example uses a multi-line comment (a comment block) to explain the code:

```JS
/*-------------------------------
The code below will change
the heading with id = "myH"
and the paragraph with id = "myP"
in my web page:
-------------------------------*/
document.getElementById("myH").innerHTML = "My First Page";
document.getElementById("myP").innerHTML = "My first paragraph.";
```

## Embedding JavaScript in HTML
----------------------------------

JavaScript can be added to your HTML file in two ways:

* Internal JS
* External JS

### **Internal JS:** 
We can add JavaScript directly to our HTML file by writing the code inside the ``<script>`` tag. The ``<script>`` tag can either be placed inside the ``<head>`` or the ``<body>`` tag according to the requirement.

Syntax:

```HTML
<script>
    // JavaScript Code
</script>
```
Example:

```HTML 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Example</title>
</head>
<body>
    <script>
        alert("This is JavaScript");
        console.log("This is JavaScript");
        document.write("This is JavaScript");
    </script>
</body>
</html>
```

### **External JS:** 
In order to accommodate larger scripts or scripts that will be used across several pages, JavaScript code generally lives in one or more js files that are referenced within HTML documents, similarly to how external assets like CSS are referenced.

The benefits of using a separate JavaScript file include:

* Separating the HTML markup and JavaScript code to make both more straightforward.
* Separate files makes maintenance easier.
* When JavaScript files are cached, pages load more quickly.

We can write JavaScript code in other file having an extension ``.js`` and then link this file inside the ``<head>`` tag of the HTML file in which we want to add this code.

How to link:

```HTML
<script src="js file path"></script>
```
Example:

Folder Structure

```
Example2
    ├──index.html
    └──js
        └── logic.js

```

**Content of ``index.html`` :**

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script src="js/logic.js"></script>
    <title>Example2</title>
</head>
<body>
    <script>
        printdate();
    </script>
</body>
</html>
```

**Content of ``logic.js`` :**

```JS
function printdate()
{
    let d = new Date();
    document.body.innerHTML = "<h1>Today's date is " + d + "</h1>";
}
```

## Using Script Tag
--------------------

The ``<script>`` tag is used to embed a client-side script (JavaScript).

The ``<script>`` element either contains scripting statements, or it points to an external script file through the src attribute.

Example:

```HTML
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```

## NoScript Tag
---------------------

The ``<noscript>`` tag defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support script.

The ``<noscript>`` element can be used in both ``<head>`` and ``<body>``. When used inside ``<head>``, the ``<noscript>`` element could only contain ``<link>``, ``<style>``, and ``<meta>`` elements.

Example:

```HTML
<script>
document.write("Hello World!")
</script>
<noscript>Your browser does not support JavaScript!</noscript>
```
