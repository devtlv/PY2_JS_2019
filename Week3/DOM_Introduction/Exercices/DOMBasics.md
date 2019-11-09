<!--Tags=["DOM"]-->

# Exercises

### Exercise 1:
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
1. The <div> DOM node?
2. The <ul> DOM node?
3. The second <li> (with Pete)?

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
1. Change the background color of the <div> DOM node and inscrease its padding
2. Don't display the first name (John) and give a border to the second name (Pete)
3. Change the font size of the whole HTML


### Exercise 3 NINJA
```html run
<!DOCTYPE HTML>
<html>
<head>
  <style>
    table {
      border-collapse: collapse;
    }
    td {
      border: 1px solid black;
      padding: 3px 5px;
    }
  </style>
</head>

<body>
  <table>
    <tr>
      <td>1:1</td>
      <td>2:1</td>
      <td>3:1</td>
      <td>4:1</td>
      <td>5:1</td>
    </tr>
    <tr>
      <td>1:2</td>
      <td>2:2</td>
      <td>3:2</td>
      <td>4:2</td>
      <td>5:2</td>
    </tr>
    <tr>
      <td>1:3</td>
      <td>2:3</td>
      <td>3:3</td>
      <td>4:3</td>
      <td>5:3</td>
    </tr>
    <tr>
      <td>1:4</td>
      <td>2:4</td>
      <td>3:4</td>
      <td>4:4</td>
      <td>5:4</td>
    </tr>
    <tr>
      <td>1:5</td>
      <td>2:5</td>
      <td>3:5</td>
      <td>4:5</td>
      <td>5:5</td>
    </tr>
  </table>
  <script>
    let table = document.body.firstElementChild;
    // your code
  </script>
</body>
</html>
```

1. Write the code to paint all diagonal table cells in red. 