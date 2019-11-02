<!---Tags=["javascript", "number", "string",  "boolean", "comparison]--->

# Javascript Value Types

## String
See the Lesson here : [String](https://di-learning.com/courses/43/sections/190/chapters/204)

### 1.  Long literal strings

Rather than having lines that go on endlessly, you can specifically break the string into multiple lines in 
the source code without affecting the actual string contents.

*The `+`operator*

```javascript
let longString = "This is a very long string which needs " +
                 "to wrap across multiple lines because " +
                 "otherwise my code is unreadable.";
```

*The backslash character `\`*

At the end of each line to indicate that the string will continue on the next line. 
Make sure there is no space or any other character after the backslash 

```javascript
let longString = "This is a very long string which needs \
to wrap across multiple lines because \
otherwise my code is unreadable.";
```

### 2.  String Properties

- Built-in `length` property:

```javascript
var length_txt = longString.length 
```

### 3.  String Methods

- The `indexOf()` method : returns the **index of (the position of) the first occurrence** of a specified text in a string:
Return -1 if the text is not found

```javascript
var str = "hello Everyone, please say hello to the class ";
var pos = str.indexOf("hello"); // pos = 0
```

- The `substring(start, [length])`methods: returns the characters in a string beginning at “start” and through the 
specified number of characters, “length”. “Length” is optional, and if omitted, up to the end of the string is assumed.

```javascript
var str = "Hello Everyone, please say hello to the class ";
str.substring(0,4) //returns "hell"
str.substring(2,4) //returns "lo"
```

-  The `toLowerCase()`method : Returns the string with all of its characters converted to lowercase.

```javascript
var str = "Hello Everyone, Please say hello to the class ";
str.toLowercase() //returns "hello everyone, please say hello to the class "
```

## Number
See the Lesson here : [Number](https://di-learning.com/courses/43/sections/190/chapters/196)

### 3.  String Methods

- The `isNaN(x)`method: return true or false

```javascript
var op = 10/"me";
isNaN(op);   //returns true because op is Not a Number
```

-The `toString()` method: returns a number as a string.
```javascript
var op = 10;
op.toString();     //returns "10"
```

- The `toFixed()` method: returns a string, with the number written with a specified number of decimals:
```javascript
var op = 10.6789
op.toFixed(0);           // returns 11
op.toFixed(2);           // returns 10.68.
```

## Boolean

JavaScript has a Boolean data type. It can only take the values `true` or `false`

- The Boolean() method: to find out if an expression (or a variable) is true
```javascript
var op = Boolean(10 > 9)   // op returns true
```

## Comparaison
See the Lesson here : [Logical Operators](https://di-learning.com/courses/43/sections/190/chapters/199)

## Array

JavaScript arrays are used to store multiple values in a single variable. : it's a **list** of values
Arrays are  are a special type of objects. The typeof operator in JavaScript returns "object" for arrays.

*Syntax*

```
var array_name = [item1, item2, ...]; 
```

```javascript
var colors = ["blue", "yellow", "green"]; 
console.log(typeof colors) // object
```

### 1.  Accessing elements in an array

You use the the index number: starting at **0**

```javascript
var colors = ["blue", "yellow", "green", 54]; 
var favorite = colors[0];
var second_favorite = colors[2];
console.log(favorite) // blue
console.log(second_favorite) // green
```

### 2.  Changing an Array Element
```javascript
var colors = ["blue", "yellow", "green"]; 
colors[0] = "pink"
console.log(colors) // ["pink", "yellow", "green"]; 
```

### 3 .Array properties

- The `lenght` property:  returns the length of an array (the number of array elements). Starts at **1**
```javascript
var colors = ["blue", "yellow", "green"]; 
colors.length // 3
```

### 4 .Array methods

- The `push()`method : add a new element to the end of an array

```javascript
var colors = ["blue", "yellow", "green" ]; 
colors.push("orange") // var colors = ["blue", "yellow", "green", "orange"];
```

- The `pop()`method : removes the last element from an array:


```javascript
var colors = ["blue", "yellow", "green" ]; 
colors.pop() // var colors = ["blue", "yellow"];
```

- The `splice()`method : add new items to an array/ remove items

The first parameter defines the position where new elements should be added (spliced in).
The second parameter defines how many elements should be removed.
The rest of the parameters define the new elements to be added.
The splice() method returns an array with the deleted items:

```javascript
var colors = ["blue", "yellow", "green" ]; 
colors.splice(1, 1, 45, 23); // var colors = ["blue", 45, 23, "green" ]; 
```

- The `slice()` method: slices out a piece of an array into a new array.
The slice() method creates a new array. It does not remove any elements from the source array.
The method then selects elements from the start argument, and up to (but not including) the end argument.
```javascript
var colors = ["blue", "yellow", "green", "pink" ]; 
var favorite : colors.slice(2) // favorite = ["green" , "pink"]; 
var second_favorite : colors.slice(0,1) // favorite = ["blue"]; 
```

- the `toString() `method:  converts an array to a string of (comma separated) array values.

```javascript
var colors = ["blue", "yellow", "green" ]; 
colors.toString() // blue,yellow,green
```

## Object
Objects in JavaScript may be defined as an *unordered collection of related data*,  in the form of 
`“key: value”` pairs. These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

> Example :  A lamp has properties  -->  height,width, brightness  and  has methods (an action) --> to shine

*Syntax*
```
var x = {
  property: value,
  property: value,    
  method: function(){}
  ...
};
```

```javascript
var person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```

### 1. Accessing  Object properties

*Syntax*
```
objectName.propertyName
OR
objectName["propertyName"]
```

```javascript
var person = {
  firstName: "John",
  lastName: "Doe",
};
console.log(person.firstName) // John
console.log(person[firstName]) // John
```

### 2. Adding/ Changing Object properties 

```javascript
var person = {
  firstName: "John",
  lastName: "Doe",
};
person.firstName = "Sarah"
person.eye_color= "blue"

console.log(person) 
// {
//   firstName: "Sarah",
//   lastName: "Doe",
//  eye_color: "blue"
// };
```

### 2. Deleting Object properties 

```javascript
var person = {
  firstName: "John",
  lastName: "Doe",
};
delete person.firstName
console.log(person) 
// {
//   lastName: "Doe",
// };
```




