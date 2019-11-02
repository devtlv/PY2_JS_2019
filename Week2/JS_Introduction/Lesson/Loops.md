<!---Tags=["loop", "for", "while"]--->

# Javascript Loop
To run the same code / repeat an action some number of times.
It's the execution of a set of instructions/functions repeatedly while some condition evaluates to true.

## For Loop
 
 *Syntax* 

 ```javascript
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```
Statement 1 :  marks the start of a for loops
Statement 2 : defines the condition for executing the code block. Must return a boolean value.
Statement 3 : is executed (every time) after the code block has been executed.
When the condition becomes false, the loop terminates marking the end of its life cycle.

```javascript
for (i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}
```

![For Loop](https://media.geeksforgeeks.org/wp-content/uploads/loop2.png)


## For/In Loop

Loops through the **properties of an object**.  This loop continues until all of the properties of the Object are processed.

*Syntax*
```
for (variable in object)
  statement`
```
 
```javascript
var person = {fname:"John", lname:"Doe", age:25};
for (x in person) {
  console.log(person[x]) // John Doe 25
}
```

## For/Of Loop

Loops through the values of an iterable objects such as Arrays, Strings and more.
`for...in`iterates over property names, `for...of` iterates over property values:

*Syntax*
```
for (variable of object)
  statement
```

``` javascript
var colors = ["blue", "yellow", "red"];

for ( i in colors) {
   console.log(i); // logs "0", "1", "2",
}

for (i of colors) {
   console.log(i); // logs blue, yellow, red
}
```

## While Loop

Allows code to be executed repeatedly based on a given **Boolean condition**.

*Syntax*
```
while (boolean condition)
{
   loop statements...
}
```

![While Loop](https://media.geeksforgeeks.org/wp-content/uploads/Loop1.png)

1.  Checks the condition -->  If it evaluated to true, then the loop body statements are executed otherwise first statement following the loop is executed. 
When the condition becomes false, the loop terminates which marks the end of its life cycle.

```javascript
var n = 0;
while (n < 3) {
  n++;
  console.log(n)
}
```

`for loops` and `while loops` are called **Entry Controlled loops** because the condition is tested before entering the loop body.

## Do while  Loop

Similar to `while loop` but it checks for condition **after executing** the statements. This is an of **Exit Control Loop.**
The test condition is tested or evaluated at the end of loop body. Therefore, the loop body will execute at least once, whether the test condition is true or false.

*Syntax*
```
do
{
    statements..
}
while (condition);
```
![Do While Loop](https://media.geeksforgeeks.org/wp-content/uploads/loop3.png)

```javascript
do {
  text += "The number is " + i;
  i++;
}
while (i < 10);
```

## Break Statement
The `break` statement **breaks the loop** and continues executing the code after the loop

```javascript`
for (i = 0; i < 10; i++) {
  if (i === 3) { 
      break;
    }
  text += "The number is " + i + "<br>"; // 0 1 2
}
```

## Continue Statement
The` continue` statement **breaks one iteration (in the loop),** and continues with the next iteration in the loop.

```javascript
for (i = 0; i < 10; i++) {
  if (i === 3) { continue; }
  text += "The number is " + i + "<br>"; // 0 1 2 4 5 6 7 8 9 
}
```


