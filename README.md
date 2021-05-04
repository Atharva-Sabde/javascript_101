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

Comments in Javascript is same as  C++/Java : // and /* *

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

- 

    .trim() → removes the whitespaces from both the sides of a string

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

There were a lot of changes introduced in the ES6 version of JavaScript in 2015. One of the biggest changes was two new keywords,  `let` and `const`, to create, or*declare*, variables. Prior to the ES6, programmers could only use the `var` keyword to declare variables.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%201.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%201.png)

`var : It is the multipurpose variable in js` 

> var, short for variable, is a JavaScript keyword that creates, or declares, a new variable.

`let : The let keyword signals that the variable can be reassigned a different value.`

> we should be aware of when using let (and even var) is that we can declare a variable without assigning the variable a value. In such a case, the variable will be automatically initialized with a value of undefined

`const : This cannot change its value.`

> However, a const variable cannot be reassigned because it is constant. If you try to reassign a const variable, you’ll get a TypeError. 
Constant variables must be assigned a value when declared. If you try to declare a const variable without a value, you’ll get a SyntaxError

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
    - In ES6, template literals use backticks ``` and `${}` to interpolate values into a string.
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
<> if variable is filled → truthy  (true)
<>if variable is :
    - `0`
    - Empty strings like `""` or `''`
    - `null` which represent when there is no value at all
    - `undefined` which represent when a declared variable lacks a value
    - `NaN`, or Not a Number

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

## Functions:

> Function Declarations are scanned and made available.
Variable Declarations are scanned and made Undefined.

In JavaScript, there are many ways to create a function. One way to create a function is by using a function declaration. Just like how a variable declaration binds a value to a variable name, a function declaration binds a function to a name, or an identifier.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2014.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2014.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2015.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2015.png)

Default Parameters

One of the features added in ES6 is the ability to use *default parameters*. Default parameters allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is `undefined` when called.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2016.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2016.png)

Return

When a function is called, the computer will run through the function’s code and evaluate the result of calling the function. By default that resulting value is `undefined`.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2017.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2017.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2018.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2018.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2019.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2019.png)

Helper Functions

We can also use the return value of a function inside another function. These functions being called within another function are often referred to as *helper functions*. Since each function is carrying out a specific task, it makes our code easier to read and debug if necessary.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2020.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2020.png)

Function Expressions

Another way to define a function is to use a *function expression*. To define a function inside an expression, we can use the `function` keyword. In a function expression, the function name is usually omitted. A function with no name is called an *anonymous function*. A function expression is often stored in a variable in order to refer to it.

To declare a function expression:

1. Declare a variable to make the variable’s name be the name, or identifier, of your function. Since the release of ES6, it is common practice to use `const` as the keyword to declare the variable.
2. Assign as that variable’s value an anonymous function created by using the `function` keyword followed by a set of parentheses with possible parameters. Then a set of curly braces that contain the function body.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2021.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2021.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2022.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2022.png)

> Unlike function declarations, function expressions are not hoisted so they cannot be called before they are defined.

Advantages of function expressions??
As we’ve seen, function expressions don’t offer much that can’t be achieved with function declarations, but using them can often result in cleaner and more readable code. Their widespread use makes them an essential part of every developer’s toolbox.

Arrow Functions

ES6 introduced *arrow function syntax*, a shorter way to write functions by using the special “fat arrow” `() =>` notation.

Arrow functions remove the need to type out the keyword `function` every time you need to create a function. Instead, you first include the parameters inside the `( )` and then add an arrow `=>` that points to the function body surrounded in `{ }`

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2023.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2023.png)

Concise Body Arrow Functions

JavaScript also provides several ways to refactor arrow function syntax. The most condensed form of the function is known as *concise body*. We’ll explore a few of these techniques below:

 1.  Functions that take only a single parameter do not need that parameter to be enclosed in parentheses. However, if a function takes zero or multiple parameters, parentheses are required.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2024.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2024.png)

2.  A function body composed of a single-line block does not need curly braces. Without the curly braces, whatever that line evaluates will be automatically returned. The contents of the block should immediately follow the arrow => and the return keyword can be removed. This is referred to as implicit return.

- Functions SUmmarry:

    Review Functions

    Give yourself a pat on the back, you just navigated through functions!

    In this lesson, we covered some important concepts about functions:

    - A *function* is a reusable block of code that groups together a sequence of statements to perform a specific task.
    - A *function declaration* :

        ![https://content.codecademy.com/courses/learn-javascript-functions/Diagram/declaration.svg](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/declaration.svg)

    - A parameter is a named variable inside a function’s block which will be assigned the value of the argument passed in when the function is invoked:

        ![https://content.codecademy.com/courses/learn-javascript-functions/Diagram/function_parameters.svg](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/function_parameters.svg)

    - To *call* a function in your code:

        ![https://content.codecademy.com/courses/learn-javascript-functions/Diagram/name.svg](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/name.svg)

    - ES6 introduces new ways of handling arbitrary parameters through *default parameters* which allow us to assign a default value to a parameter in case no argument is passed into the function.
    - To return a value from a function, we use a *return statement*.
    - To define a function using *function expressions*:

        ![https://content.codecademy.com/courses/learn-javascript-functions/Diagram/expression.svg](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/expression.svg)

    - To define a function using *arrow function notation*:

        ![https://content.codecademy.com/courses/learn-javascript-functions/Diagram/arrow_notation.svg](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/arrow_notation.svg)

    - Function definition can be made concise using concise arrow notation:

        ![https://content.codecademy.com/courses/learn-javascript-functions/Diagram/return.svg](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/return.svg)

    It’s good to be aware of the differences between function expressions, arrow functions, and function declarations. As you program more in JavaScript, you’ll see a wide variety of how these function types are used.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2025.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2025.png)

## Scope:

Scope defines where variables can be accessed or referenced. While some variables can be accessed from anywhere within a program, other variables may only be available in a specific context.

Global Scope : In global scope, variables are declared outside of blocks. These variables are called global variables. Because global variables are not bound inside a block, they can be accessed by any code in the program, including code in blocks.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2026.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2026.png)

Block Scope : Variables that are declared w ith block scope are known as local variables because they are only available to the code that is part of the same block.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2027.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2027.png)

Scope Pollution  : Scope pollution is when we have too many global variables that exist in the global namespace, or when we reuse variables across different scopes. Scope pollution makes it difficult to keep track of our different variables and sets us up for potential accidents. For example, globally scoped variables can collide with other variables that are more locally scoped, causing unexpected behavior in our code.

- Tight Scoping :

    Tightly scoping your variables will greatly improve your code in several ways:

    - It will make your code more legible since the blocks will organize your code into discrete sections.
    - It makes your code more understandable since it clarifies which variables are associated with different parts of the program rather than having to keep track of them line after line!
    - It’s easier to maintain your code, since your code will be modular.
    - It will save memory in your code because it will cease to exist after the block finishes running.

        ![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2028.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2028.png)

- Scope Summarryyyy

    - **Scope** is the idea in programming that some variables are accessible/inaccessible from other parts of the program.
    - **Blocks** are statements that exist within curly braces `{}`.
    - **Global scope** refers to the context within which variables are accessible to every part of the program.
    - **Global variables** are variables that exist within global scope.
    - **Block scope** refers to the context within which variables that are accessible only within the block they are defined.
    - **Local variables** are variables that exist within block scope.
    - **Global namespace** is the space in our code that contains globally scoped information.
    - **Scope pollution** is when too many variables exist in a namespace or variable names are reused.

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2029.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2029.png)

---

## Arrays:

Arrays are JavaScript’s way of making lists. Arrays can store any data types (including strings, numbers, and booleans). Like lists, arrays are ordered, meaning each item has a numbered position.

//======================================================================================================

### Contexts:

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2030.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2030.png)

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2031.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2031.png)

```jsx
console.log(myName)
var myName = "cosmicdust"
// above code will print 'Undefined' because the variable is declared after the calling of that variable 
// the global context will know that a variable named myName exists in code below somewhere, but it will initialize 
// undefined

var myName = "cosmicdust"
console.log(myName)

// above code will print 'cosmicdust' because the variable is declared before its usage (calling), the global  context will
// know about it already and hence the value will be reflected.
```

Every JS program will have 2 stages of execution : 

1. Memory Creation Phase
    - All variables and functions will be identified.
    - Variables will be assigned as "undefined" & Functions will be copied as it is in memory.
2. Execution Phase
    - Execution will start line by line.
    - Variables will be assigned its value ( if defined) , and functions will be called ( in a whole new context of its own )

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2032.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2032.png)

Code :

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2033.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2033.png)

Memory Creation Phase

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2034.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2034.png)

Execution Phase

---

> As the phases of memory creation and execution continue, sometimes the program will go to much deeper levels of contexts inside contexts ( function inside function and so on...) . To handle this , Javascript engine manages it using a  `Stack` also called as Call stack .

- The Outermost Context is always the Global context ( parent , where the execution starts.

Call stack is known by many names like : Execution stack | Program Stack | Control stack | Runtime Stack | Machine Stack .

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2035.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2035.png)

Call Stack of any JS program

![Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2036.png](Codecademy%20ed7317c6b5ad496eb13396741fb4db19/Untitled%2036.png)