# HTML Basics - European Cities Exercise 

---

## Emmet Tips for HTML Structure

Emmet is a powerful toolkit integrated into many code editors (such as Visual Studio Code) that helps you quickly write HTML and CSS. Here are some useful Emmet shortcuts for this exercise:

1. **Basic HTML Structure**: Type `!` and press `Tab` to create the basic HTML5 document structure.

2. **Nested Elements**: Type `div>h2+img+p` and press `Tab` to create a `section` element containing an `h2`, an `img`, and a `p` element, all nested inside it.

3. **Lists**: Type `ul>li*3` and press `Tab` to create an unordered list with three list items. Replace `ul` with `ol` for an ordered list.

4. **Classes and IDs**: Type `div#container.section` and press `Tab` to create a `div` with an id of `container` and a class of `section`.

---

## Exercise - European Cities

**Folder**: `Lab/Cities`  
**Main File**: `Lab/Cities/index.html`  
**Additional Files**: Individual city pages (e.g., `paris.html`, `rome.html`) for detailed descriptions.

In this exercise, you’ll create a website to showcase four European cities, each with a unique page linked from the main page. Each city will have an image, a description, lists, and a logo that serves as a clickable link to its respective page.

### Step-by-Step Instructions

1. **Create the Main Folder**: In your `Lab` folder, create a folder named `Cities`.

2. **Create the Main HTML File**: In the `Cities` folder, create `index.html`. This file will serve as the entry page for exploring the cities.

3. **Create Individual City Pages**: For each city, create an HTML file named after it (e.g., `paris.html`, `rome.html`, etc.) within the `Cities` folder.

4. **Add Images**: Place images for each city’s logo and main cityscape in the `Cities` folder. The main cityscape image should go in each city’s page, while the logo should be a link on `index.html`.

5. **Content Structure**:

   - **Main Page (index.html)**:

     - Add a title for the page (e.g., "Explore European Cities").
     - For each city, include:
       - A **city logo** as an image link (using the `<a>` and `<img>` tags) to each city’s page.
       - A **short introductory paragraph** about each city.

   - **City Pages (e.g., paris.html)**:
     - Each city page should include:
       - A large city image.
       - A paragraph with an overview of the city.
       - An **ordered list** of three top tourist attractions.
       - An **unordered list** of three local foods or cultural highlights.

---

### Example HTML Structure for index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Explore European Cities</title>
  </head>
  <body>
    <h1>Explore European Cities</h1>

    <!-- Example for Paris -->
    <div>
      <a href="paris.html">
        <img
          src="paris_logo.jpg"
          alt="Paris Logo"
          style="width:100px;height:auto;"
        />
      </a>
      <p>
        Paris is the capital of France, known for its iconic architecture, art,
        and vibrant culture. Click the logo to learn more!
      </p>
    </div>

    <!-- Repeat the above structure for other cities such as Rome, London, and Madrid -->
  </body>
</html>
```

> **Note**: The `href` in each `<a>` tag should link to the city’s specific HTML file (e.g., `paris.html`), and `src` in each `<img>` tag should reference the logo image.

---

### Example HTML Structure for Each City Page (e.g., paris.html)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Paris, France</title>
  </head>
  <body>
    <h1>Paris, France</h1>
    <img
      src="paris.jpg"
      alt="Paris City Image"
      style="width:100%;height:auto;"
    />

    <p>
      Paris is the vibrant capital of France, known worldwide as the city of
      love, light, and art. From its timeless Eiffel Tower to the exquisite
      cuisine, Paris has something for everyone.
    </p>

    <h2>Must-See Attractions</h2>
    <ol>
      <li>Eiffel Tower</li>
      <li>Louvre Museum</li>
      <li>Notre-Dame Cathedral</li>
    </ol>

    <h2>Local Specialties and Events</h2>
    <ul>
      <li>French baguettes and pastries</li>
      <li>Paris Fashion Week</li>
      <li>Cheese and wine tasting tours</li>
    </ul>
  </body>
</html>
```

> **Note**: Repeat the above structure in each city’s respective HTML file, replacing city-specific details for Rome, London, and Madrid.

---
