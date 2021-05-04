# javascript_101

## These are my Notes for Learning vanilla JS. The data is collected from multiple sources and compiled to form a content-rich document.

<hr>
<hr>

# Codecademy

[Projects:](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Projects%203936c3ed79fd4387aeb019ed4b5859d2.md)

Console

The console is a panel that displays important messages, like errors, for developers. Much of the work the computer does with our code is invisible to us by default. If we want to see things appear on our screen, we can print, or *log*, to our console directly.

In JavaScript, the `console` keyword refers to an object, a collection of data and actions, that we can use in our code. One method, that is built into the console object is the .log() method. When we write console.log() what we put inside the parentheses will get printed, or logged, to the console.

> When we use console.log() we’re calling the .log() method on the console object. Let’s see console.log() and some real string methods in action!

Comments in Javascript is same as C++/Java : // and /\* \*

Data Types:

Number , String , Boolean , Null , Undefined , Symbol , Object

Operators:

1. Add: `+`
2. Subtract: ``
3. Multiply: ``
4. Divide: `/`
5. Remainder: `%`

String Concatenation

Operators aren’t just for numbers! When a `+` operator is used on two strings, it appends the right string to the left string:

Properties

When you introduce a new piece of data into a JavaScript program, the browser saves it as an instance of the data type. Every string instance has a property called `length` that stores the number of characters in that string. You can retrieve property information by appending the string with a period and the property name:

The . is another operator! We call it the dot operator.

---

Methods

- .trim() → removes the whitespaces from both the sides of a string

  [Untitled](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%20Database%2023b0d459971d44e4be2927b4713a3dea.csv)

Remember that methods are actions we can perform. JavaScript provides a number of string methods.

We *call*, or use, these methods by appending an instance with:

- a period (the dot operator)
- the name of the method
- opening and closing parentheses

---

Built-in Objects

In addition to `console`, there are other [objects built into JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects). Down the line, you’ll build your own objects, but for now these “built-in” objects are full of useful functionality.

---

## Variables:

Difference between var ||| let ||| const :

[https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled.png)

There were a lot of changes introduced in the ES6 version of JavaScript in 2015. One of the biggest changes was two new keywords, `let` and `const`, to create, or*declare*, variables. Prior to the ES6, programmers could only use the `var` keyword to declare variables.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%201.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%201.png)

`var : It is the multipurpose variable in js`

> var, short for variable, is a JavaScript keyword that creates, or declares, a new variable.

`let : The let keyword signals that the variable can be reassigned a different value.`

> we should be aware of when using let (and even var) is that we can declare a variable without assigning the variable a value. In such a case, the variable will be automatically initialized with a value of undefined

`const : This cannot change its value.`

> However, a const variable cannot be reassigned because it is constant. If you try to reassign a const variable, you’ll get a TypeError.
> Constant variables must be assigned a value when declared. If you try to declare a const variable without a value, you’ll get a SyntaxError

### Mathematical Assignment Operators

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%202.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%202.png)

### The Increment and Decrement Operator

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%203.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%203.png)

### String Concatenation with Variables

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%204.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%204.png)

### String Interpolation

In the ES6 version of JavaScript, we can insert, or interpolate, variables into strings using template literals. One of the biggest benefits to using template literals is the readability of the code.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%205.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%205.png)

### typeof operator

The typeof operator checks the value to its right and returns, or passes back, a string of the data type.

-

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%206.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%206.png)

- Variables SUMMARY
  - Variables hold reusable data in a program and associate it with a name.
  - Variables are stored in memory.
  - The `var` keyword is used in pre-ES6 versions of JS.
  - `let` is the preferred way to declare a variable when it can be reassigned, and `const` is the preferred way to declare a variable with a constant value.
  - Variables that have not been initialized store the primitive data type `undefined`.
  - Mathematical assignment operators make it easy to calculate a new value and assign it to the same variable.
  - The `+` operator is used to concatenate strings including string values held in variables
  - In ES6, template literals use backticks ``` and `${}` to interpolate values into a string.
  - The `typeof` keyword returns the data type (as a string) of a value.

---

## Conditional Statements:

- `if`, `else if`, and `else` statements

---

- comparison operators

  - Less than: `<`
  - Greater than: `>`
  - Less than or equal to: `<=`
  - Greater than or equal to: `>=`
  - Is equal to: `===` ( also compares the data type)
  - Is not equal to: `!==`
  - Compare but without its type `==`

    ![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%207.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%207.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%208.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%208.png)

```jsx
null === undefined ->  false
null == undefined  ->  true
null == NaN    -> false

```

---

- logical operators
  - the *and* operator (`&&`)
  - the *or* operator (`||`) If the first condition in an || statement evaluates to true, the second condition won’t even be checked
  - the *not* operator, otherwise known as the *bang* operator (`!`)

---

- truthy vs falsy values
  Sometimes, you’ll want to check if a variable exists and you won’t necessarily want it to equal a specific value — you’ll only check to see if the variable has been assigned a value.
  <> if variable is filled → truthy (true)
  <>if variable is : - `0` - Empty strings like `""` or `''` - `null` which represent when there is no value at all - `undefined` which represent when a declared variable lacks a value - `NaN`, or Not a Number

      Then it is → falsy (false)

      ![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%209.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%209.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2010.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2010.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2011.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2011.png)

---

- ternary operators
  - The condition, `isNightTime`, is provided before the `?`.
  - Two expressions follow the `?` and are separated by a colon `:`.
  - If the condition evaluates to `true`, the first expression executes.
  - If the condition evaluates to `false`, the second expression executes.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2012.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2012.png)

---

- `switch` statement
  A switch statement provides an alternative syntax that is easier to read and write.

- Conditionsl Statements SUmmary

  **CONDITIONAL STATEMENTS**

  Review

  Way to go! Here are some of the major concepts for conditionals:

  - An `if` statement checks a condition and will execute a task if that condition evaluates to `true`.
  - `if...else` statements make binary decisions and execute different code blocks based on a provided condition.
  - We can add more conditions using `else if` statements.
  - Comparison operators, including `<`, `>`, `<=`, `>=`, `===`, and `!==` can compare two values.
  - The logical and operator, `&&`, or “and”, checks if both provided expressions are truthy.
  - The logical operator `||`, or “or”, checks if either provided expression is truthy.
  - The bang operator, `!`, switches the truthiness and falsiness of a value.
  - The ternary operator is shorthand to simplify concise `if...else` statements.
  - A `switch` statement can be used to simplify the process of writing multiple `else if` statements. The `break` keyword stops the remaining `case`s from being checked and executed in a `switch` statement.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2013.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2013.png)

---

---
