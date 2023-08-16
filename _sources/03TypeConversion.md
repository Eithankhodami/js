# Type Conversion and type coercion

## Logic of Type Conversion

Type conversion is the process of converting one data type to another. For example:

we assume we have a text input and ask user to give us a number. but the user may enter a string. so we need to convert the string to number.

```js
let num1 = '10'; // string because it is user input, so we cannot add it to another number
```

so in this case we need to do type converstion.

```{tip}
you can convert a string to number by using `Number()` function.
```

`````{admonition} FACT!
:class: tip
function `Number()` when receives a string, it tries to convert it to number. if it cannot convert it, it returns `NaN` which means `Not a Number`.
`````

What is we want to convert a number to string?

```js
let num1 = 10; // number
```

so in this case we need to do type converstion.

```{tip}
you can convert a number to string by using `String()` function.
```
so we have:
    
```js
    console.log(String(num1)); // "10"
```


## Type Conversion

Type conversion is the process of converting one data type to another. There are two types of type conversion:

1. Implicit Type Conversion
2. Explicit Type Conversion

### Implicit Type Conversion

Implicit type conversion is done automatically by the compiler. For example:

```js
    let num1 = 10;
    let num2 = 20;
    let sum = num1 + num2;
    console.log(sum); // 30
```

In the above example, the compiler automatically converts the number data type to string data type.

### Explicit Type Conversion

Explicit type conversion is done manually by the programmer. For example:

```js
let num1 = 10;
let num2 = 20;
let sum = num1 + num2;

console.log(sum.toString()); // "30"
```

In the above example, the programmer manually converts the number data type to string data type.


## Type Coercion

Type coercion is the process of converting value from one type to another (such as string to number, object to boolean, and so on). Any type, be it primitive or an object, is a valid subject for type coercion. To recall, primitives are: number, string, boolean, null, undefined + Symbol (added in ES6).

One simple example is to:

```Javascript
  console.log('I am ' + 25 + ' years old');
```
in which JS automatically converts the number to string and concatenates them.

```{tip}
the opeator `+` is used for both addition and concatenation. so if we have two numbers, it adds them. but if we have a number and a string, it concatenates them.
```

```Javascript
  console.log('I am ' + 25 + ' years old');
```

```{tip}
the operator `-` , `*` , '/' actually acts different, it converts strings to number
```

```Javascript
  console.log('4' + '5'); // 9
```

```Javascript
  console.log('4' * '5'); // 20
```

```Javascript
  console.log('20' / '5'); // 4
```