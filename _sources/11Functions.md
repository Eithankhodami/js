# Functions

## What are functions?
(11-functions)=

A function is a block of code designed to perform a particular task. A function is executed when "something" invokes it (calls it).

## Why functions?

1- You can reuse code: Define the code once, and use it many times.

2- You can use the same code many times with different arguments, to produce different results.

## Syntax of a function

```js

function name() {
  // code to be executed
}

```

for example:

```js
function myFunction() {
  console.log("Hello World!");
}

myFunction(); // call the function
```


## Function Parameters

Information can be passed to functions as a parameter. Parameters are specified after the function name, inside the parentheses. You can add as many parameters as you want, just separate them with a comma.

```js
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

the other parameter which a `function` can get is  `return` value.

```js
function name(parameter1, parameter2, parameter3) {
  // code to be executed
  return value;
}
```

Let's see a real example:

we assume we want to create a function in which we receive 3 marks scores and function calculates the average of them and return the average.

```js
function average(m1, m2, m3) {  
  let avg = (m1 + m2 + m3) / 3;       // calculate the average
  return messageToStudent = `Your average is ${avg} for this year`;  // return the average
}

let result = average(10, 15, 30);  // call the function
console.log(result);  // print the result
```

Now if you want to calculate the average of 3 students, you can call the function 3 times.

```js
let result1 = average(10, 15, 30);  // call the function
console.log(result1);  // print the result

let result2 = average(20, 25, 30);  // call the function
console.log(result2);  // print the result

let result3 = average(30, 35, 40);  // call the function
console.log(result3);  // print the result
```

Let's have a bigger example:

We want to calculate the average of 3 Marks for 3 course. if the average is more than 10, the student will pass the course, otherwise the student will fail the course. and if average is more than 18, then student will pass and get a prize.

```js

function average(m1, m2, m3) {
  let avg = (m1 + m2 + m3) / 3; 

  if (avg > 10 && avg > 18) {
    return message = `your average is ${avg} and you pass the course and get a prize`;
  } else if (avg > 10) {
    return message = `your average is ${avg} and you pass the course`;
  } else {
    return message = `your average is ${avg} and you fail the course`;
  }
}

let result1 = average(10, 15, 18);  // call the function
console.log(result1);  // print the result
```

Also we can use `Switch` to do the same:

```js
function average(mark1, mark2, mark3) {
  let avg = (mark1 + mark2 + mark3) / 3;

  switch(true) {
    case (avg > 18):
      return `Your average is ${avg} and you pass the course and get a prize!`;
    
    case (avg > 10):
      return `Your average is ${avg} and you pass the course`;

    default:
      return `Your average is ${avg} and you fail the course`;
  }
}
let result1 = average(10, 15, 18);
console.log(result1);
```
 

 