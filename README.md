# Booksky

This project is a dynamic and user-friendly book management application built using HTML, CSS, and JavaScript. It allows users to add and delete books, making it easier to manage a collection of books.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [HTML Code](#html-code)

## Introduction
The Booksky project provides a sleek and intuitive interface for managing a collection of books. Users can easily add new books and delete existing ones, all through a user-friendly interface.

## Features
- **Responsive Design**: Adapts to various screen sizes for an optimal viewing experience.
- **Add Books**: Allows users to add new books with titles, authors, and descriptions.
- **Delete Books**: Provides functionality to remove books from the list.
- **Popup Form**: Includes a popup form for adding books, enhancing the user experience.

## Getting Started
1. Clone the repository from GitHub.
2. Ensure you have an HTML viewer or a web browser to open the `index.html` file.
3. Open `index.html` in your preferred browser to use the Booksky application.

## Usage
- **Add Book**: Click the "+" button to open the popup form, enter the book details, and click "ADD" to add the book to the list.
- **Delete Book**: Click the "delete" button next to a book to remove it from the list.

## HTML Code
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Booksky</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="navbar">
        <h1>Booksky</h1>
    </div>
    <div class="container">
        <div class="book-container">
            <h2>Rich Dad Poor Dad</h2>
            <h5>Robert</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores magni libero explicabo perspiciatis in quidem necessitatibus hic, consequatur suscipit officiis.</p>
            <button onclick="deletebook(event)">delete</button>
        </div>
    </div>
    <div class="popup-overlay"></div>
    <div class="popup-box">
        <h2>Add book</h2>
        <form>
            <input type="text" placeholder="Book Title" id="book-title-input">
            <input type="text" placeholder="Book Author" id="book-author-input">
            <textarea placeholder="Short Description" id="book-description-input"></textarea>
            <button id="add-book">ADD</button>
            <button id="cancel-popup">CANCEL</button>
        </form>
    </div>
    <button class="add-button" id="add-popup-button">+</button>
    <script src="script.js"></script>
</body>
</html>
