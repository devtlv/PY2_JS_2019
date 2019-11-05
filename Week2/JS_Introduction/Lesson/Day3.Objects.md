<!---Tags=["object", "properties", "method"]-->

# Objects

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

## 3. Methods
Methods are actions.
They are stored in properties as function definitions.

*Syntax*
```
var object= {
    property : value,
    property : value,
    property : function () {
        statement
    }
}
```

```javascript
var person= {
    firstName : "Sarah",
    eye_color: "blue"
    eat : function () {
        console.log("I love chocolate)
    }
}
```

## 2. Keyword `this`

`this `refers to the object. 
`this.property`is the property of **this object**.

```javascript
var person= {
    firstName : "Sarah",
    eye_color: "blue"
    eat : function () {
        console.log("My name is" + this.firstName + "I love chocolate")
    }
}
```

## 2. Accessing object method 

*Syntax*
```
object.function()
```

```javascript
var person= {
    firstName : "Sarah",
    eye_color: "blue"
    eat : function () {
        console.log("My name is" + this.firstName + "I love chocolate")
    }
}
person.eat()
```



