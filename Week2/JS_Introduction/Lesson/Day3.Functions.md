<!--Tags=["functions"]--->

# Functions

## What is a function ?

It's block of code designed to perform a particular task.
They allow the code to be called many times without repetition.
Avoid code duplication

### 1. Defining/Declaring a function

*Syntax*
```
function fnt_name(parameters){
  statements
}
```

**Parameters** are used when defining a function, they are the **names** created in the function definition. 
Parameters are separated by commas in the` ()`.  

:warning: They are **only recognized** inside the function !!! The parameters behave as local variables.

```javascript
function myFunction(name, age) {
    console.log("My name is" + name + "my age is"  + "age)
}
```

**Arguments**, are the values the function **receives from each parameter** when the function is executed (invoked). 

```javascript
function myFunction(name, age) {
    console.log("My name is" + name + "my age is"  + "age)
}

myFunction("Sarah", 22)
myFunction("Ben", 40)
```

### 2. Calling/Inkocating a function

:warning: Functions execute when the function is **called**. 

If the function has no parameter you invoke it with the function name, followed by empty  parenthesis.
If the function has parameters you invoke it with the function name, followed by the number of arguments corresponding to the number of parameters (inside the parenthesis.)

```javascript
function myFunction(name, age) {
    console.log("My name is" + name + "my age is"  + age)
}

myFunction("Sarah", 22)
myFunction("Ben", 40)
```
### 3. Default values
If a parameter is not provided, then its value becomes `undefined`.

```javascript
function myFunction(name, age) {
    console.log("My name is" + name + "my age is"  + age) // age undefined 
}

myFunction("Sarah")
```

A default value with get passed it no argument was given during the invocation of the function. 

```javascript
function myFunction(name, age = 20) {
    console.log("My name is" + name + "my age is"  + age) // age: 20
}

myFunction("Sarah")
myFunction("Ben", 40) // age : 40
```

### 4. Local variables

A variable declared inside a function is **only visible inside that function.**
```javascript
function myFunction(name, age) {
    var eye_color = "blue"
    console.log("My name is" + name + "my age is"  + age + "I have" + eye_color + "eyes")
}

myFunction("Sarah", 22)
console.log(eye_color) // undefined
```

### 5. Global variables
Global variables are visible from any function

```javascript
var eye_color = "blue"

function myFunction(name, age) {
    console.log("My name is" + name + "my age is"  + age + "I have" + eye_color + "eyes")
}

myFunction("Sarah", 22)
console.log(eye_color) // blue
```

### 5. Return statement 

Every function in JavaScript returns `undefined` unless otherwise specified.
When a function `returns` a value, it's returning a result  The return value is "returned" back to the "caller" of the function

```javascript
function myFunction(name, age) {
    var result = "My name is" + name + "my age is"  + age 
    return result 
}

var girl = myFunction("Sarah", 22)
console.log(girl) // girl  = result 
```

```javascript
function myFunction(name, age) {
    if (name == "Sarah") {
        var result = "Hey" + name 
        return result 
    } else {
        return "You are not the right person"
    }
}

var girl = myFunction("Sarah", 22)
console.log(girl) // girl  = Hey Sarah
```

:warning: The return statement **stops function execution immediately**.

```javascript
function myFunction(name, age) {
    var result = "My name is" + name + "my age is"  + age 
    return "hey"
    return result 
}

var girl = myFunction("Sarah", 22)
console.log(girl) // girl  = "hey"
```

It is possible to use `return` without a value. That causes the function to exit immediately.

```javascript
function myFunction(name, age) {
    if (name != "Sarah") {
        return
    } 
    alert ("You are not the right person")
}

var girl = myFunction("Sarah", 22)
console.log(girl) // girl  = undefined
```


:warning:  A function should do exactly what is suggested by its name, no more. Two independent actions usually deserve two functions 
Functions should be short and do exactly one thing. If that thing is big, maybe it’s worth it to split the function into a few smaller functions
