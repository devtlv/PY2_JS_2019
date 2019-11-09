<!--Tags=["tree", "DOM"]-->

# The DOM Tree

## Accessing DOM nodes

A **document tree** is a node tree whose root is a document.
The **document element**  is the element whose parent is that document,

### Relations between DOM nodes

1. Accessing nodes with properties

``` html run
<html>
<body>
  <div>Begin</div>

  <ul>
    <li>Information</li>
  </ul>

  <div>End</div>
  <script>
        for (let i = 0; i < document.body.childNodes.length; i++) {
        alert( document.body.childNodes[i] ); // Text, DIV, Text, UL, ..., SCRIPT
        }
  </script>
</body>
</html>
```

Accessing elements : 
```
element.childNodes[index]
element.firstChild
element.lastChild
element.parentNode
element.nextSibling
element.previousSibling
```

2.  Accessing  nodes with methods

```
element.getElementById()
element.getElementsByClassName()
element.querySelector()
```

```javascript
document.getElementById('demo');
document.getElementsByClassName('demo');
document.getElementsByTagName('article');
document.querySelector('#demo-query');
document.querySelectorAll('.demo-query-all');

demoQueryAll.forEach(query => {
  query.style.border = '1px solid green';
});

// Also 
// elem.querySelectorAll(css) returns all elements inside elem matching the given CSS selector.

document.querySelectorAll('ul > li:last-child');
document.querySelectorAll(':hover')

```

## SUM UP

Method	 | Searches by...	
------------ | -------------
querySelector | CSS-selector
querySelectorAll | CSS-selector
getElementById | `id`
getElementsByName | `name``
getElementsByTagName | tag or '*'
getElementsByClassName |  `class`

3.  Changing  the HTML
* **innerHTML** property for node element
```javascript
document.getElementById(“#header”).innerHTML = “Hello World!”;
document.getElementsByTagName("div").innerHTML = "<h1>Hello World!</h1>"
```
* **data** property for text element
```javascript
let text = document.body.firstChild;
text.data = "Hello"
```

5. Adding elements
* **createElement** method, **appendChild** method
```javascript
var div = document.createElement(‘div’);
var newContent = document.createTextNode("Hello World!"); 
div.appendChild(newContent);
```

6. Deleting elements
```javascript
var elem = document.querySelector('#header');
elem.parentNode.removeChild(elem);
```


