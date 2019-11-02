<!---Tags=["if", "else","while","switch"]--->

# Conditional JS

JavaScript supports conditional statements which are used to perform different actions based on different conditions.

## If...else

![If...Else](https://www.tutorialspoint.com/javascript/images/decision_making.jpg)

JavaScript supports the following forms of if..else statement :

* if statement
* if...else statement
* if...else if... statement.

### 1. if statement

*Syntax*
```
if (expression) {
   Statement(s) to be executed if expression is true
}
```

```javascript
    if (age > 18) {
        console.log("You're a big man")
    }
```

### 2. if...else statement

*Syntax*
```
if (expression) {
   Statement(s) to be executed if expression is true
} else {
   Statement(s) to be executed if expression is false
}
```

```javascript
    if (age > 18) {
        console.log("We can go to a pub together !!")
    } else {
         console.log("Sorry...You have to stay at home tonight")
```

### 3. if...else if... statement.

*Syntax*
```
if (expression 1) {
   Statement(s) to be executed if expression 1 is true
} else if (expression 2) {
   Statement(s) to be executed if expression 2 is true
} else if (expression 3) {
   Statement(s) to be executed if expression 3 is true
} else {
   Statement(s) to be executed if no expression is true
}
```

```javascript
    if (age === 18) {
        console.log("It's your birthday !!) 
    } else if (age > 18) {
        console.log(We can go to a pub together !!")
    } else {
        console.log("Sorry...You have to stay at home tonight")
    }
```
## Switch Case

Use the switch statement to select one of many code blocks to be executed.

*Syntax*
```
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
``` 

### 1. How does it work ?

* The switch expression is evaluated once.
* The value of the expression is compared with the values of each case.
* if there is a match, the associated block of code is executed.

If multiple cases matches a case value, the **first** case is selected.
Switch cases use **strict comparison (===)**. The values must be of the same type to match.


```javascript
var expr = 'Papayas';
switch (expr) {
  case 'Oranges':
    console.log('Oranges are $0.59 a pound.');
    break;
  case 'Mangoes':
  case 'Papayas':
    console.log('Mangoes and papayas are $2.79 a pound.');
    // expected output: "Mangoes and papayas are $2.79 a pound."
    break;
  default:
    console.log('Sorry, we are out of ' + expr + '.');
}
```

### 2. The break Keyword

When JavaScript reaches a `break` keyword, it breaks out of the switch block.
This will stop the execution of inside the block.
It is not necessary to break the last case in a switch block. The block breaks (ends) there anyway.

### 3. The default Keyworkd

The `default` keyword specifies the code to run if there is no case match:
The `default` case does not have to be the last case in a switch block:

```javascript
var expr = 'Papayas';
switch (expr) {
  case 'Oranges':
    console.log('Oranges are $0.59 a pound.');
    break;
  default:
    console.log('Sorry, we are out of ' + expr + '.');
    break;
  case 'Mangoes':
  case 'Papayas':
    console.log('Mangoes and papayas are $2.79 a pound.');
    // expected output: "Mangoes and papayas are $2.79 a pound."
    break;
}
```