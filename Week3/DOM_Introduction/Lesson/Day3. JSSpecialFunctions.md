# JS Functions

## setTimeout()

Allows us to run a function once after the interval of time.

```javascript
function sayHi(phrase, who) {
  alert( phrase + ', ' + who );
}

setTimeout(sayHi, 1000, "Hello", "John"); //  calls sayHi() after one second --> Hello, John
```

## clearTimeout() to prevent the function to run

Because calling a timer function schedules an action, that action can also be cancelled before it gets executed.
A call to setTimeout returns a timer “ID” and you can use that timer ID with a clearTimeout call to cancel that timer.

```html run
<button onclick="myFunction()">Try it</button>
<button onclick="myStopFunction()">Stop the alert</button>

<script>
var myVar;

function myFunction() {
  myVar = setTimeout(function(){ alert("Hello") }, 3000);
}

function myStopFunction() {
  clearTimeout(myVar);
}   // to prevent the first function to execute
</script>
```

## setInterval()
Allows us to run a function repeatedly, starting after the interval of time, then repeating continuously at that interval.
``` javascript
setInterval(function() {
      // Do something every 5 seconds
}, 5000);
```

## clearInterval()

Because calling a timer function schedules an action, that action can also be cancelled before it gets executed.
A call to setInterval returns a timer “ID” and you can use that timer ID with a clearTimeout call to cancel that timer.

```html run
<p id="demo"></p>

<button onclick="myStopFunction()">Stop time</button>

<script>
var myVar = setInterval(myTimer, 1000);

function myTimer() {
  var d = new Date();
  var t = d.toLocaleTimeString();
  document.getElementById("demo").innerHTML = t;
}

function myStopFunction() {
  clearInterval(myVar);
}
</script>
```




