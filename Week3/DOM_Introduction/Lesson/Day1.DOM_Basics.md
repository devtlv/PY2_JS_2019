<!--Tags=["DOM","JS", "tree"]-->

# DOM Basics

## 1. A small reminder
* **HTML** is the structure of your page, the skeleton
* **CSS** controls the style of the page
* **JavaScript** makes the page dynamic.
* **The browser**  is a program that interprets HTML and CSS and renders the structure and  style into the page that you see.
It creates a *representation* of the document called  **Document Object Model. **
This model allows JavaScript to access the text content and elements of the website document as **objects.**

## 2  What is the DOM ?
The **Document Object Model** : the **DOM** makes websites interactive. 
It  allows a programming language, here JS,  to manipulate the content, structure, and style of a website.
It represents all page content as **objects** that can be modified.

In your browser, when you click on *Inspect* and on the *Arrow* you can see and have access to the DOM.

## 3. The document object
The `document` object is a built-in object that has many properties and methods that we can use to access and modify websites.
Take a look at the document object inside the console. 

![document](https://user-images.githubusercontent.com/30896388/68525135-24fce880-02d7-11ea-97de-c893fc836db5.png)

![document](https://user-images.githubusercontent.com/30896388/68525136-25957f00-02d7-11ea-881f-97b9e837af5a.png)


## 4. The DOM Tree

![document](https://www.researchgate.net/profile/Jian_Chang4/publication/254002847/figure/fig1/AS:298235726974978@1448116346303/Example-of-DOM-Node-Tree.png)

Every tree node is an **object**.

* Tags are **element nodes** and form the tree structure: 
* `<html>` is at the root,
* `<head>` and `<body>` are its children.
* The text inside elements are **text nodes**. A text node contains only a string. It may not have children and is always a leaf of the tree.

Let's look at the [DOM VIEWER](http://software.hixie.ch/utilities/js/live-dom-viewer/)

