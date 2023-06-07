# Todo List Application

This is a simple todo list application that allows you to add and manage tasks.
You can create, mark as completed, and delete tasks using this application.

## JavaScript Functions

Here are some useful JavaScript functions used in this application:

```javascript
// Selecting an element on the page
const element = document.getElementById("ID");

// Select the content of an input
const inputValue = document.getElementById("ID").value;

// Select the content of span/headers/p/buttons/etc.
const innerText = document.getElementById("ID").innerText;

// Creates an HTML element
const newElement = document.createElement("element");

// "Watch" / "listen" for an action (click, change, keypress) and then perform the action you want in the function
element.addEventListener("click", function () {
  // do this
});

// Adds a class to an element
element.classList.add("class");

// Add the class if the class isn't present; remove the class if it is present
element.classList.toggle("class");

// Adds a type to an element
element.type = "type";

// Adds element as a child
parentElement.appendChild(elementToAdd);

// Removes child element
parentElement.removeChild(elementToRemove);
```

document.getElementById("ID") selecting an element on the page

document.getElementById("ID").value select the content of an input

document.getElementById("ID").innerText select the content of
span/headers/p/buttons/etc.

let element = document.createElement("element") creates HTML element

element.addEventListener("click", function(){ // do this }) "watch" / "listen"
for an action (click, change, keypress) and then performs the action you want in
the function

element.classList.add("class") adds class to element

element.classList.toggle("class") add the class if the class isn't present
removes the class if it is present

element.type = "type" adds a type to an element

element.appendChild(elementToAdd) adds element as a child

element.removeChild(elementToRemove) removes child element

### Steps to create a todo list

1. Create directory + create github repo
2. Create HTML + CSS + JS files
   1. Link CSS and JS
3. Add content to HTML
   1. Header
   2. Text input
   3. Button
   4. (empty) unordered list (ul)
   5. Add IDs to HTML elements to select them in CSS/JS
4. Add content to JS
   1. add event listener to the add task button
      1. select the text input and assigned to a variable
      2. checked if there was any content (if)
         1. if there was content: send text input content to addItem() function
   2. create addItem() function
      1. select the list (ul)
      2. create li element
         1. add class "item"
      3. create span element
         1. add class "task-content"
         2. add value that was passed to addItem() function to innerText of span
      4. create input element
         1. add class "checkbox"
         2. add type "checkbox"
         3. add event listener to input element
            1. listen for change
            2. toggle class "line-through" on taskContent element
      5. create delete button
         1. add class "delete-button"
         2. add "delete" to innerText of delete button
      6. add created elements (checkbox, textContent, deleteButton) to li
         element
      7. add item (li) to list (ul)
