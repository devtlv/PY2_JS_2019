<!---Tags=["ES6"]--->

# ES6

Makes JavaScript better and easier to write, and is used with modern web technologies like **React**, **Node.js**.

## Variables

###  Reminder on Scopes

#### Local scope : Inside a function
```javascript
function sayHello(){
    var name = "Sarah"
}
console.log(name) // undefined
```

#### Global scope: Accessible everywhere
```javascript
var name = "Sarah"

function sayHello(){
    console.log(name) //  "Sarah"
}
console.log(name) //  "Sarah"
```

### The problem of the keyword `var`

#### NEW with ES6 : Block scope (Everythig between curly brackets - if/else or for loop)
The `var`keyword make the variable inside a block accessible outside the block
```javascript
if (age > 18) {
    var canDrive = true 
    console.log(icanDrive; // true
} 
console.log(canDrive);  // true
```

#### Redeclaration 
```javascript
var name = "Sarah"
var name = "Dan"
console.log(name);  // Dan  
```

### The solution with of the keyword `let`

#### Support Block scope
```javascript
if (age > 18) {
    let canDrive = true 
    console.log(icanDrive; // true
} 
console.log(canDrive);  // undefined
```

#### Doesn't allow redeclaration  but the variable car be changed
```javascript
let name = "Sarah"
let name = "Dan" // name has already been declared

name = "David"
console.log(name) // David
```

### The solution with of the keyword `const`

####  Support Block scope
```javascript
if (age > 18) {
    const canDrive = true 
    console.log(icanDrive; // true
} 
console.log(canDrive);  // undefined
```

#### Doesn't allow redeclaration and the variable can't be changed
```javascript
const name = "Sarah"
name = "David" // constant variable
```

## Functions

### Function declaration

*Syntax*
```
function myFunction(parameters) {
  // statement to execute
}
myFunction(arguments)
```
### Function expression
Functions stored in variables do not need function names. They are always invoked (called) using the variable name.

*Syntax*
```
var x = function (parameters) {
  // statement to execute
}
x(arguments)
```
### ES6 Arrow Function
Concise way to write functions in JavaScript.

*Syntax*
```
const myFunction = () => {
   // statement to execute
}
```

```javascript
const show = (name, age) => {
    console.log(name, age);
}
show ("Sarah",20) 
```

```javascript
const show = (x, y) => x + y
```

```javascript
const show = x => x *2
```

Arrow functions allow you to have an implicit `return` values are returned without having to use the `return` keyword.
```javascript
const show = x => x *2
show(3) // 6
```



