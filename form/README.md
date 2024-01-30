# File Tasks Project

## Basic Structure

### Project Overview

This project, named "File Tasks," aims to provide a structured set of HTML and CSS files for creating and styling articles and forms. The project is organized into different phases, each building upon the previous one. The repository is hosted on GitHub under the directory "alx-frontend-for-fun."

### Directory Structure

```
├── form
│   ├── 01-article.html
│   ├── 01-styles.css
│   ├── 02-article.html
│   ├── 02-styles.css
│   ├── 03-article.html
│   ├── 03-styles.css
│   ├── 04-article.html
│   ├── 04-styles.css
│   ├── 05-article.html
│   └── 05-styles.css
└── README.md
```

## Advanced Features

### 01-article.html and 01-styles.css

#### Comment Section

In the `01-article.html` file, create a new section named `post-comments` right after the `post` section. The section should contain a `header` with a level 2 heading (class `section-title`) that says "Leave a comment." Below the heading, add a paragraph with the text "All fields are required."

In `01-styles.css`, apply the following styles:
```css
/*** FORM ***/
/* Comment section
============================= */
/* Target post-comments class */
width: 80%;
margin: 10rem 0 0 auto;
padding-left: 7rem;

/* Target the section-title class inside the post-comments class */
font-variant: small-caps;
```

### 02-article.html and 02-styles.css

#### Basic Form Structure

From `01-article.html`, create `02-article.html`. In the comment section of the form:
- Create a fieldset with a legend ("Your personal information" - class `visually-hidden`).
- Inside the fieldset, create three divs with classes `form-group` and specific grid classes.
- Create a second fieldset with a legend ("Your comment" - class `visually-hidden`).

In `02-styles.css`, set the styles for all fieldsets:
```css
/* Basic form
============================= */
/* Target all fieldset */
display: flex;
flex-direction: column;
justify-content: flex-start;
border: none;
padding: 0 0 2rem;
```

### 03-article.html and 03-styles.css

#### Labels and Input Containers

From `02-article.html`, create `03-article.html`. In the form:
- Create labels and input containers for personal information and comment sections.

In `03-styles.css`, after the Tag list styles, add:
```css
/* Target all label */
cursor: pointer;
display: block;
white-space: nowrap;
font-size: 1.4rem;
padding: 0 0 .5rem;
```

### 04-article.html and 04-styles.css

#### Inputs

From `03-article.html`, create `04-article.html`. In the form:
- Add input fields for personal information and comment sections.

In `03-styles.css`, create `04-styles.css` with styles for input fields.

### 05-article.html and 05-styles.css

#### Help Messages

From `04-article.html`, create `05-article.html`. Add help messages next to input fields.

In `04-styles.css`, create `05-styles.css` with styles for form groups and help messages.

## Project Credits

This project is a part of the ALX Frontend Development for Fun initiative. The contributors include creative minds from Holberton School.

© 2024 File Tasks, made with ♥ by students at Holberton School.
```
