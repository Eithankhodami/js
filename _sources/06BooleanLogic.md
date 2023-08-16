# Boolean Logic

## What is Boolean Logic?

Boolean logic is a branch of computer science that deals with true and false values. It is named after George Boole, who first defined an algebraic system of logic in the mid 19th century. Boolean logic is especially important for computer science because it fits nicely with the binary numbering system, in which each bit has a value of either 0 or 1.

## Boolean Values

In JavaScript, there are two boolean values: `true` and `false`. They are used to represent the truth values of logic and Boolean algebra. The boolean values are often the result of a comparison operator.

## Logical Operators

Logical operators are used to combine boolean values. There are three logical operators in JavaScript:

1. (logical-and)=Logical AND (&&)
2. (logical-or)=Logical OR (||)
3. (logical-not)=Logical NOT (!)

```{tip}
Boolean Logic is not specific to JS, it is a general concept in programming.
```

To a better understand let's have a condition and see what we can get from it:

- A: Sara has a driver license
- B: Sara has a car

following these two statement of A, B we can have the following table:

| A     | B     | A AND B | A OR B | NOT A |
| ----- | ----- | ------- | ------ | ----- |
| false | false | false   | false  | true  |
| false | true  | false   | true   | true  |
| true  | false | false   | true   | false |
| true  | true  | true    | true   | false |

What does this mean?

- A AND B: both A and B should be true to get true
- A OR B: one of A or B should be true to get true
- NOT A: if A is true, then NOT A is false, and vice versa

Let's print some points:

Set A: Sara has a driver license(`True`) and has a car (`True`)
Set B: Sara has a driver license(`True`) and has no car (`False`)
Set C: Sara has no driver license(`False`) and has a car (`True`)
Set D: Sara has no driver license(`False`) and has no car (`False`)

let's print the results:

```javascript
console.log(true && true); // true
console.log(true && false); // false
console.log(false && true); // false
console.log(false && false); // false

console.log(true || true); // true
console.log(true || false); // true
console.log(false || true); // true
console.log(false || false); // false
```

```javascript

console.log(!true); // false
console.log(!false); // true
```

```{note}
`NOT` operator has precedence over `AND` and `OR` operators.
```

```javascript
console.log(!true && true); // false
console.log(!true || true); // true
```

```{note}
`AND` operator has precedence over `OR` operator.
```

```javascript
console.log(true && true || false); // true
console.log(true && (true || false)); // true
```
let's code example:

```javascript
const hasDriverLicense = true; //A
const hasCar = false; //B

console.log(hasDriverLicense && hasCar); // false
console.log(hasDriverLicense || hasCar); // true
console.log(!hasDriverLicense); // false
```

```{note}
`&&` and `||` are short-circuit operators, which means that if the first operand is enough to determine the result, the second operand is not evaluated.
```

Now let's create a new variable called `shouldDrive` and assign it to `hasDriverLicense && hasCar`:

```javascript
const shouldDrive = hasDriverLicense && hasCar;

if (shouldDrive) {
  console.log("Sara is able to drive");
} else {
  console.log("Someone else should drive");
}
```

now let's assume another condition:

- A: Sara has a driver license
- B: Sara has a car
- C: Sara doesn't have a bad vision

and we want to be sure sara has all conditions to drive:

```javascript
const hasDriverLicense = true; //A
const hasCar = true; //B
const hasBadVision = true; //C

if (hasDriverLicense && hasCar && !hasBadVision) {
  console.log("Sara is able to drive");
} else {
  console.log("Someone else should drive");
}
```

```{note}
Look how to add `!` Means `NOT` to `hasBadVision` to make it `false` and make the condition true.
```


### Practice:

Look at the table of following scores:

| Name  | Score1 | Score2 | Score3 | GPA   |
| ----- | ------ | ------ | ------ | ----- |
| Sara  | 14     | 12     | 19     | ?    |
| Ahmed | 14     | 10     | 9     | ?    |
| Ali   | 17     | 18     | 19     | ?    |

Task 1: calculate the GPA for each student and print it.

Task 2: print the name of the student who has the highest GPA and no score below 15.

Task 3: if GPA is over 12 and no score below 10, print "passed", otherwise print "failed".

Task 1:
```javascript
const saraScore1 = 14;
const saraScore2 = 12;
const saraScore3 = 19;

const ahmedScore1 = 14;
const ahmedScore2 = 10;
const ahmedScore3 = 9;

const aliScore1 = 17;
const aliScore2 = 18;
const aliScore3 = 19;

const saraGPA = (saraScore1 + saraScore2 + saraScore3) / 3;
const ahmedGPA = (ahmedScore1 + ahmedScore2 + ahmedScore3) / 3;
const aliGPA = (aliScore1 + aliScore2 + aliScore3) / 3;

console.log(saraGPA);
console.log(ahmedGPA);
console.log(aliGPA);
```

Task 2 Solution:

```javascript

if (saraGPA > ahmedGPA && saraGPA > aliGPA && saraScore1 > 15 && saraScore2 > 15 && saraScore3 > 15) {
  console.log("Sara");
} else if (ahmedGPA > saraGPA && ahmedGPA > aliGPA && ahmedScore1 > 15 && ahmedScore2 > 15 && ahmedScore3 > 15) {
  console.log("Ahmed");
} else if (aliGPA > saraGPA && aliGPA > ahmedGPA && aliScore1 > 15 && aliScore2 > 15 && aliScore3 > 15) {
  console.log("Ali");
} else {
  console.log("No one");
}
```

Task 3 Solution:

```javascript

if (saraGPA > 12 && saraScore1 > 10 && saraScore2 > 10 && saraScore3 > 10) {
  console.log("Sara passed");
} else {
  console.log("Sara failed");
}

if (ahmedGPA > 12 && ahmedScore1 > 10 && ahmedScore2 > 10 && ahmedScore3 > 10) {
  console.log("Ahmed passed");
} else {
  console.log("Ahmed failed");
}

if (aliGPA > 12 && aliScore1 > 10 && aliScore2 > 10 && aliScore3 > 10) {
  console.log("Ali passed");
} else {
  console.log("Ali failed");
}
```



