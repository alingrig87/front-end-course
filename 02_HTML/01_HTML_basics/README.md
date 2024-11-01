# HTML Basics

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
<html lang="en">
  <head>
    <meta charset="UTF-8" />
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

## 4. Comments in HTML

### Purpose of HTML Comments

Comments in HTML are notes or explanations added to the code to clarify structure, purpose, or to temporarily disable elements during testing. Comments are ignored by the browser and do not appear on the webpage, but they are helpful for developers.

- **Syntax**: Use `<!-- comment here -->` to create a comment.

### Example:

```html
<!-- This comment explains the purpose of the content below -->
<div class="notice">
  <h2>Important Notice</h2>
  <p>
    All services will be temporarily unavailable on Saturday for maintenance.
  </p>
</div>
```

### Using Comment Shortcuts in VS Code

1. **Emmet Shortcut**: In VS Code, type `c` and press `Tab` to add a new comment line (`<!-- -->`).
2. **Keyboard Shortcut (Ctrl + /)**: Press **Ctrl + /** (Windows/Linux) or **Cmd + /** (Mac) to comment or uncomment selected code. This shortcut automatically wraps selected text in `<!-- -->`.

---

## 5. Using Visual Studio Code (VS Code) for HTML

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

## 6. Common HTML Tags and Elements

### 6.1 Headings

HTML provides six levels of headings, from `<h1>` to `<h6>`. `<h1>` is the largest and most important heading, while `<h6>` is the smallest.

```html
<h1>Exploring Ancient Civilizations</h1>
<h2>The Egyptian Civilization</h2>
<h3>Key Contributions and Discoveries</h3>
```

### 6.2 Paragraphs

The `<p>` tag is used to define paragraphs of text.

```html
<p>
  The Egyptian civilization is known for its monumental architecture, art, and
  advanced knowledge in various fields.
</p>
```

### 6.3 Links

Links are created using the `<a>` tag with the `href` attribute.

```html
<a href="https://www.history.com/topics/ancient-egypt"
  >Learn more about Ancient Egypt</a
>
```

### 6.4 Images

Images are embedded using the `<img>` tag with the `src` attribute, which specifies the image URL.

```html
<img src="egypt_pyramid.jpg" alt="A pyramid in Egypt" />
```

### 6.5 Lists

HTML provides ordered and unordered lists.

- **Unordered List**: Created using `<ul>` and `<li>` tags.

  ```html
  <ul>
    <li>Pyramids of Giza</li>
    <li>Great Sphinx of Giza</li>
    <li>Temple of Karnak</li>
  </ul>
  ```

- **Ordered List**: Created using `<ol>` and `<li>` tags.

  ```html
  <ol>
    <li>Discover fire</li>
    <li>Develop tools</li>
    <li>Build monumental structures</li>
  </ol>
  ```

### 6.6 Tables

Tables are created using `<table>`, `<tr>`, `<th>`, and `<td>` tags.

<table>
  <tr>
      <th>Carte</th>
      <th>Autor</th>
      <th>Anul Publicării</th>
  </tr>
  <tr>
      <td>Ion</td>
      <td>Liviu Rebreanu</td>
      <td>1920</td>
  </tr>
  <tr>
      <td>Enigma Otiliei</td>
      <td>George Călinescu</td>
      <td>1938</td>
  </tr>
  <tr>
      <td>Moromeții</td>
      <td>Marin Preda</td>
      <td>1955</td>
  </tr>
  <tr>
      <td>Ultima noapte de dragoste, întâia noapte de război</td>
      <td>Camil Petrescu</td>
      <td>1930</td>
  </tr>
  <tr>
      <td>Baltagul</td>
      <td>Mihail Sadoveanu</td>
      <td>1930</td>
  </tr>
</table>

### 6.7 Divisions and Spans

- **`<div>`**: A block-level element used to group other elements for styling and layout.
- **`<span>`**: An inline element used to style a part of text or a small section of the page.

```html
<div class="ai-info">
  <span>ChatGPT</span> is an advanced AI language model developed by OpenAI,
  designed to understand and generate human-like text.
</div>
```

---

## 7. HTML Attributes

Attributes provide additional information about HTML elements. They are added inside the opening tag.

### Common Attributes

- **id**: Assigns a unique identifier to an element.
- **class**: Classifies elements for styling.
- **style**: Applies inline CSS styles to an element.
- **alt**: Provides alternate text for images.

Example:

```html
<p id="intro" class="highlight" style="color: green;">
  Ancient civilizations left a lasting impact on history.
</p>
```

#### Best Practices for Naming HTML Classes and IDs

Proper naming conventions for classes and IDs improve the readability and maintainability of your code. Here are some best practices to follow, with examples.

---

#### 1. Use Descriptive and Clear Names

Make sure that class and ID names clearly describe the purpose or content of the element. This makes your code more understandable and easier to navigate.

**Examples of Good Practice**:

```html
<div class="navigation-bar">
  <!-- Class for the navigation bar -->
  <div id="main-header">
    <!-- ID for the main header section -->
    <div class="product-list"><!-- Class for a list of products --></div>
  </div>
</div>
```

**Avoid Ambiguous Names**:

```html
<div class="nb">
  <!-- Too vague; it's unclear what this means -->
  <div id="mh"><!-- Ambiguous; hard to understand without context --></div>
</div>
```

---

#### 2. Use "kebab-case" for Classes and "camelCase" for IDs

A common convention is to use "kebab-case" (lowercase words separated by hyphens) for classes and "camelCase" (words without spaces or hyphens, capitalizing each word after the first) for IDs.

**Examples**:

```html
<div class="main-content">
  <!-- kebab-case for classes -->
  <div id="mainContent"><!-- camelCase for IDs --></div>
</div>
```

---

#### 3. Avoid Cryptic Abbreviations

Use abbreviations only if they are widely understood (e.g., "btn" for "button"). Avoid using abbreviations that might be confusing for others.

**Examples of Good Practice**:

```html
<div class="submit-button">
  <!-- Clear and descriptive -->
  <div class="btn-primary">
    <!-- Abbreviation "btn" is widely recognized for button -->
  </div>
</div>
```

**Avoid Using Unclear Abbreviations**:

```html
<div class="sbmt-btn">
  <!-- Hard to understand; avoid using complex abbreviations -->
  <div id="cont-list">
    <!-- Unclear if "cont" means "content" or "container" -->
  </div>
</div>
```

---

#### 4. Prefix Class Names with Context

If a class is used within a specific section or component, prefix the name to indicate context. This helps avoid conflicts and keeps styles scoped to the intended area.

**Examples**:

```html
<div class="header-logo">
  <!-- Logo within the header -->
  <div class="footer-links"><!-- Links specific to the footer --></div>
</div>
```

---

#### 5. Keep Class and ID Names Short but Meaningful

While it's essential to avoid overly long names, don't compromise clarity for brevity. Strive for short, descriptive names.

**Examples of Good Practice**:

```html
<div class="user-profile">
  <!-- Clear and concise -->
  <div id="searchResults"><!-- Short but meaningful --></div>
</div>
```

**Avoid Overly Long Names**:

```html
<div class="main-header-navigation-bar-logo">
  <!-- Too long, makes code harder to read -->
  <div id="profile-settings-section-links-list"><!-- Overly complex --></div>
</div>
```

---

#### 6. Use Classes for Styling, IDs for JavaScript

Use classes primarily for styling, as classes allow for multiple elements to share the same styling. Reserve IDs for elements that need unique identification, such as for JavaScript manipulation.

**Examples**:

```html
<div class="card">
  <!-- Class for styling multiple cards -->
  <div id="uniqueButton">
    <!-- ID for a unique button, used in JavaScript -->
  </div>
</div>
```

---
