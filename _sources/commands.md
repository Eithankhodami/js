# Commands in JavaScript

## Comments

Comments are used to explain the code and make it more readable. They can also be used to prevent execution of code.

### Single-line comments

Single-line comments begin with two slashes (//).

```javascript

// This is a single-line comment.

```

### Multi-line comments

Multi-line comments begin with a slash and an asterisk (/*) and end with an asterisk and a slash (*/).

```javascript

/* This is a
multiline comment. */

```

## Semicolons

JavaScript statements are separated by semicolons. If you omit the semicolon, JavaScript will insert it automatically. However, it is considered a good practice to terminate each statement with a semicolon.

```javascript

var myName = "John";
var myAge = 25;
var isMarried = false;

```

## typeof operator

The typeof operator returns the type of a variable or an expression.

```javascript

var myName = "John";
var myAge = 25;
var isMarried = false;

console.log(typeof myName); // string
console.log(typeof myAge); // number
console.log(typeof isMarried); // boolean

```
(console-log-fact)=
```{note}
you can assign more than one variable in console.log() function.

```javascript

const myName = "John";
const myAge = 25;
const isMarried = false;

console.log(typeof myName, typeof myAge, typeof isMarried); // string number boolean
```
```