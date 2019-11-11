# Exercises

### Exercise 1
```html run
<html>
<body>
  <div id="container">Users:</div>
  <ul class="list">
    <li>John</li>
    <li>Pete</li>
  </ul>
  <ul class="list">
    <li>Sarah</li>
    <li>Dan</li>
  </ul>
</body>
</html>
```
For the questions below, use at least **2 PROPERITIES** to access :
1. The `<div>` node
2. The `<ul>` nodes,. and render all of it's children one by one
3. The first `<li>` of each `<ul>`

### Exercise 2
```html run
<html>
<body>
  <div id="container">Users:</div>
  <ul class="list">
    <li>John</li>
    <li>Pete</li>
  </ul>
  <ul class="list">
    <li>David</li>
    <li>Sarah</li>
    <li>Dan</li>
  </ul>
</body>
</html>
```
1. Change the name "Pete" by "Richard"
2. Change each first name of the `<ul>` by your name
3. Add add the end of each `<ul>`, a paragraph that says "Hey students"
4. Delete the `<li>` Sarah
5. Bonus: 
* Change the class of `<ul>` by "student_list"
* Add a class "university" to the first `<ul>`

### Exercise 3 **NINJA -- Event**
``` html run
<article>
<h1> Some Facts </h1>
<h2> The CHOCOLATE </h2>
<p>Chocolate is made from tropical Theobroma cacao tree seeds. Its earliest use dates back to the Olmec civilization in Mesoamerica.</p>
<p> After the European discovery of the Americas, chocolate became very popular in the wider world, and its demand exploded. </p>
<p>  Chocolate has since become a popular food product that millions enjoy every day, thanks to its unique, rich, and sweet taste.</p> 
<p> But what effect does eating chocolate have on our health?<:p> </article>
What is your name ?<input type="text" name="userName">
What did you think of the article ?<input type="text" name="questionToUser">
```

1.	Give to all paragraphs inside the article tag the class  `para_article` 
2.	Remove the last paragraph in the article.
3.	Add an event listener so that when you click on the h2, it is removed from the DOM.
4.	Set the font size of the h1 to be a random pixel size from 0 to 100.
5.	Hide the 1st paragraph, when it's clicked 
6.	Fade out the 2nd paragraph over 2000 milliseconds, when it's clicked
7.	Get the value in the inputs and append it to the end of the html, inside a table

### Exercise 4  **NINJA  -- Event**

1.	Create a form with two inputs text : student_first_name and lstudent_last_name and a button.
2.	When the teacher clicks on the button, append the complete student name in a list.
3.	Create another button that calculates the number of students aldready added to the class. Alert the number when the button is clicked.
4.	Bonus : Create a delete button next to each student, when it's clicked, it should delete the student

### Exercise 4  **GOLD**

Write a function `createCalendar(elem, year, month)`
The call should create a calendar for the given year/month and put it inside elem.
The calendar should be a table, where a week is `<tr>`, and a day is `<td>`. The table top should be `<th>` with weekday names: the first day should be Monday, and so on till Sunday.
For instance, createCalendar(cal, 2012, 9) should generate in element cal the following calendar:

MO | TU | WE | TH | FR | SA | SU
------------ | ------------- | ------------- | ------------- | ------------- | ------------- | -------------
.| . | . | . | . | 1| 2
3| 4 | 5| 6| 7 | 8 | 9 | 
10| 11 | 12| 13| 14 | 15 | 16 | 
17| 18 | 19| 20| 21 | 22 | 23 | 
24| 25 | 26| 27| 28 | 29 | 30 | 