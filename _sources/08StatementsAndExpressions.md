# Statements and Expressions

## Statements

A statement is an instruction to perform a specific action. For example, the following code is a statement that tells the browser to display the string "Hello World!" inside an alert box:

```js
alert("Hello World!");
```

## Expressions

An expression is a combination of values, variables, and operators that evaluates to a single value. For example, the following code is an expression that evaluates to the number 5:

```js
3 + 2;
```

## Difference between Statements and Expressions

The main difference between statements and **expressions is that statements do not return a value** while expressions do.

```{note}
JS is a sequence of statements. IN ANOTHER WORD when our code contains a semi-colon, it is a statement. When it does not contain a semi-colon, it is an expression.
```

I hope that you remember [](01template-literals), so in the template literal, we use expressions in `${}`.

```js
const myName = "John";
const myAge = 25;
const birthYear = 1995;
const job = "teacher";

console.log(`My name is ${myName}. I am ${myAge} years old. I was born in ${birthYear}. I am a ${job}.`);
```

to remember what which is between `${}` is an expression.


