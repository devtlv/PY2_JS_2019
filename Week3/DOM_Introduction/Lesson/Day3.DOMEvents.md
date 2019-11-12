# DOM Events

## Event handlers
An event handler is a function that runs in case of an event.

1. HTML-attribute :  set in HTML with an attribute named on<event>

```javascript
    <script>
    function inform(){
        alert("You clicked me")
    }
    </script>
    
    <form>
    <input type="button" name="test" value="Click me" onclick="inform()">
    </form>
```

**Some Event Handler**

Name | Goal
------------ | -------------
onclick() | invoke JavaScript upon clicking (a link, or form boxes)
onload() | invoke JavaScript after the page or an image has finished loading.
onmouseover() | invoke JavaScript if the mouse passes by some link
onmouseout( | invoke JavaScript if the mouse goes pass some link
onunload() | invoke JavaScript right after someone leaves this page.

More EventHandler [here](https://www.javatpoint.com/understanding-html-dom-events)

### Specific Event Handler

1. Event: change
The change event triggers when the element has finished changing.
For text inputs that means that the event occurs when it loses focus.
```html run
<input type="text" onchange="alert(this.value)">
<input type="button" value="Button">
```

2. Event: input
The input event triggers every time after a value is modified by the user. 
```html run
<input type="text" id="input"> oninput: <span id="result"></span>
<script>
  input.oninput = function() {
    result.innerHTML = input.value;
  };
</script>
```



2. DOM property: set a handler using a DOM property on<event>.
```javascript
    
    <form>
        <input  type="button" name="test" value="Click me">
    </form>
    
    <script>
       document.getElementById('button').onclick = function() {
            alert('Click!');
        };
    </script>
```

3. Element `this`

```javascript
<button onclick="alert(this.innerHTML)">Click me</button>
```

4. `addEventListener()`  to create multiple events on the same Element
*Syntax*
```
element.addEventListener(event, listener);
```
```javascript
x.addEventListener("click", RespondClick); 
y.addEventListener("mouseover", RespondMouseOver); 
y.addEventListener("mouseout", RespondMouseOut); 

function RespondMouseOver() { 
           //statement
 } 
  
function RespondMouseOut() { 
     //statement
} 
  
function RespondClick() { 
    //statement
} 
``` 

5. Event object
When an event happens, the browser creates an event object, puts details into it and passes it as an argument to the handler.

Event Object properties

Name | Description
------------ | -------------
e  | The object containing the event properties
type | The event that occurred (click, focus, blur, etc.)
target |  The element to which the event occurred

```javascript

<form>
    <input  type="button" name="test" value="Click me">
</form>

    <script>
        document.getElementById('button').addEventListener("click", RespondClick); 
        function RespondClick(e) {
            var evtType = e.type
            alert(evtType)  // click
            ~~var inputField=document.getElementById("email");~~
            var inputField=e.target;
            inputField.style.border="3px solid #6F3";
        }
    </script>
```

6. Bubbling

When an event happens on an element, it first runs the handlers on it, then on its parent, then all the way up on other ancestors.

```html run
<form onclick="alert('form')">FORM
  <div onclick="alert('div')">DIV
    <p onclick="alert('p')">P</p>
  </div>
</form>

<!-- click on P, alert P thant Div than Form -->
```
![Bubbling](https://miro.medium.com/max/633/1*rG3JcxeSnztEtmkEVzo4Hg.png)

#### Understanding the difference between `this`and `event.target`
* `event.target` – is the innermost element over which the event originated
* `this` (= `e.currentTarget`)– is the “current” element, the one that has a currently running handler on it.

```html run
  <form id="form">FORM
    <div>DIV
      <p>P</p>
    </div>
  </form>

  <script>
  form.onclick = function(event) {
  event.target.style.backgroundColor = 'yellow';
  console.log("target = " + event.target.tagName + ", this=" + this.tagName);
};
  </script>
  ```

#### Stop the bublling  `event.stopPropagation()`

```html run
<body onclick="alert(`the bubbling doesn't reach here`)">
  <button onclick="event.stopPropagation()">Click me</button>
</body>
```
