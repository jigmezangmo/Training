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

```
    .container {
    justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
    }
```

* flex-start (default): items are packed toward the start of the flex-direction.

* flex-end: items are packed toward the end of the flex-direction.

* start: items are packed toward the start of the writing-mode direction.

* end: items are packed toward the end of the writing-mode direction.

* left: items are packed toward left edge of the container.

* right: items are packed toward right edge of the container.

* center: items are centered along the line.

* space-between: items are evenly distributed in the line; first item is on the start line.

* space-around: items are evenly distributed in the line with equal space around them.

* space-evenly: items are distributed so that the spacing between any two items (and the space to the edges) is equal.

## Align-items

```
    .container {
    align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
    }
```

* stretch (default): stretch to fill the container (still respect min-width/max-width)

* flex-start / start / self-start: items are placed at the start of the cross axis. 

* flex-end / end / self-end: items are placed at the end of the cross axis. 

* center: items are centered in the cross-axis

* baseline: items are aligned such as their baselines align

# Align-content

```
    .container {
    align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
    }
```

* flex-start / start: items packed to the start of the container. 

* flex-end / end: items packed to the end of the container. 

* center: items centered in the container.

* space-between: items evenly distributed; the first line is at the start of the container while the last one is at the end.

* space-around: items evenly distributed with equal space around each line.

* space-evenly: items are evenly distributed with equal space around them
stretch (default): lines stretch to take up the remaining space


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






