# Calling Functions

Let's create a function named `foodProcessor` in which we have:

```js
function foodProcessor (meat, veg) {
    const food = `processed food with ${meat} and ${veg} for today is ready!`;
    return food;
}
```

Now assume that our `foodProcessor` actually can get small piece of meat and veg and process them to a delicious food. So we can call it like this:
so we need to cut food and veg into small pieces.

```js

const cutterMachine = function (foodProcessor) {
    return foodProcessor *5;
}
```
Now that we have `cutterMachine` we can use it in our `foodProcessor`:

```js

const foodProcessor = function (meat, veg) {
    const meatPieces = cutterMachine(meat);
    const vegPieces = cutterMachine(veg);

    const food = `processed food with ${meatPieces} piece of meat and ${vegPieces} pieces of vegies for today is ready!`;
    return food;
}

```

```js 

console.log(foodProcessor(2, 3));

```
