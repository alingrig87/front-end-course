
# CSS Display and Visibility Properties

Display and visibility properties in CSS control the visibility and layout behavior of elements on a webpage. They are essential for managing the flow, stacking, and appearance of elements.

---

## 1. `display`

The `display` property sets the layout behavior of an element, determining how it occupies space in the layout.

- **block**: The element takes up the full width of its container and starts on a new line.
- **inline**: The element takes up only as much width as necessary and does not start on a new line.
- **inline-block**: Combines the characteristics of `inline` and `block`, allowing elements to flow inline while respecting height and width settings.
- **none**: The element is not displayed at all (removed from the document flow).

```css
span {
	display: inline-block;
}
```

Using `display` can adjust how elements interact with each other within the document flow.

---

## 2. `visibility`

The `visibility` property controls whether an element is visible or hidden.

- **visible**: The element is visible (default).
- **hidden**: The element is invisible but still takes up space in the layout.

```css
div {
	visibility: hidden;
}
```

`visibility` is useful for toggling visibility without disrupting the layout structure.

---

## 3. `opacity`

The `opacity` property sets the transparency level of an element.

- **Range**: Values from `0` (completely transparent) to `1` (completely opaque).

```css
img {
	opacity: 0.5;
}
```

Using `opacity` can create transparency effects, useful for overlays and highlighting.

---

## 4. `z-index`

The `z-index` property defines the stacking order of positioned elements. Higher values are placed in front of lower values.

- **Positive Values**: Place elements in front.
- **Negative Values**: Place elements behind.

```css
.modal {
	z-index: 100;
}
```

Setting `z-index` is essential for layering elements, especially in complex layouts or with modals.

---

## 5. `float`

The `float` property aligns elements to the left or right of their container, allowing other content to wrap around them.

- **left**: The element floats to the left.
- **right**: The element floats to the right.
- **none**: Default; the element does not float.

```css
img {
	float: right;
}
```

`float` is often used for wrapping text around images or for layout purposes.

---

## 6. `clear`

The `clear` property specifies whether an element should move below any preceding floated elements.

- **left**: Prevents floating elements on the left side.
- **right**: Prevents floating elements on the right side.
- **both**: Moves the element below both left and right floated elements.

```css
footer {
	clear: both;
}
```

Using `clear` is helpful for layout control, particularly when ending a floated section.

---

## Practical HTML Example Using Display and Visibility Properties

Here's an example HTML document demonstrating display and visibility properties:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Display and Visibility Properties Example</title>
    <style>
        .container {
            display: flex;
            justify-content: space-around;
            border: 2px solid #333;
            padding: 10px;
        }

        .box {
            width: 100px;
            height: 100px;
            background-color: #007acc;
            color: white;
            text-align: center;
            line-height: 100px;
        }

        .hidden-box {
            visibility: hidden;
        }

        .transparent-box {
            opacity: 0.5;
        }

        .float-right {
            float: right;
            margin-left: 20px;
            width: 150px;
        }

        .clearfix::after {
            content: "";
            display: block;
            clear: both;
        }

        .modal {
            position: relative;
            z-index: 100;
            padding: 10px;
            background-color: rgba(0, 0, 0, 0.8);
            color: white;
            width: 200px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container clearfix">
        <div class="box">Visible Box</div>
        <div class="box hidden-box">Hidden Box</div>
        <div class="box transparent-box">Transparent Box</div>
    </div>
    <img src="example.jpg" alt="Floated Image" class="float-right" />
    <div class="modal">Modal with z-index</div>
    <footer>Footer section with clear applied</footer>
</body>
</html>
```

In this example:

- **`.container`** demonstrates `display: flex` for layout control and spacing of items.
- **`.hidden-box`** uses `visibility: hidden`, making the box invisible but leaving space.
- **`.transparent-box`** applies `opacity`, adding transparency to the box.
- **`.float-right`** uses `float: right` to align an image to the right with text wrapping.
- **`.modal`** with `z-index` demonstrates layering on top of other elements.
- **`footer`** applies `clear: both` to prevent it from being affected by floated elements.

This example combines display and visibility properties to create flexible layouts and visibility effects.
