<!---Tags=["javascript", "introduction", "file"]--->

# Introduction to Javascript

## A small reminder

* HTML is the structure of your page, the skeleton
* CSS controls the style of the page
* JavaScript makes the page dynamic.

## What is Javascript ?

*JavaScript* is a **scripting language** used to create and control dynamic website content, for example: 
- autocomplete text suggestions
- interactive forms

JS is a language that can be typed directly into an HTML document, and web browsers will be able to understand them. 
Using JavaScript doesn’t require downloading any additional programs or compilers.

## Where do we write Javascript ?

1. Embedded JS in HTML file

You can add JavaScript code in an HTML document by employing  the HTML tag `<script>` that wraps around JavaScript code.
The `<script>` tag can be placed in the `<head>` section of your HTML, in the `<body>` section, or after the `</body>` close tag, 
depending on when you want the JavaScript to load.

Usually the JavaScript code is added between the `<head>` tags, signalling the browser to run the JavaScript script 
before loading in the rest of the page. 

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Today's Date</title>
    <script>
        let d = new Date();
        alert("Today's date is " + d);
    </script>
    </head>
    <body>
    </body>
</html>
```

2. External JS file

The benefits of using a separate JavaScript file :

- Code more understandable 
- Easier maintenance
- Pages load more quickly
- Can run the same JavaScript on several pages in a web site

Usually the scipt tag for the external JS file is placed at the end of the body section, so the web page itself will have loaded before the script is read. 

```html
<!DOCTYPE html>
<html>
    <body>

    <script src="script.js"></script>
    </body>
</html>
```

### JS and  Object Oriented Programming (OOP)

1. What is an object ?

Objects act just like real life objects.  
Objects have properties and methods.

> Example :  A lamp has properties  -->  height,width, brightness 
>                               has methods (an action) --> to shine

JavaScript gives you the ability to **make your own objects**

2. Creating an object

The simplest way is to use the `new` operator.




