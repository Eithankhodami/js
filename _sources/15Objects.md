# Objects

## What is an object?

An object is a collection of properties, and a property is an association between a name (or key) and a value. A property's value can be a function, in which case the property is known as a method. In addition to objects that are predefined in the browser, you can define your own objects.

## How to create an object?

There are two ways to create an object:

1. Using an object literal - `{}`

2. Using the `Object` constructor - `new Object()`

### Using an object literal

To create an object using an object literal, you simply list the properties within curly braces `{}`:

```js
const person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 30,
    hobbies: ['music', 'movies', 'sports'],
    address: {
        street: '50 main st',
        city: 'Boston',
        state: 'MA'
    }
}
```

The above object contains five properties and one method and is referred to as a five-property object. The properties are separated by commas.

The object properties have unique names:

- `firstName`
- `lastName`
- `age`
- `hobbies`
- `address`

## Using the `Object` constructor

To create an object using the `Object` constructor, you pass the object properties as arguments to the constructor:

```js
const person = new Object({
    firstName: 'John',
    lastName: 'Doe',
    age: 30,
    hobbies: ['music', 'movies', 'sports'],
    address: {
        street: '50 main st',
        city: 'Boston',
        state: 'MA'
    }
});
```

## How to access object properties?

You can access the object properties in two ways:

1. Dot notation - `objectName.propertyName`

2. Bracket notation - `objectName['propertyName']`

### Dot notation

To access the object properties using the dot notation, you simply put the dot `.` followed by the property name after the object name:

```js
const person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 30,
    hobbies: ['music', 'movies', 'sports'],
    address: {
        street: '50 main st',
        city: 'Boston',
        state: 'MA'
    }
}

console.log(person.firstName);
// Output: John

console.log(person.lastName); // Output: Doe

console.log(person.age); // Output: 30

console.log(person.hobbies); // Output: ['music', 'movies', 'sports']

console.log(person.address); // Output: { street: '50 main st', city: 'Boston', state: 'MA' }
```

### Bracket notation

calling an object using bracker notations is also possible.

to do, we use `objectName['propertyName']`

for example if we have following object:

```js
const person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 30,
    hobbies: ['music', 'movies', 'sports'],
    address: {
        street: '50 main st',
        city: 'Boston',
        state: 'MA'
    }
}
```
now lets call objects using bracket:

```js
console.log(person['firstName'])
```



