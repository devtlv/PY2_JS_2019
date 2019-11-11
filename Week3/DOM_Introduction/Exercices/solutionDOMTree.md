# Solution

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


### Solution
```javascript
1) 
document.querySelector("ul").lastElementChild.innerHTML = "Richard"

2)
var ul = document.querySelectorAll("ul")
for (var i = 0; i < ul.length; i++){
	ul[i].firstElementChild.innerHTML = "Lise"
}

3) 
for (var i = 0; i < ul.length; i++){
	var newElem = document.createElement('li')
	newElem.innerHTML="HeyStudents"
	ul[i].append(newElem)
}

4) 
var name = document.querySelectorAll("ul")[1]
var sarah = name.children[1]
sarah.remove()
```
