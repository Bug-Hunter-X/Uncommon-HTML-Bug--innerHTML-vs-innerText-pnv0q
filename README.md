# Uncommon HTML Bug: innerHTML vs innerText

This repository demonstrates a subtle but important difference between using `innerHTML` and `innerText` in JavaScript when manipulating HTML elements.  Incorrect use of `innerHTML` can lead to unexpected behavior and security vulnerabilities.

## The Bug
The `bug.html` file shows a common mistake where `innerHTML` is used to change the content of a div element.  In many cases, `innerText` is safer and more appropriate.

## The Solution
The `bugSolution.html` file demonstrates the correct approach using `innerText` to modify the div element's content.

## Key Differences
* **innerHTML:**  Parses the string as HTML.  This can be powerful but also dangerous if the string contains user-supplied data (potential XSS vulnerability).
* **innerText:**  Sets the plain text content of the element, ignoring HTML tags.  Generally safer for simple text updates.