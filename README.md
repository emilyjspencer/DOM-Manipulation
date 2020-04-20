# NOTES

* The **DOM** is an API (Application Programming Interface)

* **APIs** allow you to use their built-in functions to make changes to the HTML document.
Using the DOM allows us to build web pages that change and react when the user does something

* When the HTML document runs in the browser, it becomes part of the DOM called the document object.

* The Dom's API structure is **hierarchical**.
The HTML elements within the document object are all connected to each other.
Any HTML element that is inside another is a **child element**.
The outer element is the **parent**

* JavaScript can be used to access, change, add or remove HTML elements
* The DOM is **case sensitive**

### DOM methods and properties

**Methods**

There are various methods that can be used, but these need to be called on the document.
Doing so tells the browser that we want to access the API.

**Selection methods:**

**getElementById()**
**getElementsByClassName()**
**getElementsByTagName()**
**getElementsByName()**

**Creating and adding methods:**

**createElement()** - makes a new element.
We can us JavaScript to assign the element to a variable and then use the innerHTML property to set 
the content of the new element

**appendChild()** - allows you to add a new HTML element to an existing HTML element

```html 
<script>
  var newDiv = document.createElement("div");
  newDiv.innerHTML = "hello";
  document.body.appendChild(newDiv);
</script>
```

**Deletion methods**

**removeChild()** - is used to remove child elements 

```html
document.getElementById("buttonone").removeChild(this);
```

* The **this** keyword refers to the HTML element that was used to call the function

**getAttribute()**

**setAttribute()**

**Properties**

**innerHTML** property can be used to access or change the content of an HTML element

```html
var showStar = document.getElementById("list");
alert(showStar.innerHTML);
```

**Node Methods**

**node.childNodes**
**node.firstChild**
**node.lastChild**
**node.parentNode**
**node.nextSibling**
**node.previousSibling**

**Local Storage**

* The **localStorage** API can be used to save information submitted.
localStorage allows you to save information in the browser even if the page is refreshed or closed.

* localStorage is a collection of functions.

* Tell the browser that you want to use localStorage by typng the localStorage keyword and giving a name
to the information you want to store

```html
localStorage.storageName = "stuff";
```

* To **remove** a piece of information from localStorage, set to an empty string:

```html
localStorage.storageName = "";
``` 
