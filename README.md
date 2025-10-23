# CodeConnect - Project Upload Page

This project is a front-end UI for "CodeConnect," a conceptual platform for developers to share projects. The page is a complete, interactive form that allows a user to "publish" a new project, including uploading an image, adding a description, and assigning tags.

Unlike a static site, the primary goal of this project was to practice **modern, asynchronous JavaScript (ES6+)** to create a dynamic user experience and simulate server interactions.

### 💻 Tech Stack
* **HTML5:** For the semantic structure of the form.
* **CSS3:** For all styling and layout.
* **JavaScript (ES6+):** For all client-side interactivity.

### ✨ Key JavaScript Features
This project was built to demonstrate proficiency in core JavaScript concepts:

* **Async Image Preview:** Uses `FileReader` wrapped in a `Promise` to read a user's image file and display a live preview *before* submission.
* **Async Tag Validation:** Simulates an API call (using `setTimeout` and `async/await`) to "validate" if a tag exists in a hardcoded list before adding it to the UI.
* **Dynamic DOM Manipulation:** Tags are dynamically created (`createElement`), added (`appendChild`), and removed (`removeChild`) from the DOM in real-time.
* **Promise-Based API Simulation:** The "Publish" button triggers an `async` function that returns a `Promise`. This promise uses `Math.random()` to simulate a real network request that can either succeed (`resolve`) or fail (`reject`).
* **Error Handling:** Uses `try...catch` blocks to gracefully handle potential errors, such as a failed "publication" or tag validation.
* **Event Delegation:** The "remove tag" feature uses a single event listener on the parent tag list (`<ul>`) for better performance and efficiency.
* **Form Control:** Includes a "Discard" button that properly resets the form, the tag list, and the image preview to their default states.
