# CSS Basics

CSS (Cascading Style Sheets) is the language used to style HTML documents. It allows you to control the layout, colors, fonts, and other visual aspects of a webpage.

---

## Linking CSS to HTML

There are three main ways to include CSS in an HTML document:

1. **Inline CSS**: Styles are added directly within an HTML element using the `style` attribute.

   ### Example:

   ```html
   <p style="color: blue; font-size: 18px;">
   	This is an inline-styled paragraph.
   </p>
   ```

2. **Internal CSS**: Styles are included within a `<style>` tag inside the `<head>` section of an HTML document.

   ### Example:

   ```html
   <html>
   	<head>
   		<style>
   			p {
   				color: green;
   				font-size: 20px;
   			}
   		</style>
   	</head>
   	<body>
   		<p>This is an internally-styled paragraph.</p>
   	</body>
   </html>
   ```

3. **External CSS**: Styles are written in a separate `.css` file and linked using the `<link>` tag in the HTML `<head>`.

   ### Example:

   ```html
   <link rel="stylesheet" href="styles.css" />
   ```

   #### `styles.css` file:

   ```css
   p {
   	color: red;
   	font-size: 22px;
   }
   ```

---

## CSS Syntax

The CSS syntax consists of selectors and declaration blocks:

```css
selector {
	property: value;
}
```

- **Selector**: Specifies the HTML elements to be styled (e.g., `p` for paragraphs).
- **Property**: Defines the aspect to style, such as `color` or `font-size`.
- **Value**: Specifies the style setting for the property.

### Example

```css
h1 {
	color: blue;
	font-size: 24px;
}
```

---

## Common CSS Properties and Examples

### 1. Selectors

- **Tag Selector**: Targets all elements of a specific HTML tag.

  ```css
  p {
  	color: black;
  }
  ```

- **Class Selector**: Targets elements with a specific class attribute, prefixed with a period (`.`).

  ```css
  .highlight {
  	background-color: yellow;
  }
  ```

- **ID Selector**: Targets an element with a unique ID, prefixed with a hashtag (`#`).
  ```css
  #header {
  	font-weight: bold;
  }
  ```

### 2. Text and Font Properties

- **`color`**: Sets the color of the text.

  ```css
  p {
  	color: #333333;
  }
  ```

- **`font-size`**: Sets the size of the font.

  ```css
  h2 {
  	font-size: 24px;
  }
  ```

- **`text-align`**: Aligns text horizontally (e.g., `left`, `center`, `right`).

  ```css
  .centered {
  	text-align: center;
  }
  ```

- **`font-weight`**: Sets the weight of the font (e.g., `normal`, `bold`).
  ```css
  .bold-text {
  	font-weight: bold;
  }
  ```

### 3. Background and Border Properties

- **`background-color`**: Sets the background color of an element.

  ```css
  .highlighted {
  	background-color: lightblue;
  }
  ```

- **`border`**: Defines the border around an element (width, style, color).

  ```css
  .box {
  	border: 2px solid #000;
  }
  ```

- **`background-image`**: Sets an image as the background.
  ```css
  body {
  	background-image: url('background.jpg');
  }
  ```

### 4. Box Model Properties

- **`padding`**: Adds space inside the element’s border.

  ```css
  .container {
  	padding: 10px;
  }
  ```

- **`margin`**: Adds space outside the element’s border.

  ```css
  .spaced {
  	margin: 20px;
  }
  ```

- **`width`** and **`height`**: Define the size of an element.
  ```css
  .fixed-size {
  	width: 100px;
  	height: 200px;
  }
  ```

### 5. Shadows

- **`box-shadow`**: Adds shadow around an element.

  ```css
  .shadow-box {
  	box-shadow: 2px 2px 5px grey;
  }
  ```

- **`text-shadow`**: Adds shadow to text.
  ```css
  h1 {
  	text-shadow: 1px 1px 2px black;
  }
  ```

---

## Practical Example Combining Styles

Here's an example of a styled HTML page using both internal and external CSS:

### HTML

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<link rel="stylesheet" href="styles.css" />
		<style>
			.title {
				color: darkblue;
				text-align: center;
			}
		</style>
	</head>
	<body>
		<h1 class="title">Welcome to My Styled Page</h1>
		<p class="highlight">This is a highlighted paragraph.</p>
		<div id="header" class="shadow-box">Header with Shadow</div>
	</body>
</html>
```

### CSS (styles.css)

```css
body {
	font-family: Arial, sans-serif;
	background-color: #f0f0f0;
}

.highlight {
	background-color: yellow;
	padding: 5px;
}

#header {
	font-size: 24px;
	font-weight: bold;
	margin: 10px;
}
```
