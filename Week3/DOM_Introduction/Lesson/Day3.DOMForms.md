# Forms

## 1. Accessing a Form

Document forms are members of the special collection `document.forms`

```html run
<form name="my">
  <input name="one" value="1">
  <input name="two" value="2">
</form>

<script>
  // get the form
  let form = document.forms.my; // <form name="my"> element
  // OR
  let form = document.forms[0]; // the first form on the page

  //  get the number of forms on the page
  document.forms.length

  // get the element
  let elem = form.elements.one; // <input name="one"> element
</script>
```

## 2. Accessing /Changing an attrivute of an element of a Form

```html run
<form name="my">
  <input name="one" value="1">
  <input name="two" value="2">
</form>

<script>
  let form = document.forms.my; // <form name="my"> element
  let elem = form.elements.one; // <input name="one"> element

  console.log(elem.value); // 1
  elem.value = 'hey' // value = 'hey'

  //If it's radio button
  console.log(input.checked)// true OR false
</script>
```

## 3. `select` Form

Properties | Goal
----- | -----
select.options | the collection of `<option>` subelements,
select.value | the value of the **currently selected** `<option>`
select.selectedIndex |  the number of the **currently selected** `<option>`

```html run
<select id="select">
  <option value="apple">Apple</option>
  <option value="pear">Pear</option>
  <option value="banana">Banana</option>
</select>

<script>
  // all three lines do the same thing
  select.options[2].selected = true;
  select.selectedIndex = 2;
  select.value = 'banana';
</script>

```

## 4.  Form Events

We saw before the events: `onchange` and `oninput`.

* `onsubmit` to submit a form. 
Used : if you click on un input `type=submit` and when you press Enter on an input field.
```html run
<form onsubmit="alert('submit!');">
  First: Enter in the input field <input type="text" value="text"><br>
  Second: Click "submit": <input type="submit" value="Submit">
</form>
```

### Using `event.preventDefault()`

Many browser events have a “default action". `event.preventDefault()` send a signal that those actions should be canceled.
You should use this method to prevent a from from submitting but you click on a "Submit" button. 
It prevents the page from refreshing. 


