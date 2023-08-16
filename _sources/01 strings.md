# Strings 

## What is String?

A string is a sequence of characters. In Python, strings are enclosed inside single quotes, double quotes, or triple quotes. 

As we already discussed, string has to be in either single quotes, double quotes, or triple quotes. 

```JavaScript
const myName = "John";
```

or

```JavaScript
const myName = 'John';
```

Let's have a practice:

```JavaScript
const myName = "John";
const myAge = 25;
const birthYear = 1995;
const job = "teacher";
```

now lets cancatenate these variables:

```JavaScript
console.log("My name is " + myName + ". I am " + myAge + " years old. I was born in " + birthYear + ". I am a " + job + ".");
```

**One problem** in such format is the problem of using spaces between strings, which is not a good practice.

**Another problem** is that we have to use `+` operator to concatenate strings.

**Solution** is to use **template literals**.

(01template-literals)=
## Template literals

Template literals are string literals allowing embedded expressions. You can use multi-line strings and string interpolation features with them.

Template literals are enclosed by the backtick (` `) (grave accent) character instead of double or single quotes.

Template literals can contain placeholders. These are indicated by the dollar sign and curly braces (`${expression}`). The expressions in the placeholders and the text between the backticks (` ``) get passed to a function.

Let's have a practice:

```JavaScript
const myName = "John";
const myAge = 25;
const birthYear = 1995;
const job = "teacher";

console.log(`My name is ${myName}. I am ${myAge} years old. I was born in ${birthYear}. I am a ${job}.`);
```

```{note}
1. You can use both single quotes and double quotes inside template literals.

2. You can use multi-line strings inside template literals.

3. You can use expressions inside template literals.

4. you can do any javascript code inside `${}`
```

let's have a practice:

```JavaScript
const myName = "John";
const birthYear = 1995;
const job = "teacher";
const now = 2023;

console.log(`My name is ${myName}. I am ${now - birthYear} years old. I was born in ${birthYear}. I am a ${job}.`);
```

as you can see in the above example, we can do any javascript code inside `${}`. so we did `now - birthYear` inside `${}`.

```{note}
you may use `...` as if you want to wtihe a long string in multiple lines. or instead of using single or double quotes.
```

for exmaple:

```JavaScript
console.log(`This is an example
which can be used to write without using single or double quotes`);
```

