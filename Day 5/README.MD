# Java Script Introduction

* Java Script adds programming to our web pages. Works with HTML and CSS to make  up the website.

* We place the JavaScript code into the webpage and the browser executes it.

## Variables

* Variable naming can only start with letter
* Variable are case sensitive
* Must always start with VAR
* Numeric variables - numbers
* String variables - text and characters - must use double quotation marks
* Boolean - True or False

## Using and external file

```
<!doctype html>
<html lang= "en">
<head>
<script src= "test.js"> </script>
</head>
</html>
```

## Functions

* Functions plays an important role in JavaScript along with variables, they form basic blocks of JavaScript.

```
function saySomething (){
    // all the statement go inside curly braces
    alert ("This is a function");
}
saySomething ();

# Example
 
function addSomething (num, str) {
    var add = num + str;
    alert (add);
}
addSomething (200, "program to write");
```



