# JavaScript Crash

JavaScript is a cross-platform, object-oriented scripting language used to make webpages interactive (e.g. having complex animations, clickable buttons, popup menus, etc.). There are also more advanced server side versions of JavaScript such as Node.Js which allow you to add more functionality to a website than simply downloading files (such as realtime collaboration between multiple computers). Inside a host environment (for example, a web browser), JavaScript can be connected to the objects of its environment to provide programmatic control over them.

JavaScript contains a standard library of objects, such as Array, Date, and Math, and a core set of language elements such as operators, control structures, and statements. Core JavaScript can be extended for a variety of purposes by supplementing it with additional objects; for example:

- Client-side JavaScript extends the core language by supplying objects to control a browser and its Document Object Model (DOM). For example, client-side extensions allow an application to place elements on an HTML form and respond to user events such as mouse clicks, form input, and page navigation.
- Server-side JavaScript extends the core language by supplying objects relevant to running JavaScript on a server. For example, server-side extensions allow an application to communicate with a database, provide continuity of information from one invocation to another of the application, or perform file manipulations on a server.

This means that in the browser, JavaScript can change the way the webpage (DOM) looks. And, likewise, Node.js JavaScript on the server can respond to custom requests from code written in the browser.

## Variables

- You use variables as symbolic names for values in your application. The names of variables, called identifiers, conform to certain rules.A JavaScript identifier must start with a letter, underscore (\_), or dollar sign (\$); subsequent characters can also be digits (0-9). Because JavaScript is case sensitive, letters include the characters "A" through "Z" (uppercase) and the characters "a" through "z" (lowercase).

### Variable declarations

- **var** - Declares a variable, optionally initializing it to a value.
- **let** - Declares a block-scoped, local variable, optionally initializing it to a value.
- **const** - Declares a block-scoped, read-only named constant.

### Data Structures and types

- **Boolean** - true or false
- **null** - A special keyword denoting a null value
- **undefined** - A top-level property whose value is not defined
- **Number** - An integer of floating point number
- **BigInt** - An integer with arbitrary precision
- **String** - A sequence of characters that represent a text value
- **Symbol** - (new in ECMAScript 2015). A data type whose instances are unique and immutable.

- **Object** - This is a reference data type used to define collections of data - Date,RegExp,Math

-We can get the type of a variable using typeof
-In computer science, aliteral is anotation representing a fixed value in the source code
-Comments // /\* \*/

## Operators

- Assignement,Comparison,Arithmetic,Bitwise,Logical,String,Conditional,Comma,Unary,Relational

### Assignement

- = , += , -= , \*= , /= , %=

### Comparison

- == , != , === , !== ,> , >= , < , <=

### Arithmetic

- %,+,-,--,++,\*\*,/

### Logical Operators

- &&,||,!

## Conditional Flow

- if/else if/else
- switch

## Loops

- for
- do..while
- while
- break
- continue
- for...in
- for.. of

## template literals

- Template literals are string literals allowing embedded expressions

## Arrays

- An array is an ordered set of values that you refer to with a name and an index.
- creating arrays,populating arrays,looping through an array,length
- Array methods
  - concat
  - join
  - push
  - pop
  - shift
  - unshift
  - slice(start,stop)
  - splice(index,count_to_remove,element)
  - reverse()
  - sort()
  - indexOf
  - forEach -do after function
  - map
  - every
  - some
  - reduce

## Functions

- A function is a JavaScript procedure—a set of statements that performs a task or calculates a value. To use a function, you must define it somewhere in the scope from which you wish to call it.
- function declaration/function definition/function statement
- function expressions
- calling functions
- function scope - discussion on scope - scope defines the lifetime and visibility of a variable. Variables are not visible outside the scope in which they are declared.
- function parameters -default parameters,rest parameters
- Arrow Functions

## Math and Date Objects

- new Date(),Math.
- **Date**
  - Nothing: creates today's date and time. For example, today = new Date();.
  - A string representing a date in the following form: "Month day, year hours:minutes:seconds." For example, var Xmas95 = new Date("December 25, 1995 13:30:00"). If you omit hours, minutes, or seconds, the value will be set to zero.
  - A set of integer values for year, month, and day. For example, var Xmas95 = new Date(1995, 11, 25).
  - A set of integer values for year, month, day, hour, minute, and seconds. For example, var Xmas95 = new Date(1995, 11, 25, 9, 30, 0);.

## Object Literals

- In object literal notation, an object description is a set of comma-separated name/value pairs inside curly braces. The names can be identifiers or strings followed by a colon.

## JSON

- JavaScript Object Notation (JSON) is a standard text-based format for representing structured data based on JavaScript object syntax. It is commonly used for transmitting data in web applications (e.g., sending some data from the server to the client, so it can be displayed on a web page, or vice versa).
- Even though it closely resembles JavaScript object literal syntax, it can be used independently from JavaScript, and many programming environments feature the ability to read (parse) and generate JSON.JSON exists as a string — useful when you want to transmit data across a network. It needs to be converted to a native JavaScript object when you want to access the data. This is not a big issue — JavaScript provides a global JSON object that has methods available for converting between the two.A JSON object can be stored in its own file, which is basically just a text file with an extension of .json

### Arrays JSON

- an array is also valid JSON, in this case each element is the array must be wraped around the {} braces(you still need to follow JSON rules)

### Special Nuances of JSON

- JSON is purely a data format — it contains only properties, no methods.
- JSON requires double quotes to be used around strings and property names. Single quotes are not valid.
- Even a single misplaced comma or colon can cause a JSON file to go wrong, and not work
- JSON can actually take the form of any data type that is valid for inclusion inside JSON, not just arrays or objects. So for example, a single string or number would be a valid JSON object
- Unlike in JavaScript code in which object properties may be unquoted, in JSON, only quoted strings may be used as properties.

## JavaScript Modules and Packages

- A module is a JavaScript file that exports one or more values(objects,functions or variables) using the export keyword. Modules can be loaded by the Node.js require() function
  - Inbuilt Modules
  - ThirdParty Modules
  - Own Modules
- A package is a directory/folder containing a program described by a package.json file. A package usually contains one or more Node modules.
- npm init/yarn init command initializes a folder as a package with a package.json, any third party modules installed will be inside a node_modules folder in this folder

## Creating Object using ES6 Classes (Maybe)
