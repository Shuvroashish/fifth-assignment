1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Ans:
"getElementById" Selects one element by unique ID, returns Element or null, on the other hand "getElementsByClassName" Selects all elements by class, returns live HTMLCollection.
"querySelector" Selects first element by CSS selector, returns Element or null and "querySelectorAll" Selects all elements by CSS selector, returns non-live NodeList.


2. How do you create and insert a new element into the DOM?

Ans:
First
let newDiv = document.createElement("div");

Second
newDiv.textContent = "Hello, I am new here!";

then insert into the DOM 
document.body.appendChild(newDiv);


3.What is Event Bubbling and how does it work?

Ans:
Event Bubbling means when an event happens on an element, it first runs on that element, then moves up to its parent, then to the parent’s parent, until it reaches body or html tag.

First click on a child element.Then the event first runs on that child.Then it moves up to the parent. After that to the parent’s parent… all the way up to body or html tag.


4.What is Event Delegation in JavaScript? Why is it useful?

Ans:
Event Deligation means adding one listener to the parent Instead of adding event listeners to many child elements


It is usefull because-

.we don’t need separate listeners for every button/item.

.it Saves memory when we have lots of elements.



5.What is the difference between preventDefault() and stopPropagation() methods?


Ans:
preventDefault()  stop the browser’s default behavior on the other hand

stopPropagation() stop the event from moving to parent.