# Hoisting

Hoisting is a JavaScript mechanism where variable and function declarations are moved to the top of their scope before code execution.

---

## Variable Hoisting in JavaScript

### var Hoisting
Variables declared with `var` are hoisted and initialized with `undefined`:

```javascript
console.log(x); // undefined
var x = 5;
console.log(x); // 5
```

Equivalent to:
```javascript
var x;
console.log(x); // undefined
x = 5;
console.log(x); // 5
```

---

### let and const Hoisting
Variables declared with `let` and `const` are hoisted but not initialized (Temporal Dead Zone):

```javascript
console.log(x); // ReferenceError: Cannot access 'x' before initialization
let x = 5;
```

---

## Function Hoisting

### Function Declarations
Function declarations are fully hoisted:

```javascript
greet(); // "Hello!"

function greet() {
    console.log("Hello!");
}
```

### Function Expressions
Function expressions are not hoisted:

```javascript
greet(); // TypeError: greet is not a function

var greet = function() {
    console.log("Hello!");
};
```

---

## Hoisting in Kotlin

Kotlin doesn't have hoisting like JavaScript. Variables and functions must be declared before use:

```kotlin
// This won't compile
println(x) // Error: Unresolved reference: x
val x = 5
```

```kotlin
// Correct order
val x = 5
println(x) // 5
```

---

## Best Practices

1. **Declare variables at the top** of their scope
2. **Use `let` and `const`** instead of `var` in JavaScript
3. **Declare functions before use** for clarity
4. **Understand scope** to avoid unexpected behavior

---

## Key Differences

| Language | Hoisting Behavior |
|----------|------------------|
| JavaScript (var) | Variables hoisted and initialized to undefined |
| JavaScript (let/const) | Variables hoisted but in Temporal Dead Zone |
| JavaScript (functions) | Function declarations fully hoisted |
| Kotlin | No hoisting - declarations must come before use |
