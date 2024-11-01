
# HTML Basics - An In-Depth Guide

HTML, or **HyperText Markup Language**, is the standard language used to create web pages. It provides structure to web content, enabling text, images, videos, links, and other elements to be displayed in a browser.

---

## 1. What is HTML?

HTML stands for **HyperText Markup Language**. It is a markup language that web browsers use to interpret and render text, images, videos, and other content on a web page. HTML uses a series of elements, known as tags, to structure and format content.

---

## 2. Setting Up Your First HTML File

To begin working with HTML, we typically create a file named `index.html`. The `index.html` file is often used as the main entry point for a website. Web servers automatically recognize it as the homepage, making it a standard naming convention for starting a project.

### Creating `index.html` in VS Code

1. **Open Visual Studio Code (VS Code)**: This code editor is highly recommended for working with HTML, as it offers extensions, preview options, and helpful shortcuts.
2. **Create a New File**: Go to `File` > `New File`, or press `Ctrl+N` (Windows/Linux) or `Cmd+N` (Mac).
3. **Save as index.html**: Go to `File` > `Save As`, and name your file `index.html`.

---

## 3. Basic HTML Document Structure

Below is a simple HTML document that you can use in your `index.html` file:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First HTML Page</title>
  </head>
  <body>
    <h1>Welcome to HTML</h1>
    <p>This is a basic HTML document structure.</p>
  </body>
</html>
```

### Explanation of the HTML Document Structure

- **`<!DOCTYPE html>`**: Declares the document type and version of HTML being used (HTML5 in this case).
- **`<html>`**: The root element that wraps all content of the web page.
- **`<head>`**: Contains meta-information about the document, including its title and links to stylesheets and scripts.
- **`<title>`**: Specifies the title of the web page that appears on the browser tab.
- **`<body>`**: Contains the content of the page, such as headings, paragraphs, images, and links.

---

## 4. Using Visual Studio Code (VS Code) for HTML

### HTML Shortcuts in VS Code

- **Emmet Abbreviation**: In VS Code, typing `!` and pressing `Tab` will expand to the HTML boilerplate, which includes `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>` tags. This is a quick way to start an HTML file.
- **Auto-complete for Tags**: As you type, VS Code suggests tags and closes them automatically.

### Installing a Live Server Extension

1. **Install Live Server**: In the Extensions sidebar of VS Code, search for "Live Server" and install it. This extension allows you to see your changes instantly in the browser.
2. **Start the Live Server**: Right-click your `index.html` file and select `Open with Live Server`. This will open your file in a browser and auto-refresh whenever you save changes.

### Basic Workflow with VS Code and Live Server

- **Edit and Save**: Make edits in your `index.html` file, then press `Ctrl+S` (Windows/Linux) or `Cmd+S` (Mac) to save.
- **Auto-Reload**: The browser automatically refreshes with the latest changes.

---

## 5. Common HTML Tags and Elements

### 5.1 Headings

HTML provides six levels of headings, from `<h1>` to `<h6>`. `<h1>` is the largest and most important heading, while `<h6>` is the smallest.

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
```

### 5.2 Paragraphs

The `<p>` tag is used to define paragraphs of text.

```html
<p>This is a paragraph in HTML.</p>
```

### 5.3 Links

Links are created using the `<a>` tag with the `href` attribute.

```html
<a href="https://www.example.com">Visit Example</a>
```

### 5.4 Images

Images are embedded using the `<img>` tag with the `src` attribute, which specifies the image URL.

```html
<img src="image.jpg" alt="Description of image" />
```

### 5.5 Lists

HTML provides ordered and unordered lists.

- **Unordered List**: Created using `<ul>` and `<li>` tags.

  ```html
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
  ```

- **Ordered List**: Created using `<ol>` and `<li>` tags.

  ```html
  <ol>
    <li>First item</li>
    <li>Second item</li>
  </ol>
  ```

### 5.6 Tables

Tables are created using `<table>`, `<tr>`, `<th>`, and `<td>` tags.

```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
</table>
```

### 5.7 Divisions and Spans

- **`<div>`**: A block-level element used to group other elements for styling and layout.
- **`<span>`**: An inline element used to style a part of text or a small section of the page.

```html
<div class="container">
  <span>Inline styled text</span>
</div>
```

---

## 6. HTML Attributes

Attributes provide additional information about HTML elements. They are added inside the opening tag.

### Common Attributes

- **id**: Assigns a unique identifier to an element.
- **class**: Classifies elements for styling.
- **style**: Applies inline CSS styles to an element.
- **alt**: Provides alternate text for images.

Example:

```html
<p id="intro" class="text-primary" style="color: blue;">This is a paragraph.</p>
```

---
