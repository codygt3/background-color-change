# background-color-change

## Simple Website Tutorial

Welcome to the Simple Website Tutorial! This guide will walk you through the steps to create a basic website using HTML, CSS, and JavaScript.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Step-by-Step Guide](#step-by-step-guide)
  - [1. Create the HTML File](#1-create-the-html-file)
  - [2. Create the CSS File](#2-create-the-css-file)
  - [3. Create the JavaScript File](#3-create-the-javascript-file)
  - [4. Link the CSS and JavaScript Files](#4-link-the-css-and-javascript-files)
  - [5. Open the HTML File in a Browser](#5-open-the-html-file-in-a-browser)
- [Things to Look Out For](#things-to-look-out-for)
- [Conclusion](#conclusion)

## Introduction

In this tutorial, you'll learn how to create a simple website with an HTML structure, styled with CSS, and interactivity added using JavaScript. By the end of this guide, you will have a basic understanding of how these three technologies work together to create a functional webpage.

## Project Structure

Create a project directory and set up the following file structure:
```plaintext
simple-website/
├── index.html
├── styles.css
└── script.js
```

## Step-by-Step Guide

### 1. Create the HTML File

Open your code editor and create a file named `index.html`. Add the following code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Change Background Color</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  Click the Button to Change the Background!
  <button id="colorButton">Change Color</button>

  <script src="script.js"></script>
</body>
</html>
```
### 2. Create the CSS File

Create a file named `styles.css` and add the following code to style your webpage:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: white;
  margin: 0;
  padding: 20px;
}

h1 {
  color: #333;
}

button {
  font-size: 20px;
  padding: 10px 20px;
  background-color: #4CAF50;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
```

### 3. Create the JavaScript File

Create a file named `script.js` and add the following code:
```js
const button = document.getElementById('colorButton');
const colors = ['red', 'blue', 'green', 'yellow', 'purple', 'orange'];

button.addEventListener('click', () => {
  const randomColor = colors[Math.floor(Math.random() * colors.length)];
  document.body.style.backgroundColor = randomColor;
});
```


### 4. Link the CSS and JavaScript Files

Ensure that the CSS and JavaScript files are linked correctly in your `index.html` file. The `<link>` tag for CSS should be inside the `<head>` section, and the `<script>` tag for JavaScript should be just before the closing `</body>` tag.

### 5. Open the HTML File in a Browser

Open your `index.html` file in a web browser to see your simple website in action. You should see a styled heading, a paragraph, and a button that displays an alert when clicked.

## Things to Look Out For

- Ensure the file paths in the `<link>` and `<script>` tags are correct.
- Use proper HTML structure and semantics.
- Keep your CSS organized and use meaningful class names.
- Avoid inline styles and JavaScript as much as possible for better maintainability.
- Test your website in different browsers to ensure compatibility.

## Stretch Goals
If you finish early, feel free to try out these additions to your website!

### 6. Make it a Header!
Enclose the "Hello World!" in an ``<h1>`` tag as shown here:
```<h1> Hello World! </h1>```
<br>
The full code should now look like this:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Change Background Color</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1>Click the Button to Change the Background!</h1>
  <button id="colorButton">Change Color</button>

  <script src="script.js"></script>
</body>
</html>
```


## Conclusion

Congratulations! You've created a simple website that changes the background color using HTML, CSS, and JavaScript. This is just the beginning – there are many more features and technologies to explore. Keep learning and experimenting to build more complex and dynamic websites.

Feel free to reach out if you have any questions or feedback. Happy coding!
