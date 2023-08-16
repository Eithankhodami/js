# If-else statement
(02-if-else-statement)=
The If-else statement is so called control structure or conditional statement.

## What is if-else statement?

The if-else statement is used to execute a block of code if a condition is true, and another block of code if the condition is false.

## Syntax

```javascript
if (condition) {
  // code to be executed if condition is true
} else {
  // code to be executed if condition is false
}
```

## Example

```javascript
const myAge = 25;

if (myAge >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a teenager.");
}
```

```{note}
the `else` block is optional. So if you don't have it, the code will be executed if the condition is true and nothing will happen if the condition is false.
```

### Some importnat points

1. basically anything inside `{}` us so called `block of code`.

2. variable outside of code block is not accessible inside the code block.
 so that you have to be concern about.
you may think what does this mean? let's see an example:

```javascript
const birthYear = 1990;
// Now I want to see if person is from 20th or 21st century?
if (birthYear <= 2000) {
  century = 20;
} else {
    century = 21;
}

console.log(century); // Uncaught ReferenceError: myName is not defined
```

this basically means that you cannot access `myName` variable outside of the code block. 

Let's have some more example of using if-else statement:

```javascript
const myAge = 25;

if (myAge >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a teenager.");
}
```

```javascript
const x = 10;

if (x > 0) {
  console.log("x is a positive number.");
} else {
  console.log("x is a negative number.");
}
```

```javascript

time = 10;

if (time < 10) {
  console.log("Good morning.");
} else {
  console.log("Good day.");
}
```

something we want to have more than one condition. for example:

```javascript

time = 10;

if (time < 10) {
  console.log("Good morning.");
} else if (time < 20) {
  console.log("Good day.");
} else {
  console.log("Good evening.");
}
```

in such situation we use `else if` statement.

```{note}
you can have as many `else if` statement as you want.
```

```javascript

time = 10;

if (time < 10) {
  console.log("Good morning.");
} else if (time < 20) {
  console.log("Good day.");
} else if (time < 24) {
  console.log("Good evening.");
} else {
  console.log("Good night.");
}
```

```javascript
const myAge = 25;

if (myAge >= 18) {
  console.log("You are an adult.");
} else if (myAge >= 13) {
  console.log("You are a teenager.");
} else if (myAge >= 3) {
  console.log("You are a child.");
} else {
  console.log("You are a baby.");
}
```

```{seealso}
before continueing with this section, you may want to read about 
[Type coversions](03TypeConversion.md), 
also 
[truthy and falsy values](04TruthyFalsyValues.md). 
```

Now that you have learned about [Type coversions](03TypeConversion.md), also [truthy and falsy values](04TruthyFalsyValues.md); Let's have an example:

```javascript
const money = 0;
if (money) {
  console.log("Don't spend it all.");
} else {
  console.log("You should get a job!");
}
```
The result here is `You should get a job!` because `0` is a falsy value.

```javascript
const money = 100;

if (money) {
  console.log("Don't spend it all.");
} else {
  console.log("You should get a job!");
}
```

The result here is `Don't spend it all.` because `100` is a truthy value.