4.  Changing a value of an attribute

```javascript
document.getElementsByTag(“img”).src = “test.jpg”;
```

```html run
<input type="text" id="elem" value="value">

<script>
  alert(elem.type); // "text"
  alert(elem.id); // "elem"
  alert(elem.value); // value
</script>
```