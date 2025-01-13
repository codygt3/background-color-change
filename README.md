# background-color-change

## Simple Website Tutorial

Welcome to the Simple Website Tutorial! This guide will walk you through the steps to create a basic website using HTML, CSS, and JavaScript.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Step-by-Step Guide](#step-by-step-guide)
  - [1. Create the HTML File](#1-create-the-html-file)
  - [2. Add a Title](#2-add-a-title)
  - [3. Add a button](#3-add-a-button)
  - [4. Create the CSS File](#4-create-the-css-file)
  - [5. Change Background Color](#5-change-background-color)
  - [6. Change Title Color](#6-change-title-color)
  - [7. Change Colors Using Hex Numbers](#7-change-color-using-hex-numbers)
  - [8. Create Styling for your Button](#8-create-styling-for-your-button)
- [Things to Look Out For](#things-to-look-out-for)
- [Conclusion](#conclusion)

## Introduction

In this tutorial, you'll learn how to create a simple website that allows you to change the background color through a button press using HTML structure, styled with CSS, and some aspects of JavaScript.

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

  <script src="script.js"></script>
</body>
</html>
```

### 2. Add a Title

Add in the text for your website:

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
  <h1>Click the Button to Change the Background!</h1>  <----

  <script src="script.js"></script>
</body>
</html>
```

### 3. Add a button

Add in the button for your website:

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
  <button id="colorButton">Change Color</button>   <----

  <script src="script.js"></script>
</body>
</html>
```

### 4. Create the CSS File

Create a file named `styles.css` and add the following code to style your webpage:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: white;
  margin: 0;
  padding: 20px;
}
```

### 5. Change Background Color

Add in styling for the body tag and change the color to blue:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: blue;    <----
  margin: 0;
  padding: 20px;
}
```

### 6. Change Title Color

Add in styling for your title you created and change the color to red:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: blue;
  margin: 0;
  padding: 20px;
}

h1 {
  color: red;    <----
}
```

### 7. Change Colors Using Hex Numbers

Using the following website: https://htmlcolorcodes.com/ 
Change the body and title to your favorite colors using hex numbers:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: #62F1A7;    <----
  margin: 0;
  padding: 20px;
}

h1 {
  color: #628EF1;    <----
}
```

### 8. Create Styling for your Button

Add in styling for the button you created and customize it:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: #62F1A7;
  margin: 0;
  padding: 20px;
}

h1 {
  color: #628EF1;
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

## Stretch Goals
Lets work on JavaScript!

### 3. Create the JavaScript File

Create a file named `script.js` and add the following code. Feel free to add your own list of colors:

```js
const button = document.getElementById('colorButton');
const colors = ['red', 'blue', 'green', 'yellow', 'purple', 'orange'];

button.addEventListener('click', () => {
  const randomColor = colors[Math.floor(Math.random() * colors.length)];
  document.body.style.backgroundColor = randomColor;
});
```

### 5. Open the HTML File in a Browser

Open your `index.html` file in a web browser to see your simple website in action. You should see a styled heading, a paragraph, and a button that displays an alert when clicked.

## Things to Look Out For

- Ensure the file paths in the `<link>` and `<script>` tags are correct.
- Use proper HTML structure and semantics.
- Keep your CSS organized and use meaningful class names.
- Avoid inline styles and JavaScript as much as possible for better maintainability.
- Test your website in different browsers to ensure compatibility.

## Conclusion

Congratulations! You've created a simple website that changes the background color using HTML, CSS, and JavaScript. This is just the beginning – there are many more features and technologies to explore. Keep learning and experimenting to build more complex and dynamic websites.

Feel free to reach out if you have any questions or feedback. Happy coding!
