<!-Tags=["javascript", "variables", "user-interface functions","boolean, "comparison"]-->
# Javascript variables and user-interface functions

## Variables

In a programming language, variables are used to **store data values**.
JavaScript uses the `var `keyword to declare variables.
An `equal` sign is used to **assign values to variables**.

```javascript
var x = 3
```

## Keywords

The `var` keyword tells the browser to create variables:

```javascript
var x, y;
x = 5 + 6;
y = x * 10;
```


## Comments

Code after double slashes `//` or between `/*` and `*/ `is treated as a comment.
Comments are ignored, and will not be executed:

```javascript
var x = 5;   // I will be executed
// var x = 6;   I will NOT be executed
```

## User-interface functions

The mini-window with the message is called a modal window. The word “modal” means that the visitor can’t interact with 
the rest of the page, press other buttons, etc. until they have dealt with the window. 

1. alert

This shows a message and **pauses script execution** until the user presses “OK”.


```javascript
    //alert(message);
    alert("Hello");
```

2. prompt

It shows a modal window with a text message, **an input field** for the visitor, and the buttons OK/Cancel.
The visitor may type something in the prompt input field and press OK. Or they can cancel the input by pressing Cancel or hitting the Esc key.
The call to prompt returns the text from the input field or null if the input was cancel


```javascript
    //`var result = prompt(title, [default])
    //  title : the text to show the visitor.
    // default: optional second parameter, the initial value for the input field.
    var age = prompt('How old are you?', 20);
    alert(`You are ${age} years old!`); // You are 20 years old!
```

3. confirm

The function confirm shows a modal window with a question and two buttons: OK and Cancel.
The result is `true`if OK is pressed and `false` otherwise

```javascript
    //var result = confirm(question);
    var isBoss = confirm("Are you the boss?");
    alert( isBoss ); // true if OK is pressed
```



