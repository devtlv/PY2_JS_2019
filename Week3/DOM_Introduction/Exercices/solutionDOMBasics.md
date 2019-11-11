# Solutions

### Execise 1:

```html run
<html>
<body>
  <div>Users:</div>
  <ul>
    <li>John</li>
    <li>Pete</li>
  </ul>
</body>
</html>
``` 

For each of the questions, find **2 WAYS** of accessing :
1. The  `div` DOM node?
2. The `ul` DOM node?
3. The second `li` (with Pete)?


```javascript
1) 
document.querySelector("div")
document.getElementsByTagName("div")[0]
document.body.firstElementChild

2) 
document.getElementsByTagName("ul")[0]
document.querySelector("ul")
document.body.childNodes[3]
document.body.children[1]

3)
document.querySelectorAll("li")[1]
document.querySelector("ul").lastElementChild


4)  Get John from Pete
document.querySelectorAll("li")[1].previousElementSibling
5) Gt the ul from Pete
document.querySelectorAll("li")[1].parentNode
```

### Exercise 2

```html run
<html>
<body>
  <div>Users:</div>
  <ul>
    <li>John</li>
    <li>Pete</li>
  </ul>
</body>
</html>
``` 
For the following exercises, you can help yourself with this [website](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference):
1. Change the background color of the `div` DOM node to lightblue and inscrease its padding
2. Don't display the first name (John) and give a border to the second name (Pete)
3. Change the font size of the whole HTML
4. Bonus:
* Check if the background color of the `div` is lightblue, if yes alert "Hello x and y" (x and y are the new users)

```javascript
document.querySelector("div").style.backgroundColor = "lightblue"

document.querySelector("div").style.padding = "20px"

document.querySelectorAll("li")[1].previousElementSibling.style.display="none"

document.querySelectorAll("li")[1].style.visibility="hidden"  // keep the space

document.querySelector("div").style.border="1px solid blue"

document.body.style.fontSize = "40px"

window.getComputedStyle(document.querySelector("div"), null).getPropertyValue('background-color');
// rgb(173, 216, 230)

```
