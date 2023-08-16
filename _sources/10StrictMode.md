# What is Stric Mode?
(10-strict-mode)=

Strict mode is a way to introduce better error-checking into your code. When you use strict mode, you cannot, for example, use implicitly declared variables, or assign a value to a read-only property, or add a property to an object that is not extensible.

Strict mode is declared by adding "use strict"; to the beginning of a script or a function. Declared at the beginning of a script, it has global scope (all code in the script will execute in strict mode):

```js
"use strict";
x = 3.14;       // This will cause an error because x is not declared
```

Declared inside a function, it has local scope (only the code inside the function is in strict mode):

```js
x = 3.14;       // This will not cause an error.
myFunction();

function myFunction() {
  "use strict";
  y = 3.14;   // This will cause an error
}
```

## Why Strict Mode?

1- Strict mode makes it easier to write "secure" JavaScript.

2- Strict mode changes previously accepted "bad syntax" into real errors.

3- As an example, in normal JavaScript, mistyping a variable name creates a new global variable. In strict mode, this will throw an error, making it impossible to accidentally create a global variable.

4- In normal JavaScript, a developer will not receive any error feedback assigning values to non-writable properties.

```js
"use strict";
var obj = {};
Object.defineProperty(obj, "x", {value:0, writable:false});

obj.x = 3.14;            // This will cause an error
```

5- In strict mode, any assignment to a non-writable property, a getter-only property, a non-existing property, a non-existing variable, or a non-existing object, will throw an error.

6- Strict mode stops using predefined global variables. In normal JavaScript, a developer will not receive any error feedback assigning values to non-writable properties.

for example if you use `interface` as variable, without strict mode, it will not throw any error, but with strict mode, it will throw an error.

