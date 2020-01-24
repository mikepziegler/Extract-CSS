# Extract-CSS

This package is for extracting css classes, ids and elements and providing them as a JSON Object

## Installation

```
npm install @types/d3 --save-dev
```

## How to use

1. Point to a CSS File

Javascript
```
var ExtractCSS = require("extract-style");
var style = ExtractCSS("path/to/stylesheet.css");
```

2. Get desired Objects

Here is an example of a css file:

```
.container {
    max-width: 1200px;
    margin: 0px auto;
}

.center {
    display: flex;
    align-items: center;
    justify-content: center;
}

#ExampleId {
    background-color: aqua;
}

h1 {
    font-size: 30px;
}
```

Get CSS Class
```
var  container = style.Classes.container
```

Get CSS ID
```
var ExampleId = style.IDs.ExampleId
```

Get CSS Element
```
var h1 = style.Elements.h1
```
