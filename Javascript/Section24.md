# Section 24 Introducing the world of the DOM
Document Object Model

### What is it
- The DOM is a Javascript representation of a webpage
- It's your JS "window" into the contents of a webpage
- It's just a bunch of objects that you can interact with via JS
![alt text](https://www.freecodecamp.org/news/content/images/2021/09/Document.jpg)
- The document object is our entry point into the world of the DOM. It contains representations of all the content on a page.

#### Selecting
- getElementById
- getElementsByTagName
- getElementsByClassName
- querySelector
- querySelectorAll : returns a Nodelist

#### Manipulating
- innerText
- textContent
- innerHTML
- getAttribute("href") == document.querySelector("sth").href
- setAttribute("some_attribute", "change")
- document.querySelector().style
- window.getComputedStyle(Element);

#### ClassList
