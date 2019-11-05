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

