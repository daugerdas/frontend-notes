- Introduction
- Variables 
- Data types
- Type conversions
- Data structures
- Operators
- Loops
- Control flow
- Functions
- Asynchronous JavaScript
- Working with APIs (fetch)
- Classes
- Modules
- Memory
- Strict mode
- DOM
- Dev Tools

## Introduction
JavaScript is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions. JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles. The standards for JavaScript are the ECMAScript Language Specification (ECMA-262) and the ECMAScript Internationalization API specification (ECMA-402).

JavaScript can execute not only in the browser, but also on the server, or actually on any device that has a special program called the JavaScript engine.The browser has an embedded engine sometimes called a “JavaScript virtual machine”. Different engines have different “codenames”. For example: V8 – in Chrome, Opera and Edge, SpiderMonkey – in Firefox, there are other codenames like “Chakra” for IE, “JavaScriptCore”, “Nitro” and “SquirrelFish” for Safari, etc.

#### Just-in-time
In computing, just-in-time (JIT) compilation (also dynamic translation or run-time compilations) is a way of executing computer code that involves compilation during execution of a program (at run time) rather than before execution.

#### First-class functions
A programming language is said to have First-class functions when functions in that language are treated like any other variable.

#### Prototype-based programming

Prototype-based programming is a style of object-oriented programming in which classes are not explicitly defined, but rather derived by adding properties and methods to an instance of another class or, less frequently, adding them to an empty object.
In simple words: this type of style allows the creation of an object without first defining its class.

#### Dynamic typing
Dynamically-typed languages are those (like JavaScript) where the interpreter assigns variables a type at runtime based on the variable's value at the time.

#### Imperative programming
In computer science, imperative programming is a programming paradigm of software that uses statements that change a program's state.

#### Object-oriented programming
Object-oriented programming is a programming paradigm based on the concept of "objects", which can contain data and code. The data is in the form of fields (often known as attributes or properties), and the code is in the form of procedures (often known as methods).

#### Declarative programming
In computer science, declarative programming is a programming paradigm—a style of building the structure and elements of computer programs—that expresses the logic of a computation without describing its control flow.

#### Functional programming
In computer science, functional programming is a programming paradigm where programs are constructed by applying and composing functions. 

### Languages transpiled to JavaScript
Recently a plethora of new languages appeared, which are transpiled (converted) to JavaScript before they run in the browser.
Examples of such languages:
- CoffeeScript is “syntactic sugar” for JavaScript. It introduces shorter syntax, allowing us to write clearer and more precise code. Usually, Ruby devs like it.
- TypeScript is concentrated on adding “strict data typing” to simplify the development and support of complex systems. It is developed by Microsoft.
- Flow also adds data typing, but in a different way. Developed by Facebook.
- Dart is a standalone language that has its own engine that runs in non-browser environments (like mobile apps), but also can be transpiled to JavaScript. Developed by Google.
- Brython is a Python transpiler to JavaScript that enables the writing of applications in pure Python without JavaScript.
- Kotlin is a modern, concise and safe programming language that can target the browser or Node.

## Variables
The names of variables, called identifiers, conform to certain rules. This syntax can be used to declare both local and global variables, depending on the execution context.

#### var
Declares a variable, optionally initializing it to a value.

#### let
Declares a block-scoped, local variable, optionally initializing it to a value.

#### const
Declares a block-scoped, read-only named constant.


### Hoisting
JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.

var-declared variables are hoisted, meaning you can refer to the variable anywhere in its scope, even if its declaration isn't reached yet. You can see var declarations as being "lifted" to the top of its function or global scope. However, if you access a variable before it's declared, the value is always undefined, because only its declaration is hoisted, but not its initialization.

Whether let and const are hoisted is a matter of definition debate. Referencing the variable in the block before the variable declaration always results in a ReferenceError, because the variable is in a "temporal dead zone" from the start of the block until the declaration is processed.

Unlike var declarations, which only hoist the declaration but not its value, function declarations are hoisted entirely — you can safely call the function anywhere in its scope.

In colloquial terms, any of the following behaviors may be regarded as hoisting:

- Being able to use a variable's value in its scope before the line it is declared. ("Value hoisting")
- Being able to reference a variable in its scope before the line it is declared, without throwing a ReferenceError, but the value is always undefined. ("Declaration hoisting")
- The declaration of the variable causes behavior changes in its scope before the line in which it is declared (let, const, class).

### Variable scope 
A variable may belong to one of the following scopes:

- Global scope: The default scope for all code running in script mode.
- Module scope: The scope for code running in module mode.
- Function scope: The scope created with a function.
In addition, variables declared with let or const can belong to an additional scope:
- Block scope: The scope created with a pair of curly braces (a block).

## Data types
- Objects
  - Prototypal inheritance 
  - Object prototype

## Data structures
- Arrays
