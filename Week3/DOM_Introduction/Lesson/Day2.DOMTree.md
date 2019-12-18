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
element.children[index]
element.firstElementChild
element.lastElementChild
element.parentNode
element.nextSibling
element.previousSibling
element.textContent
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
var demoQueryAll = document.querySelectorAll('.demo-query-all');

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
getElementsByName | `name`
getElementsByTagName | tag or '*'
getElementsByClassName |  `class`

## Changing DOM nodes


1.   Changing  the HTML
* **innerHTML** property for node element
```javascript
document.getElementById(“header”).innerHTML = “Hello World!”;
document.getElementsByTagName("div").innerHTML = "<h1>Hello World!</h1>"
```
* **data** property for text element
```javascript
let text = document.body.firstChild;
text.data = "Hello"
```

2. Creating elements
* **createElement** method
*Syntax*
`document.createElement(tag)`
```javascript
    var div = document.createElement(‘div’);
```

* **createTextNode** method
*Syntax*
`document.createTextNode(text)`
```javascript
    let textNode = document.createTextNode('Here I am');
```

3. Adding Element
* **append** method
*Syntax*
`element.append`
```javascript
    document.body.append(div);
```

Method	 | Goal	
------------ | -------------
node.append() |  append nodes or strings at the end of node,
node.prepend() | insert nodes or strings at the beginning of node,
node.before() | insert nodes or strings before node,
node.after() | insert nodes or strings after node,
node.replaceWith() |  replaces node with the given nodes or strings.


3. Deleting elements
* **removeChild** method
```javascript
var elem = document.querySelector('#header');
elem.parentNode.removeChild(elem);
```
* **remove** method
```javascript
var elem = document.querySelector('#header');
elem.remove();
```
