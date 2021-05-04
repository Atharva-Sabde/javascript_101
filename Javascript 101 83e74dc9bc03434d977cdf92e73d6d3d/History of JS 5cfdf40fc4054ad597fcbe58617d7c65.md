# History of JS:

### ECMA script:   (europian computer manufacturing association)

When scripting languages were new, and many , all browsers struggled to keep the compatibility with all these languages.
so ECMA decided to make some standards

They made a common guidelines for scripting languages , and Now many languages including JS folows all those guidelines with some other languages too..

ES6  → 2015     [ECMAScript 6 was the second major revision to JavaScript.] [Functional programming concept was introduced in ES6]

ES7 → 2016

.

.

ES10 

### Compatibility Table : [https://kangax.github.io/compat-table/es6/](https://kangax.github.io/compat-table/es6/)

### ES6 References :

[https://codeburst.io/es6-tutorial-for-beginners-5f3c4e7960be](https://codeburst.io/es6-tutorial-for-beginners-5f3c4e7960be)

[https://javascript.plainenglish.io/9-es6-features-every-javascript-developer-should-know-b1f2915e7add](https://javascript.plainenglish.io/9-es6-features-every-javascript-developer-should-know-b1f2915e7add)

[https://www.youtube.com/watch?v=YbXjFoFceag](https://www.youtube.com/watch?v=YbXjFoFceag)

---

![History%20of%20JS%205cfdf40fc4054ad597fcbe58617d7c65/Untitled.png](History%20of%20JS%205cfdf40fc4054ad597fcbe58617d7c65/Untitled.png)

# **[Javascript ES6: Learn important features in a few minutes](https://frontendjournal.com/javascript-es6-learn-important-features-in-a-few-minutes/)**

[SEPTEMBER 10, 2020](https://frontendjournal.com/javascript-es6-learn-important-features-in-a-few-minutes/) / [ELEANOR MARSHALL](https://frontendjournal.com/author/blogadmin/)

The next-generation of javascript also known as ECMAScript 6 (also called ES6 or Harmony), is bringing us lots of amazing features that you probably will need to know. But instead of you spend too much time learning and researching all of the features I separated a few that I felt are the ones you’ll be probably using in your daily basis.

Don’t worry if you are new to javascript or you’re coming from a server-side language, I believe this is the best time to learn it as ES6 has a much cleaner and friendlier syntax, known as `sugar syntax`.

### Sugar Syntax

First of all, Syntactic Sugar is a syntax that make a language easier to understand and more readable, it makes the language “sweeter” for us. It also means that some “new” features of ES6 are not really new because ES6 is trying to simplify the syntax to make things easier for us. So instead of writing the your code using the old tricky way, you’ll be able to code in a the simpler way, with sugar syntax.

Look below the sugar syntax in action to create a class in Javascript.

### Classes

![History%20of%20JS%205cfdf40fc4054ad597fcbe58617d7c65/Untitled%201.png](History%20of%20JS%205cfdf40fc4054ad597fcbe58617d7c65/Untitled%201.png)

Always remember: Javascript does not support classes like other Object-Oriented languages. Instead, Javascript can simulate classes using `functions` and `prototype`.

Below is the new syntax to create classes. You will feel familiar to this way if you come from a Java background or other OO language.

```
class Project {
  constructor(name) {
    this.name = name;
  }

  start() {
    return "Project " + this.name + " starting";
  }
}

var project = new Project("Journal");
project.start(); // "Project Journal starting"

```

All the methods you declare in a class will be added to the prototype of the class.

### 

[]()

### Inheritance in ES6 and Prototype:

As said before, javascript does not support classes. So, if it doesn’t support classes, does it support inheritance?

Yes, inheritance in javascript is possible via `prototype`. If you’re not familiar with prototype, the good news is that with ES6 you don’t necessarily need to know it to get the benefits of classes and inheritance. `prototype` is not hard to learn but for the purpose of this post you can understand `prototype` as the way javascript implements inheritance.

This is how I would create a subclass of Project, called WebProject and inherit the attributes and methods from Project.

```
class WebProject extends Project {
  constructor(name, technologies) {
    super(name);
    this.technologies = technologies;
  }

  info() {
    return this.name + " uses " + arrayToString(this.technology);
  }
}

function arrayToString(param) {
  // ... some implementation
}

var webJournal = new WebProject("FrontEnd Journal", "javascript");
webJournal.start(); // "FrontEnd Journal starting"
webJournal.info(); // "FrontEnd Journal uses javascript"

```

Notice that in my WebProject constructor, I invoke the Project constructor and then I can make use of its attributes and method.

### Modules

If you don’t want to leave all of your javascript in just one file or you do want to re-use some functionality in other parts of your application, you’ll probably want to use modules. The magic keyword you need remember is `export`. Use export before the function you want to expose and you’re done.

This is the structure of our app. The Project and the WebProject classes are stored in `application.js`.

```
myproject (folder)
 |
 -- modules (folder)
 |   |
 |   -- helpers.js
 |
 -- application.js

```

Let’s separate out the `arrayToString()` function from the `application.js` and put it into the module `modules/helpers.js`, so we can re-use it in other places.

```
// modules/helper.js
export function arrayToString(param) {
  // some implementation
}

```

Now we just need to import our module in `application.js`:

```
// application.js
import { arrayToString } from 'modules/helpers';

class WebProject extends Project {
  constructor(name, technologies) {
    super(name);
    this.technologies = technology;
  }

  info() {
    return this.name + " uses " + arrayToString(this.technology);
  }
}

// ...

```

### What else should I know about ES6?

Well, the next two feature in ES6 are very interesting. Enter `let` and `const`. They will make the development easier and even avoid common mistakes in Javascript.

### let

To understand `let`, first we need to keep in mind that `var` creates function-scoped variables:

```
function printName() {
  if(true) {
    var name = "Rafael";
  }
  console.log(name); // Rafael
}

```

Notice that, unlike Java or many other languages, any variable created inside a function in Javascript it is hoisted to the top of the function. It means no matter where you declare the variable, it’s the same as if you declare it at the top of the function. This behaviour is called `hoisting`.

So the function above can be better understood like this:

```
function printName() {
  var name; // variable declaration is hoisted to the top
  if(true) {
    name = "Rafael";
  }
  console.log(name); // Rafael
}

```

Now, how does `let` work?Let’s modify the same example and introduce let in it.

```
function printName() {
  if(true) {
    let name = "Rafael";
  }
  console.log(name); // ReferenceError: name is not defined
}

```

As `let` is inside a block, name is only seen inside that block.

```
function printName() {
  var name = "Hey";
  if(true) {
    let name = "Rafael";
    console.log(name); // Rafael
  }
  console.log(name); // Hey
}

```

In this case, as `let` is referencing a previously declared variable, the value “Rafael” is valid only inside the block. Outside the block the value of `name` is “Hey”.

In summary, `var` is function-scoped and `let` is block-scoped.

### const

The ability to create constant variables is something javascript was missing for a long time. With ES6 you’ll be able to create constants and make sure its value won’t be changed during the application execution.

The syntax for creating constants is as follow:

```
const SERVER_URL = ""

```

### Other interesting features

ECMAScript 6 also brings these amazing features you might want to take a look: `Map`, `WeakMap`, `generators` and `Proxies`.

### When will I be able to use ES6?

At the moment Firefox is the browser that has implemented more features. Juriy Zaytsev has put together some a useful table of compatibility for the major browsers. [http://kangax.github.com/es5-compat-table/es6/](http://web.archive.org/web/20181127080747/http://kangax.github.com/es5-compat-table/es6/)

Some ES6 features is also available in Node JS. Check out Alex Young’s blog post on [ES6 for Node](http://web.archive.org/web/20181127080747/http://dailyjs.com/2012/10/15/preparing-for-esnext/) to get started.

### Conclusion

The next-generation of javascript will bring a simpler and friendlier syntax helping the learning process for developers coming from other OO languages. The main problem I see now is that it’s gonna take some time until we can use ES6 extensively in all major browsers.

Now, for server side development using Nodejs, ES6 is already a reality as many features are already present in V8.