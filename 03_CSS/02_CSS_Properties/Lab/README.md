
# CSS Landing Page Project Lab

In this lab, you will build a **landing page** for a fictional brand or product. The project is designed to help you practice CSS properties, including text styling, backgrounds, borders, box model settings, and layout properties.

### Project Structure

Create a folder named `LandingPageProject` with the following files:

```
LandingPageProject/
│
├── index.html
└── styles.css
```

### Lab Tasks

Each task is organized to guide you step-by-step through styling the landing page. Work through each section, writing CSS in the `styles.css` file and HTML in `index.html`.

---

## Task 1: Basic HTML Structure and Page Setup

1. **Set up HTML File**: Create an HTML structure in `index.html`.
   - Add the basic tags: `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`.
   - Set the title to "Welcome to [Brand Name]".

2. **Link CSS**: Link the `styles.css` file to `index.html` within the `<head>` section.
   ```html
   <link rel="stylesheet" href="styles.css">
   ```

3. **Page Layout**: Add the following elements:
   - **Header**: With an `<h1>` element for the brand name.
   - **Main Content Section**: Add a `<p>` tag to describe the brand/product.
   - **Image Section**: Use an `<img>` tag as a placeholder.
   - **Call-to-Action Button**: Add a `<button>` element with "Learn More" text.
   - **Footer**: Add a `<footer>` with some placeholder text like “© 2024 [Brand Name]”.

---

## Task 2: Text Styling

1. **Header Styling**: Use CSS to style the `<h1>` element.
   - Set the font color, size, and alignment to the center.
   - Choose a font-family and adjust the font-weight for a bold look.

   ```css
   h1 {
       color: #333;
       font-size: 36px;
       text-align: center;
       font-family: Arial, sans-serif;
       font-weight: bold;
   }
   ```

2. **Paragraph Styling**: Style the `<p>` element for the main content.
   - Set the font-size, color, and line-height for readability.
   - Use `text-align: justify` to align the paragraph.

3. **Button Styling**: Style the button to make it prominent.
   - Set a background color, text color, padding, and border-radius.
   - Change the font-size and add a `text-transform` property to capitalize text.

---

## Task 3: Background Styling

1. **Body Background**: Set a background color for the entire page.
   - Choose a light color to give a clean look.

   ```css
   body {
       background-color: #f4f4f9;
       margin: 0;
       font-family: Arial, sans-serif;
   }
   ```

2. **Header Background**: Add a background color to the header area.
   - Experiment with gradient backgrounds for a more modern look.

3. **Section Background with Image**: Set a background image for the main content section.
   - Choose a `background-size` of `cover` and `background-position` of `center`.

---

## Task 4: Border and Outline Styling

1. **Image Border**: Add a border around the image.
   - Set a color and adjust the border-width.
   - Use `border-radius` to make the image rounded.

2. **Button Outline on Focus**: Add an outline when the button is focused.
   - Use `outline` and `outline-offset` properties.

   ```css
   button:focus {
       outline: 2px solid #333;
       outline-offset: 2px;
   }
   ```

---

## Task 5: Box Model and Spacing

1. **Content Padding and Margins**: Apply padding and margin to main sections.
   - Set padding for the main content area to create space within.
   - Apply margin to the footer to separate it from other content.

2. **Image Spacing**: Add margin to the image for spacing.

3. **Button Padding**: Adjust padding to make the button larger.

---

## Task 6: Display and Layout Properties

1. **Center Aligning with Margin**: Center the main container using `margin: auto`.

2. **Flexbox Layout**: Use Flexbox to align the header, main content, and footer sections.

3. **Visibility Control**: Use `display: none` to temporarily hide an element (e.g., hide the footer).

4. **Z-Index on Header**: If adding a floating menu, use `z-index` to control stacking order.

---

## Final Task: Review and Refine

1. **Add Hover Effects**: Add a hover effect to the button for interactivity.
   ```css
   button:hover {
       background-color: #555;
       color: #fff;
   }
   ```

2. **Check Responsiveness**: Adjust properties as needed for mobile view.

---

### Completed Project Preview

After completing all tasks, your landing page should include a styled header, main content, image, and footer, with a visually appealing layout. Adjust any CSS as needed for a polished result.
