 Answer the following questions: 

1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?


Answer: 

The difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll:

a. One element by ID is returned by getElementById
b. getElementsByClassName('class') returns an HTMLCollection (live) containing every element with class.
c. querySelector('selector') Using any CSS selector, returns the first matching element.
d. querySelectorAll('selector') Returns a static NodeList with all matching elements.


2. How do you **create and insert a new element into the DOM**?

Answer: 

Steps for creating and insert a new element to the DOM Below:

 Use document.createElement('tagName') to create an element.

 Set innerHTML, text, or attributes.

 Use appendChild, insertBefore, or append to add it to the DOM.

 // 1. Create the element const newDiv = document.createElement('div');

 // 2. Include fresh content Div.textContent = "Hello, World!"; new Div.className = "greeting";

 // 3. Add to the document's DOM. body.appendChild(newDiv); // appends to the body's end

3. What is **Event Bubbling** and how does it work?

Answer: 

When an event occurs on a child element,That time it first affects the target element and gradually moves towards the parent element until it reaches the root. This phenomenon is called event bubbling.



4. What is **Event Delegation** in JavaScript? Why is it useful?

Answer: 

To handle events on child elements, assign a single listener to a parent.

Effective because it works with dynamically added elements and saves memory.

For Example:

parent.addEventListener('click', e => { 
if(e.target.tagName === 'LI') console.log('LI clicked'); 
});


5. What is the difference between **preventDefault() and stopPropagation()** methods?

Answer: 

preventDefault() Stops the browser's default actions (such as navigating links or submitting forms).

 stopPropagation() Prevents the event from disintegrating into its original components.

