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
The latest ECMAScript standard defines eight data types.  JavaScript is also a weakly typed language, which means it allows implicit type conversion when an operation involves mismatched types, instead of throwing type errors.

All types except Object define immutable values represented directly at the lowest level of the language. We refer to values of these types as primitive values. All primitive types, except null and undefined, have their corresponding object wrapper types, which provide useful methods for working with the primitive values. Seven data types that are primitives.
- Boolean. true and false.
- null. A special keyword denoting a null value.
- undefined. A top-level property whose value is not defined.
- Number. An integer or floating point number. For example: 42 or 3.14159.
- BigInt. An integer with arbitrary precision. For example: 9007199254740992n.
- String. A sequence of characters that represent a text value.
- Symbol. A data type whose instances are unique and immutable.

And non-primitive - Object.

### Boolean 
Boolean is a logical data type that can have only the values true or false. The Boolean value is named after English mathematician George Boole, who pioneered the field of mathematical logic.

### null
In computer science, a null value represents a reference that points, generally intentionally, to a nonexistent or invalid object or address. In JavaScript, null is marked as one of the primitive values, because its behavior is seemingly primitive. However, when using the typeof operator, it returns "object".

### undefined
undefined is a primitive value automatically assigned to variables that have just been declared, or to formal arguments for which there are no actual arguments. Conceptually, undefined indicates the absence of a value, while null indicates the absence of an object (which could also make up an excuse for typeof null === "object"). The language usually defaults to undefined when something is devoid of a value:
- A return statement with no value (return;) implicitly returns undefined.
- Accessing a nonexistent object property (obj.iDontExist) returns undefined.
- A variable declaration without initialization (let x;) implicitly initializes the variable to undefined.
- Many methods, such as Array.prototype.find() and Map.prototype.get(), return undefined when no element is found.

### Number
In JavaScript, Number is a numeric data type in the double-precision 64-bit floating point format (IEEE 754).

NaN ("Not a Number") is a special kind of number value that's typically encountered when the result of an arithmetic operation cannot be expressed as a number. It is also the only value in JavaScript that is not equal to itself. 

It is capable of storing positive floating-point numbers between 2<sup>-1074</sup> (Number.MIN_VALUE) and 2<sup>1024</sup> (Number.MAX_VALUE) as well as negative floating-point numbers between -2<sup>-1074</sup> and -2<sup>1024</sup>, but it can only safely store integers in the range -(2<sup>53</sup> − 1) (Number.MIN_SAFE_INTEGER) to 2<sup>53</sup> − 1 (Number.MAX_SAFE_INTEGER). Outside this range, JavaScript can no longer safely represent integers; they will instead be represented by a double-precision floating point approximation. You can check if a number is within the range of safe integers using Number.isSafeInteger().

Values outside the range ±(2<sup>-1074</sup> to 2<sup>1024</sup>) are automatically converted:
- Positive values greater than Number.MAX_VALUE are converted to +Infinity.
- Positive values smaller than Number.MIN_VALUE are converted to +0.
- Negative values smaller than -Number.MAX_VALUE are converted to -Infinity.
- Negative values greater than -Number.MIN_VALUE are converted to -0.

### BigInt
In JavaScript, BigInt is a numeric data type that can represent integers in the arbitrary precision format. With BigInts, you can safely store and operate on large integers even beyond the safe integer limit (Number.MAX_SAFE_INTEGER) for Numbers. A BigInt is created by appending n to the end of an integer or by calling the BigInt() function.

### String
In any computer programming language, a string is a sequence of characters used to represent text. In JavaScript, a String is one of the primitive values and the String object is a wrapper around a String primitive. The String type represents textual data and is encoded as a sequence of 16-bit unsigned integer values representing UTF-16 code units. Each element in the string occupies a position in the string. The first element is at index 0, the next at index 1, and so on. The length of a string is the number of UTF-16 code units in it, which may not correspond to the actual number of Unicode characters.

JavaScript strings are immutable. This means that once a string is created, it is not possible to modify it. String methods create new strings based on the content of the current string — for example:
- A substring of the original using substring().
- A concatenation of two strings using the concatenation operator (+) or concat().

### Symbol 
Symbol is a built-in object whose constructor returns a symbol primitive — also called a Symbol value or just a Symbol — that's guaranteed to be unique. A Symbol is a unique and immutable primitive value and may be used as the key of an Object property.

### Object
In JavaScript, objects can be seen as a collection of properties. With the object literal syntax, a limited set of properties are initialized; then properties can be added and removed. Property values can be values of any type, including other objects, which enables building complex data structures. Properties are identified using key values. A key value is either a String value or a Symbol value. In computer science, an object is a value in memory which is possibly referenced by an identifier. In JavaScript, objects are the only mutable values. Functions are, in fact, also objects with the additional capability of being callable. There are two types of object properties: The data property and the accessor property. Each property has corresponding attributes.

### Other data structures

#### Dates
When representing dates, the best choice is to use the built-in Date utility in JavaScript.

#### Indexed collections: Arrays and typed Arrays
Arrays are regular objects for which there is a particular relationship between integer-keyed properties and the length property. Additionally, arrays inherit from Array.prototype, which provides a handful of convenient methods to manipulate arrays. For example, indexOf() searches a value in the array and push() appends an element to the array. This makes Arrays a perfect candidate to represent ordered lists.

#### Keyed collections: Maps, Sets, WeakMaps, WeakSets
These data structures take object references as keys. Set and WeakSet represent a collection of unique values, while Map and WeakMap represent a collection of key-value associations.

#### Structured data: JSON
JSON (JavaScript Object Notation) is a lightweight data-interchange format, derived from JavaScript, but used by many programming languages. JSON builds universal data structures that can be transferred between different environments and even across languages.


