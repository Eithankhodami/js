# Switch Statement

## 1. Switch Statement

The switch statement is used to perform different actions based on different conditions.

For example, let's say we want to print a message based on the day of the week. We can use the switch statement to do that.

```javascript
const day = "Monday";

switch (day) {
  case "Monday":
    console.log("Today is Monday");
    break;
  case "Tuesday":
    console.log("Today is Tuesday");
    break;
  case "Wednesday":
    console.log("Today is Wednesday");
    break;
  case "Thursday":
    console.log("Today is Thursday");
    break;
  case "Friday":
    console.log("Today is Friday");
    break;
  case "Saturday":
    console.log("Today is Saturday");
    break;
  case "Sunday":
    console.log("Today is Sunday");
    break;
  default:
    console.log("Invalid day");
}
```
```{note}
- The switch statement starts with the `switch` keyword followed by the expression to evaluate and a pair of curly braces.
- Inside the curly braces, we have a list of `case` statements.
- The `case` statement is followed by a value and a colon.
- If the value matches the expression, the statements inside the `case` statement will be executed.
- If the value does not match the expression, the statements inside the `case` statement will not be executed.
- The `break` keyword is used to terminate the `case` statement.
- The `default` statement is used to specify the code to run if there is no match.
```

```{tip}
you can have more than one `case` statement for the same value.
```

```javascript
const day = "Monday";

switch (day) {
  case "Monday":
  case "Tuesday":
  case "Wednesday":
  case "Thursday":
  case "Friday":
    console.log("It's a weekday");
    break;
  case "Saturday":
  case "Sunday":
    console.log("It's a weekend");
    break;
  default:
    console.log("Invalid day");
}
```
```
