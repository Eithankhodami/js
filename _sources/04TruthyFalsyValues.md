# Falsy Values
(04TruthyFalsyValues)=

Falsy values are values that evaluate to false when converted to a boolean.

there are 5 falsy values in JavaScript:

1. `NaN`
2. `0`
3. `""` (empty string)
4. `null`
5. `undefined`

```{tip}
to convert to a `boolean` you can use `Boolean()` function.
```

```js
    console.log(Boolean(NaN)); // false
    console.log(Boolean(0)); // false
    console.log(Boolean("")); // false
    console.log(Boolean(null)); // false
    console.log(Boolean(undefined)); // false
```

The rest of converstion will be `true` in conversion format.

```js
    console.log(Boolean(1)); // true
    console.log(Boolean("hello")); // true
    console.log(Boolean({})); // true
    console.log(Boolean([])); // true
```

```{tip}
In practice converting using such format is so rare!
```

