
Question-1: What are the different ways to select an element in the DOM?
Answer:
document.getElementById("id");
document.getElementsByClassName("class");
document.getElementsByTagName("tag");
document.querySelector(".class or #id or tag");
document.querySelectorAll(".class or tag");
document.getElementsByName("name");
Question-2: What is the difference between innerHTML, innerText, and textContent ?
Answer:
The main differences between innerHTML, innerText, and textContent lie in how they handle content and performance. innerHTML retrieves or sets the HTML content within an element, including any HTML tags, allowing for manipulation of the markup itself. It is useful when you need to get or set complex HTML structures. On the other hand, innerText only retrieves or sets the visible text content of an element, excluding any HTML tags, and it does not account for hidden text (such as text hidden with CSS properties like display: none). It also triggers a reflow of the page layout, making it slower compared to textContent. In contrast, textContent retrieves or sets all the text inside an element, including hidden text, but does not parse HTML tags, offering a faster alternative to innerText as it does not require reflow. Therefore, textContent is ideal when dealing with plain text, while innerHTML is more appropriate for handling and updating HTML structure, and innerText is better for manipulating visible text content.
Question-3: What is event delegation in the DOM?
Answer:
A technique where you attach a single event listener to a parent element, allowing it to handle events triggered on its child elements, instead of adding separate listeners to each child element.
Question-4: What is event bubbling in the DOM?
Answer:
Event bubbling is a process in the DOM where an event, triggered on a target element, propagates upward through its ancestor elements, such as parents, grandparents, and so on. The event first triggers the listener on the target element, and then bubbles up to its parent elements, triggering their event listeners in turn. This allows parent elements to handle events for their child elements without needing separate listeners on each child. Event bubbling can be stopped using event.stopPropagation() if you don't want the event to continue propagating up the DOM tree.
Question-5: How do you create, add, and remove elements using JavaScript?
Answer:
To create an element, you can use the document.createElement() method. To add an element, you can use the appendChild() method or the insertBefore() method. To remove an element, you can use the removeChild() method.
