# Errors understanding

In this section we discuss some errors in JavaScript we may face.

### Error1: 
`Uncaught SyntaxError: Unexpected token`

This error means that you have problem with coding syntax. For example, you may forget to close a bracket or a quote.

for example:
    
```javascript
        var myName = "John;
```
    
```{caution}
this is wrong. because we forget to close the quote.
    
```javascript
        var myName = "John";
```


### Error2:

`Uncaught ReferenceError: myName is not defined`

This error means that you have problem with variable declaration. For example, you may forget to declare a variable.

for example:
    
```javascript
        myName = "John";
```
    
```{caution}
this is wrong. because we forget to declare the variable.
    
```javascript
        var myName = "John";
```

### Error 3:
(constant-error)=
`Uncaught TypeError: Assignment of constant variable`

This error means that we have a `constant` varibale and we cannot change it. so we can say that `const` is **read-only** or **immutable**.

### Error 4:
(constant-initial-error)=

`Uncaught SyntaxError: Missing initializer in const declaration`

This error means that we have a `constant` varibale and we cannot create it without initial value. so we can say that `const` needs an initial value.
