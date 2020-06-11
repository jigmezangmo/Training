# REPORTS 

# Flexbox Layout Module

* The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

## Display

*  This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

```
    <html>
        <head>
            <link rel = "stylesheet" href = "style.css">
        <head>
        <body>
            <nav class = "container">
                <div> Home </div>
                <div> Search </div>
                <div> Logout </div>
            </nav>
        </body>
    </html>

    CSS
        .container {
        display: flex;
        }
```

## Flex-direction

* It establishes the main-axis, thus defining the direction flex items are placed in  the flex container.

```
    .container {
    flex-direction: row | row-reverse | column | column-reverse;
    }
```
*   row (defaulf): left to right
*   row-reverse: right to left
*   column: top to bottom
*   column-reverse: bottom to top

## Flex-wrap

* By default, flex items will all try to fit onto one line.

```
    .container {
    flex-wrap: nowrap | wrap | wrap-reverse;
    }
```

*   nowrap (default): all flex items will be on one line
*   wrap: flex items will wrap onto multiple lines, from top to bottom.
*   wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

## Flex-flow

*   This is a shorthand for the flex-direction and flex-wrap properties, which together define the 
    flex container's main and cross axes. The default value is row nowrap.

```
    .container {
    flex-flow: column wrap;
    }
```

## Justify-content

```
    .container {
    justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
    }
```

*   flex-start (default): items are packed toward the start of the flex-direction.

*   flex-end: items are packed toward the end of the flex-direction.

*   start: items are packed toward the start of the writing-mode direction.

*   end: items are packed toward the end of the writing-mode direction.

*   left: items are packed toward left edge of the container.

*   right: items are packed toward right edge of the container.

*   center: items are centered along the line.

*   space-between: items are evenly distributed in the line; first item is on the start line.

*   space-around: items are evenly distributed in the line with equal space around them.

*   space-evenly: items are distributed so that the spacing between any two items (and the space to the edges) is equal.

## Align-items

```
    .container {
    align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
    }
```

*   stretch (default): stretch to fill the container (still respect min-width/max-width)

*   flex-start / start / self-start: items are placed at the start of the cross axis. 

*   flex-end / end / self-end: items are placed at the end of the cross axis. 

*   center: items are centered in the cross-axis

*   baseline: items are aligned such as their baselines align

# Align-content

```
    .container {
    align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
    }
```

*   flex-start / start: items packed to the start of the container. 

*   flex-end / end: items packed to the end of the container. 

*   center: items centered in the container.

*   space-between: items evenly distributed; the first line is at the start of the container while the last one
    is at the end.

*   space-around: items evenly distributed with equal space around each line.

*   space-evenly: items are evenly distributed with equal space around them
    stretch (default): lines stretch to take up the remaining space.

# Grid Layout

* The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier
  to design web pages without having to use floats and positioning.

## Display

* Defines the element as a grid container and establishes a new grid formatting context for its contents.

```
    .container {
    display: grid | inline-grid;
    }
```

* Values:
    - grid – generates a block-level grid
    - inline-grid – generates an inline-level grid


## Grid-template-columns / Grid-template-rows

```
    .container {
    grid-template-columns:  ... |   ...;
    grid-template-rows:  ... |   ...;
    }
```

* Values:

    - <track-size> – can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)
    - <line-name> – an arbitrary name of your choosing

## Grid-template-areas

```
    .container {
    grid-template-areas: 
    " | . | none | ..."
    "...";
    }
```

* Values:

    - <grid-area-name> – the name of a grid area specified with grid-area

    - . – a period signifies an empty grid cell

    - none – no grid areas are defined

## Grid-template

*  A shorthand for setting grid-template-rows, grid-template-columns, and 
   grid-template-areas in a single declaration.

```
    .container {
    grid-template: none | <grid-template-rows> / <grid-template-columns>;
    }
```


# Introduction to Programming

## Evolution of Computing Devices

    *   1940 -  ENIAC (size of 3-4 double decker buses)
    *   1947 -  Transistors (size of the vaccum tubes and consumed less power)
    *   1958 -  Integrated Circuits (Jack Kilby and Robert Noyce)
    *   1968 -  Intel Electronics (Robert Noyce)

## Binary Number System

    *   Base 2 number System
    *   Computer understand only 0 and 1
    *   0 and 1 are also called bit ("Binary Digit")
    *   8 bit is 1byte
    *   A byte can represent 256 values
    *   2^ * place multiplier

## Memory Classification

    *   Registers
    *   Cache
    *   Primary Memory (RAM)
    *   Secondary Memory (Hard Disks etc.)

## High Level Language

    *   Compiler -> Machine specific assembler -> Machine language (Fortran, Algol in 1950's and 60's)
    *   Translate to machine code using "Assembler"

## Stack & Heap

    *   Stack and Heap Memory Space used by programs
    *   Allocated on RAM
    *   Stack us used for static memory allocation and Heap for dynamic memory allocation


# Java Script Introduction

* Java Script adds programming to our web pages. Works with HTML and CSS to make up the website.

* We place the JavaScript code into the webpage and the browser executes it.

## Variables

    *   Variable naming can only start with letter
    *   Variable are case sensitive
    *   Must always start with VAR
    *   Numeric variables - numbers
    *   String variables - text and characters - must use double quotation marks
    *   Boolean - True or False
    *   Using and external file

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

## Data Types

* Variables and Data-types : String

```
    var firstName = 'Jigme';
    console.log(firstName);
```

* Number type

```
    var lastName = 'zangmo';
    var age = 20;
```

* Boolean type

```
    var fullAge = true;
    console.log(fullAge);
```

* undefine

```
    var job;
    console.log(job);

    job = 'Teacher';
    console.log(job);
```

* Variable naming rules

```
    var _3years = 3;
    var jigmeZangmo = 'Jigme and Mark';
    console.log(_3years);
    console.log(jigmeZangmo);
```

* Variable mutation and type coercion

```
    var firstName = 'jigme';
    var age = 25;

// Type coercion

    console.log(firstName + ' ' + age);

    var job, isMarried;
    job = 'teacher';
    isMarried = false;
    console.log(firstName + ' is a ' + age + ' year old '
    + job + '. Is he married? ' + isMarried);

// Variable mutation

    age = "twenty five";
    job = 'cook';

    alert(firstName + ' is a '+ age + ' year old '
    + job + '.Is he married? ' + isMarried);

    var lastName = prompt('what is his last Name?');
    console.log(firstName + ' ' + lastName);
```

## Basic Operators

```
    var year, yearJigme, yearZangmo;
    now = 2020;
    ageJigme = 25;
    ageZangmo = 34;


// Math Operators

    yearJigme = now - ageJigme;
    yearZangmo = now - ageZangmo;

    console.log(yearZangmo);

    console.log(now + 2);
    console.log(now * 4);
    console.log(now / 10);


// Logical Operators

    var jigmeOlder = ageJigme > ageZangmo;
    console.log(jigmeOlder);


// typeof Operator

    console.log(typeof jigmeOlder);
    console.log(typeof ageZangmo);
    console.log(typeof 'Zangmo is older than Jigme');
    var x;
    console.log(typeof x);
```

# Webpack

*   Webpack is a static module bundler.
*   In a particular project, webpack treats all files and assests as modules.

```
             Webpack // builds
                | 
            Dependency Graph
                | // It doesn't execute "statically" the source code but stitches modules & their dependencies
                |     together into bundles
              Bundle
```

## Webpack Main Concepts

1.  Entry

*   Is a module, which webpack uses to start building its internal dependency graph.
*   Entry property is set to ./src/index.js

2.   Output

*   Output property instructs webpack where to emit the bundles(s) & what to use for that
    file(s).
*   The default value for this property is 
        -   ./dist/main.js - for the main bundle
        -   ./dist- for other generated files. (eg: img)

3.  Loaders

*   By default, webpack only understands JavaScript & JSON files.
*   Loaders is use to convert other types of files into valid modules.

4.  Plugins

*   Are used for any other task that loaders can't do.

5.  Mode

*   Development: "webpack --mode developement"
*   Building: "webpack --mode production".

# DOM ( Standard Object Model )

##   What is the DOM?

*   Document Object Model (DOM) is a platform & language-neutral interface that allows programs & scripts to
    dynamically access & update the content, structure, & style of a document.

*   HTML DOM is a standard for how to get, change, add, or delete HTML elements.

## HTML DOM Methods

*   HTML DOM methods are actions you can perform (on HTML Elements).
*   HTML DOM properties are values (of HTMl Elements) that you can set or change.
*   A property is a value that you can get or set (like changing the content of an HTML elements).
*   A method is an action you can do (like ad or deleting an HTML element).

## Changing HTML Content

```
    Syntax: document.getElementById(id).innerHTML= new HTML
```

## Changing the Value of an Attributes

```
    Syntax: document.getElementById(id).attribute= new value
```

## Changing HTML Style

```
    Syntax: document.getElementById(id).style.property= new style
```

# Using Events

*   HTML DOM allows to execute code when an event occurs.
*   Events are generated by the browser when "things happen" to HTML elements.
        -   An element is clicked on.
        -   The page has loaded.
        -   Input fileds are changed.








