# Arrays

## What is an Array in JS

before understanding arrays, we need to know what is a Data Structure. 

A data structure is a particular way of organizing data in a computer so that it can be used effectively. For example, we can store a list of items having the same data-type using the array data structure.

By understanding data structures, you will learn how to write more efficient code and gain a deeper understanding of JavaScript.

An array is a special variable, which can hold more than one value at a time.

An array can hold many values under a single name, and you can access the values by referring to an index number.

An array can hold different types of values under a single name, and you can access the values by referring to an index number.

## How to create an Array

There are two ways to create an array in JavaScript:

1. Using an array literal - `[]`
2. Using the `Array` constructor - `new Array()`

### Using an array literal

To create an array using an array literal, you simply list the elements within square brackets `[]`:

```js
const fruits = ['Apple', 'Banana'];
```

The above array contains two elements and is referred to as a two-element array. The elements are separated by commas.

The array elements have unique indexes:

- The first element has the index `0`
- The second element has the index `1`

### Using the `Array` constructor

To create an array using the `Array` constructor, you pass the array elements as arguments to the constructor:

```js
const fruits = new Array('Apple', 'Banana');
```

The above array is created and assigned to the `fruits` variable.

## How to access Array Elements

to call an element in an array you can do this:

```js
const fruits = ['Apple', 'Banana'];

console.log(fruits[0]);
// Output: Apple
```

## amount of elements in an array

```js
const fruits = ['Apple', 'Banana'];

console.log(fruits.length);
// Output: 2
```

Now let's assume we have an array of some names:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];
```

so if we want to call the last element, either we should know how many elements are there. or we can use `length` property of an array:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];

console.log(names[names.length - 1]);
// Output: Sue
```

```{tip}
? Why we use `names.length - 1`?

The answer is that the index of an array starts from 0. so if we have 10 elements in an array, the last element will be in index 9. so we need to subtract 1 from the length of an array to get the last element.
```

## How to change an Array Element

To change an array element, you use the following syntax:

```js
array[index] = value;
```

Let's assume we have an array of some names:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];
```

and we want to change the name of `Sue` to `Susan`:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];

names[9] = 'Susan';

console.log(names);
// Output: ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Susan']
```

## How to add an Array Element

To add an element to the end of an array, you use the `push()` method:

```js
array.push(value);
```

Let's assume we have an array of some names:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];
```

and we want to add `Susan` to the end of the array:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];

names.push('Susan');

console.log(names);
// Output: ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue', 'Susan']
```


Now assume I am Eithan, I am 33 years old (Now), I have 2 friends [Jack and John] and I am a researcher, Now I can insert all these different data types into an array:

before doing this, I am 33 while now is 2023, what if it was 2024? I need to update my age, so I can do this:

```js
const eithan = ['Eithan', '33', 'researcher', ['Jack', 'John']];
```

or I can say:

```js
const eithan = ['Eithan', 2024-1989, 'researcher', ['Jack', 'John']];
```
again I can say:

```js
const friendsofEithan = ['Jack', 'John'];
const eithan = ['Eithan', 2024-1989, 'researcher', friendsofEithan];
console.log(eithan);
```

# How to remove an Array Element

To remove an element from the end of an array, you use the `pop()` method:

```js
array.pop();
```

Let's assume we have an array of some names:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];
```

and we want to remove the last element of the array:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda', 'Sue'];

names.pop();

console.log(names);
// Output: ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda']
```
# Add an element to the beginning of an Array

To add an element to the beginning of an array, you use the `unshift()` method:

```js
array.unshift(value);
```

Let's assume we have an array of some names:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda'];
```

and we want to add `Sue` to the beginning of the array:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda'];

names.unshift('Sue');

console.log(names);
// Output: ['Sue', 'John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda']
```
we also can remove the first element of an array using `shift()` method:

```js
const names = ['Sue', 'John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda'];

names.shift();

console.log(names);
// Output: ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda']
```

# How to find the index of an Array Element

To find the index of an array element, you use the `indexOf()` method:

```js
array.indexOf(value);
```

Let's assume we have an array of some names; and we want to find the index of `Sara`:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda'];

console.log(names.indexOf('Sara'));

// Output: 3
```

# `includes()` method

The `includes()` method determines whether an array includes a certain value among its entries, returning `true` or `false` as appropriate.

```js
array.includes(value);
```

Let's assume we have an array of some names; and we want to find if `Sara` is in the array:

```js
const names = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike', 'Tom', 'Jack', 'Linda'];

console.log(names.includes('Sara'));

// Output: true
```



Let's have a little more fun with array and [functions](11Functions.md).

assume we have 6 friends.

```js
const friends = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike'];
```
now we want to check if I have a friend named `Sara` or not, we can do this:

```js
const friends = ['John', 'Roy', 'Mick', 'Sara', 'Jennifer', 'Mike'];

const checkFriend = function (name) {
    if (friends.includes(name)) {
        console.log(`Yes, ${name} is my friend.`);
    } else {
        console.log(`No, ${name} is not my friend.`);
    }
}

checkFriend('Sara');
checkFriend('Eithan');
```
