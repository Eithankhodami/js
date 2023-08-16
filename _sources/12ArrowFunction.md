# Arrow Functions
(12-arrow-functions)=
We already learned about [Functions](11Functions.md) and now let's discuss Arrow function is a simple and concise way to write functions in ES6. It is also called 'Fat Arrow Functions' or 'Lambda Functions'.

```js
const calcAge = birthYear => 2037 - birthYear;

const age1 = calcAge(1991);
console.log(age1);
```

```js
const yearsUntilRetirement = (birthYear) => {
  const age = 2037 - birthYear;
  const retirement = 65 - age;
  // return retirement;
  return `retires in ${retirement} years`;
};

console.log(yearsUntilRetirement(1991));
```

```js
const yearsUntilRetirement = (birthYear, firstName) => {
  const age = 2037 - birthYear;
  const retirement = 65 - age;
  // return retirement;
  return `${firstName} retires in ${retirement} years`;
};

console.log(yearsUntilRetirement(1991, 'Jonas'));   // Jonas retires in 44 years

console.log(yearsUntilRetirement(1980, 'Bob'));     // Bob retires in 25 years
```
