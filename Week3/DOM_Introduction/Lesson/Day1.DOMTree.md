<!--Tags=["tree", "DOM"]-->

# The DOM Tree

## Accessing DOM nodes

A **document tree** is a node tree whose root is a document.
The **document element**  is the element whose parent is that document,

### Relations between DOM nodes

1. Accessing nodes properties

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

2.  Accessing nodes method

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
```

