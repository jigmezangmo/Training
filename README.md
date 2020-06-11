# REPORTS 

## Flexbox Layout Module

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
* row (defaulf): left to right
* row-reverse: right to left
* column: top to bottom
* column-reverse: bottom to top

## Flex-wrap
* By default, flex items will all try to fit onto one line.

```
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

* nowrap (default): all flex items will be on one line
* wrap: flex items will wrap onto multiple lines, from top to bottom.
* wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

## Flex-flow
*   This is a shorthand for the flex-direction and flex-wrap properties, which together define the 
    flex container's main and cross axes. The default value is row nowrap.

```
.container {
  flex-flow: column wrap;
}
```

## Justify-content
* This 
