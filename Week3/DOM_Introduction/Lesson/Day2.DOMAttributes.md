# HTML Attributes

### 1.  Accessing and changing a value of an attribute

Method  | Goal
------------ | -------------
elem.hasAttribute(name) | checks for existence.
elem.getAttribute(name) | gets the value.
elem.setAttribute(name, value) | sets the value.
elem.removeAttribute(name) |  removes the attribute.

```html run
<body>
  <div id="elem" about="Elephant"></div>

  <script>
    alert(elem.getAttribute('About') ); // (1) 'Elephant', reading

    elem.setAttribute('Test', 123); // (2), writing

    for (let attr of elem.attributes) { // (4) list all
      alert( `${attr.name} = ${attr.value}` );
    }
  </script>
</body>
```

### 2. Other Examples

```javascript
document.getElementsByTagName(“img”).src = “test.jpg”;
```

```html run
<input type="text" id="elem" value="value">

<script>
  alert(elem.type); // "text"
  alert(elem.id); // "elem"
  alert(elem.value); // value
</script>
```