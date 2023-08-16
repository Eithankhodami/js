# Equality Operators

## What is Equality Operators?

The equality operators are used to compare two values and return a boolean value (true or false).

## Types of Equality Operators

There are two types of equality operators:

1. Strict equality operator (===)
2. Abstract equality operator (==)

## Strict Equality Operator (===)

The strict equality operator (===) compares two values for equality. If the two values are of different types, the result is false. If the two values are of the same type and have the same value, the result is true.

### Example

```javascript
console.log(5 === 5); // true
console.log(5 === "5"); // false
```

## Abstract Equality Operator (==)

The abstract equality operator (==) compares two values for equality. Unlike the strict equality operator, the abstract equality operator attempts to convert the values being compared to a common type. If the values are of the same type, then the abstract equality operator behaves exactly like the strict equality operator. If the values are of different types, then the abstract equality operator applies a set of rules to convert one of the values to the other type. The abstract equality operator then compares the converted values. If the converted values are equal, then the abstract equality operator returns true. If the converted values are not equal, then the abstract equality operator returns false.

### Example

```javascript
console.log(5 == 5); // true
console.log(5 == "5"); // true
```

```{note}
**STRONGLY** suggest to use `===` instead of `==`.
```

we also have `!=` and `!==` which are **NOT equal**  operators.

```javascript
console.log(5 != 5); // false
console.log(5 != "5"); // false

console.log(5 !== 5); // false
console.log(5 !== "5"); // true
```

This means that in the first and second, becayse the values are equal, so the result is false. But in the third one, the values are equal but the types are different, so the result is true.
