toStyle
=======

Converts style objects to strings. Can be used on node or in the browser.

## Install

```npm install toStyle```

## Usage

```js
var toStyleString = require('to-style').string
var toStyleObject = require('to-style').object
```

### toStyleString

```js
toStyleString({
    border: {
        width: 1,
        color: 'red'
    },
    padding: 4,
    margin: {
        top: 5
    }
}) == 'border-width: 1px; border-color: red; padding: 4px; margin-top: 5px;'
```

### toStyleObject
```js

toStyleObject({
    padding: {
        top: 3,
        bottom: 2
    },
    border: '1px solid red',
    margin: 4
}) // =>
/*
{
    'padding-top': '3px',
    'padding-bottom': '2px',
    'border': '1px solid red',
    'margin': '4px'
}
 */
```


