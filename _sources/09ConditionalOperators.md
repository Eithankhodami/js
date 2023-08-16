# Conditional Operators

## What is Conditional Operator?
(08-ternary-operator)=
Conditional operator is a ternary operator (or 3 parts operator as it has 3 parts) that takes three operands. It is also known as the ternary operator. It is the only operator in JavaScript that takes three operands. It is a shorthand for if...else statement.

let's define the way how to write with an example:

Let's assume if your age is more than 18 and if yes, you can drink beer otherwise you can't drink beer.

```js
let age = 20;
let canDrinkBeer = age > 18 ? console.log(`yes, you can drink`) : console.log(`no, you can't drink`);
```

## Syntax

```js
condition ? expression1 : expression2;
```
we can define `expression1` as `if block` and `expression2` as `else block`.

Also there is possibility to shorten the code:

```js
let age = 20;
let canDrinkBeer = age > 18 ? `yes, you can drink` : `no, you can't drink`;
console.log(canDrinkBeer);
```

```{note}
Since that is a ternary operator, it is possible to use it as a statement or as a [](01template-literals)expression.
```

```js
console.log(`I would like to drink ${age > 18 ? 'beer' : 'juice'}`)
```

Another example:

```js
const budget = 130;
const price = 120;
console.log (budget > price ? 'you can buy it' : 'you can not buy it');
```

```{caution}
we should not use [Ternary Operators](08-ternary-operator) as replacement of [conditional statements](02-if-else-statement) statement. It is just a shorthand for `if...else` statement.
```


