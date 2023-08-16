# What is JavaScript?

java script is a high-level, interpreted programming language that conforms to the ECMAScript specification. JavaScript has curly-bracket syntax, dynamic typing, prototype-based object-orientation, and first-class functions.

Java is also high-level programming language but it is compiled language. Java is a general-purpose programming language that is class-based, object-oriented, and designed to have as few implementation dependencies as possible.

## which technology is used in javascript?
```{tip}
    -HTML
        html is for structure of the web page. it is used to create the basic structure of the web page.
    -CSS
        css is for styling of the web page. it is used to style the web page.
    -JavaScript
        javascript is for functionality of the web page. it is used to make the web page interactive. including animations, dynamic styling, dynamic content, etc.
```
```javascript
    console.log("Hello World");
```

## What is ECMAScript?

ECMAScript is a standard for a scripting language. It is a standardized specification of a scripting language developed by Brendan Eich of Netscape; initially it was named Mocha, later LiveScript, and finally JavaScript. JavaScript is the most widely used implementation of ECMAScript.

## What is the difference between JavaScript and ECMAScript?

JavaScript is a high-level programming language while ECMAScript is an international standard for programming languages. JavaScript is a dialect of the ECMAScript standard. JavaScript implements ECMAScript and builds on top of ECMAScript.

## Some notes about coding

1. JavaScript is case-sensitive. The language keywords, variables, function names, and any other identifiers must always be typed with a consistent capitalization of letters.
```javascript
    var myName = "John";
    var myname = "John";
    var MyName = "John";
    var MYNAME = "John";
    var myName = "John";
```
all the follwoing variables are different from each other.

2. JavaScript ignores multiple spaces. You can add white space to your script to make it more readable. JavaScript ignores spaces, tabs, and newlines that appear in JavaScript programs. You can use spaces freely in your script to format and indent it.

```javascript
    var myName = "John";
    var myName="John";
    var myName     =     "John";
    var myName
    =
    "John";
```
all the follwoing variables are same.

3. JavaScript ignores comments. JavaScript supports two styles of comments: single-line and multiline. Single-line comments begin with two slashes (//), and multiline comments begin with a slash and an asterisk (/*) and end with an asterisk and a slash (*/).

```javascript
    // This is a single-line comment.
    /* This is a
    multiline comment. */
```

4. JavaScript statements are separated by semicolons. JavaScript statements are separated by semicolons. If you omit the semicolon, JavaScript will insert it automatically. However, it is considered a good practice to terminate each statement with a semicolon.

```javascript
    var myName = "John";
    var myAge = 25;
    var isMarried = false;
```

5. It is better to follow standard coding in variable naming, so start with lowercase and then camel case.

```javascript
    var myName = "John";
    var myAge = 25;
    var isMarried = false;
```
or
```javascript
    var my_name = "John";
    var my_age = 25;
    var is_married = false;
```
5.1. You can use underscore in variable naming but it is not recommended.

```javascript
    var my_name = "John";
    var my_age = 25;
    var is_married = false;
```

6. You can use single quotes or double quotes for string values. It is recommended to use single quotes.

```javascript
    var myName = 'John';
    var myAge = "25";
```

7. You can use single quotes inside double quotes and double quotes inside single quotes.

```javascript
    var myName = "John's";
    var myAge = '25';
```

8. You can use backslash to escape quotes.

```javascript
    var myName = 'John\'s';
    var myAge = "25";
```

9. You can use backslash to escape backslash.

```javascript
    var myName = 'John\\';
    var myAge = "25";
```

10. You can use backslash to escape new line.

```javascript
    var myName = 'John\n';
    var myAge = "25";
```

11. you can use dollar sign als in naming.

```javascript
    var $myName = 'John';
    var myAge = "25";
```

12. imaging number 3.14 which is well-known as pi number, one important thing about pi is this is a fixed number and we don't change it, to show such cases, we can use uppercase letters.

```javascript
    var PI = 3.14;
```
interestingly JS automatically assign a different color for it.
## Values in JavaScript

1. JavaScript supports different types of values. The following are the most commonly used values in JavaScript:

    - Numbers
    NUMBERS are always having a floating datatype, for example
    ```javascript
        var myAge = 25;
        var mySalary = 2500.50;
    ```
    are both numbers. we maybe don't see the float in 25, but it is float.

    - Strings
    are used to name variables, always use single quotes for strings.
    ```javascript
        var myName = 'John';
    ```

    - Booleans
    are used to check conditions, for example
    ```javascript
        var isMarried = false;
    ```
    boolean values are always `true` or `false`. we use booleans to check conditions. or making decisions.
    - null
    is sort of value which is basically empty. it is used to initialize variables.
    ```javascript
        var myName = null;
    ```
    ```{caution}
    null is not an object. it is a primitive value. but it is a special primitive value. it is a special primitive value because typeof null returns "object".
    ```
    
    - undefined
    is sort of value which is basically empty. it is used to initialize variables.
    ```javascript
        var myName = null;
        var myAge = undefined;
    ```
    or for example if we create a `var` which is not assigned yet, it is `undefined`.
    ```javascript
        var myName;
    ```
    this is `undefined`.

    - BigInt
    it is sort of a big integer data which is hard to representative. later we discuss it.

```{tip}
Dynamic typing means that you don't have to specify the data type of a variable when you declare it. The JavaScript engine will automatically determine the data type of the variable when the program is being processed. JavaScript is a dynamically typed language. It means that you don't have to specify the data type of a variable when you declare it. The JavaScript engine will automatically determine the data type of the variable when the program is being processed. we can easily change the type of a variable. for example we can assign a number to a variable and then assign a string to it.
```
```{caution}
Dynamic can sometimes be the source of problem and bug in our code. for example if we assign a number to a variable and then assign a string to it, it will be a problem. because we can't do mathematical operations on strings. so we should be careful about it.
```
#### example of Dynamic typing

```javascript
    var myName = "John";
    console.log(myName);
    myName = 25;
    console.log(myName);
```
we can see that we can change the type of a variable.

```{tip}
using dynamic typing we have changed the `myName` variable from string to number.

to do so, without any extra code such as `var` or `let` simply put the variable name and assign a new value to it.
```

### Objects vs non-objects

1. JavaScript values are classified as objects and non-objects. The non-objects are called primitive values. The primitive values are the values that do not have properties or methods. The primitive values are immutable, which means that they cannot be changed. The primitive values are passed by value. The primitive values are as follows:

    - Numbers
    - Strings
    - Booleans
    - null
    - undefined

following example is an object:
    
```javascript
        var person = {
            firstName: "John",
            lastName: "Doe",
            age: 25,
            isMarried: false
        };
```
and this is a primitive value:
    
 ```javascript
        var myName = "John";
``` 


## Var, Let, and Const

1. JavaScript variables are containers for storing data values. JavaScript has three types of variables:

    - var
    - let
    - const

### let

`let` is assigned for which we want to change the value later. for example:

```javascript
    let myName = "John";
    myName = "Doe";
```
we can change the value of `myName` variable.

technical term for changing is **reassigning**; also this means that the variable is **mutable**. and we can change it.

### const

const is a sort of variable in which we are not supposed to change it anyway in future. so this is a **immutable** variable.

```javascript
    const myName = "John";
    myName = "Doe";
```
let's have an example:
for example birth year is always constant, so let's create it:

```javascript
const birthYear = 1991;
```
now if we want to change it, we get error.

```
birthYear = 1992;
```
we will get `TypeError`[Look at Errors here](Errors.md) or [here](constant-error)

```{tip}
`const` needs an initial value. so we can't create a `const` without initial value.
```

```javascript
const birthYear;
```
this is wrong. and we get `SyntaxError`[Look at Errors here](Errors.md) or [here](constant-initial-error)

```javascript
const birthYear = 1991;
```
this is correct.

```{note}
Maybe there is question, which one should we use? `let` or `const`?

the answer is, it depends on the situation. if we want to change the value of a variable, we should use `let`. but if we don't want to change the value of a variable, we should use `const`.
```

### Var

`var` is the old way of creating variables. it is not recommended to use `var` anymore. but we should know it because we may face it in old codes.

```javascript
    var myName = "John";
    myName = "Doe";
```

```{note}
I also in some point up to now have used `var` but as I already mentioned, it is not recommended to use `var` anymore.
```
## Operators

An operator is basically an option which gives us chance to do some operations on our values. for example we can do mathematical operations on numbers.

operators are divided into different categories:

1. Arithmetic operators
2. Assignment operators
3. Comparison operators
4. Logical operators
5. Bitwise operators

### Arithmetic operators
Or let's so call Mathematical Opeators

1. Addition (+)

```javascript
    var x = 5;
    var y = 2;
    var z = x + y;
```

another example:

```javascript
    const yearNow = 2023;
    const userBirthdate = 1990;
    const age = yearNow - userBirthdate;
    console.log(z);
```
and you will get `33` as output.

```{seealso}
```{tip}
[`Consol.log` Mulitple `const` passing](console-log-fact)
```

Another thing we can do is concatenation. for example:

```javascript
    const firstName = "John";
    const lastName = "Doe";
    const fullName = firstName + " " + lastName;
    console.log(fullName);
```

2. Subtraction (-)

```javascript
    const x = 5;
    const y = 2;
    const z = x - y;
```
3. Multiplication (*)

```javascript
    const x = 5;
    const y = 2;
    const z = x * y;
```
4. Division (/)

```javascript
    const x = 5;
    const y = 2;
    const z = x / y;
```
5. Modulus (%)

```javascript
    const x = 5;
    const y = 2;
    const z = x % y;
```

6. Increment (++)

```javascript
    const x = 5;
    x++;
```
Basically what does it mean? it means that we add 1 to the variable. so if we have `x = 5` and we increment it, we will have `x = 6`.

7. Decrement (--)

```javascript
    const x = 5;
    x--;
```

Basically what does it mean? it means that we subtract 1 from the variable. 
so if we have `x = 5` and we decrement it, we will have `x = 4`.

### Assignment operators

there are some operators which you need to know them. 

1. `=+`

```javascript
        const x = 5;
        x += 2;
```

Basically what does it mean? it means that we add 2 to the variable. 
so if we have `x = 5` and we add 2 to it, we will have `x = 7`.

2. `-=`

```javascript
        const x = 5;
        x -= 2;
```

Basically what does it mean? it means that we subtract 2 from the variable. 
so if we have `x = 5` and we subtract 2 from it, we will have `x = 3`.

3. `*=`

```javascript
            const x = 5;
            x *= 2;
```
Basically what does it mean? it means that we multiply 2 to the variable. 
so if we have `x = 5` and we multiply 2 to it, we will have `x = 10`.

4. `/=`

```javascript
        var x = 5;
        x /= 2;
```
Basically what does it mean? it means that we divide 2 from the variable. 
so if we have `x = 5` and we divide 2 from it, we will have `x = 2.5`.

5. `%=`

    ```javascript
            const x = 5;
            x %= 2;
    ```
Basically what does it mean? it means that we get the remainder of dividing 2 from the variable. 
so if we have `x = 5` and we get the remainder of dividing 2 from it, we will have `x = 1`.


## Comparison operators

Comparison operators are used in logical statements to determine equality or difference between variables or values.

1. `==`

```javascript
        const x = 5;
        const y = 2;
        console.log(x == y);
```
Basically what does it mean? it means that we check if x is equal to y.

&#8594; The asnwer for this is `false`.

```{note}
so basically we can say that comparison operators return boolean values.
```

2. `===`

```javascript
        const x = 5;
        const y = 2;
        console.log(x === y);
```

Basically what does it mean? it means that we check if x is equal to y and also they are the same type.

&#8594; The asnwer for this is `false`.

3. `!=`

```javascript
        const x = 5;
        const y = 2;
        console.log(x != y);
```

Basically what does it mean? it means that we check if x is not equal to y.

&#8594; The asnwer for this is `true`.

4. `!==`

```javascript
        const x = 5;
        const y = 2;
        console.log(x !== y);
```

Basically what does it mean? it means that we check if x is not equal to y or they are not the same type.

&#8594; The asnwer for this is `true`.

5. `>`

```javascript
        const x = 5;
        const y = 2;
        console.log(x > y);
```

Basically what does it mean? it means that we check if x is greater than y.

&#8594; The asnwer for this is `true`.

6. `<`

```javascript
        const x = 5;
        const y = 2;
        console.log(x < y);
```

Basically what does it mean? it means that we check if x is less than y.

&#8594; The asnwer for this is `false`.

7. `>=`

```javascript
        const x = 5;
        const y = 2;
        console.log(x >= y);
```

Basically what does it mean? it means that we check if x is greater than or equal to y.

&#8594; The asnwer for this is `true`.

8. `<=`

```javascript
        const x = 5;
        const y = 2;
        console.log(x <= y);
```

Basically what does it mean? it means that we check if x is less than or equal to y.

&#8594; The asnwer for this is `false`.

## Precedence of operators

The precedence of operators determines the order they are applied when evaluating an expression. You can override operator precedence by using parentheses.

```javascript
        const x = 5;
        const y = 2;
        const z = 4;
        console.log(x + y * z);
```

&#8594; The asnwer for this is `13`.

```javascript
        const x = 5;
        const y = 2;
        const z = 4;
        console.log((x + y) * z);
```

&#8594; The asnwer for this is `28`.

```{caution}
although normal operators works from left to right, but there are some operators which works from right to left. for example `++` and `--`.
```

```JavaScript
        const x = 5;
        const y = 2;
        const z = 4;
        console.log(x + y++ * z);
```

&#8594; The asnwer for this is `13`.

```JavaScript
        const x = 5;
        const y = 2;
        const z = 4;
        console.log(x + ++y * z);
```

or for example:

```JavaScript
        let x, y;   //we can create multiple variables in one line.
        x = y = 25-10+5;
        console.log(x, y);
```

&#8594; The asnwer for this is `20 20`.

Why is that so lets take a look at the way it is done

Javascript first does the mathmatical part which is `25-10+5` and then assign it to `y` and then assign `y` to `x`.


