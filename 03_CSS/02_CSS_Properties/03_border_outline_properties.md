
# CSS Border and Outline Properties

Borders and outlines are used to add visual boundaries to elements, making them essential for structuring and highlighting elements on a webpage. Below is a guide to the primary CSS border and outline properties with examples.

---

## 1. `border`

The `border` property defines the width, style, and color of an element's border. It is a shorthand for setting all sides at once.

- **Width**: e.g., `1px`, `2px`
- **Style**: e.g., `solid`, `dotted`, `dashed`
- **Color**: e.g., named color, hex, RGB

```css
p {
	border: 2px solid #000;
}
```

---

## 2. `border-radius`

The `border-radius` property rounds the corners of an element's border, allowing for soft, circular shapes.

```css
button {
	border-radius: 5px;
}
```

`border-radius` is often used to create rounded buttons or card-style layouts.

---

## 3. `border-top`, `border-right`, `border-bottom`, `border-left`

These properties allow you to define borders for specific sides of an element individually.

```css
div {
	border-top: 2px solid black;
}
```

Using these properties is useful for adding emphasis or styling to particular sides of an element.

---

## 4. `outline`

The `outline` property creates a line around an element, without affecting its layout. It is commonly used for focus indicators.

- **Width**: e.g., `2px`
- **Style**: e.g., `solid`, `dotted`
- **Color**: e.g., named color, hex

```css
input:focus {
	outline: 2px solid blue;
}
```

Outlines are often used to improve accessibility by providing clear visual focus cues.

---

## 5. `outline-offset`

The `outline-offset` property adjusts the distance between the outline and the element’s border edge, enhancing visual separation.

```css
button:focus {
	outline-offset: 3px;
}
```

This property provides extra space between the outline and element, which can be helpful in creating distinctive focus states.

---

## 6. `box-shadow`

The `box-shadow` property adds shadow effects around an element, providing depth and emphasis.

- **Offset**: e.g., `2px 2px`
- **Blur Radius**: e.g., `5px`
- **Color**: e.g., `grey`

```css
.card {
	box-shadow: 2px 2px 5px grey;
}
```

`box-shadow` is widely used to add subtle or dramatic depth to elements, making them stand out.

---

## Practical HTML Example Using CSS Border and Outline Properties

Here's an example HTML document demonstrating the border and outline properties covered above:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Border and Outline Properties Example</title>
    <style>
        .container {
            border: 2px solid #333;
            border-radius: 10px;
            padding: 20px;
            max-width: 600px;
            margin: 50px auto;
            box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.2);
            text-align: center;
        }

        button {
            border: 2px solid #007acc;
            border-radius: 8px;
            padding: 10px 20px;
            outline: none;
        }

        button:focus {
            outline: 2px solid #ff7f50;
            outline-offset: 3px;
        }

        .highlight {
            border-top: 4px dashed #ff4500;
            padding-top: 15px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>CSS Border and Outline Example</h1>
        <p>Experiment with different borders and outlines to create visually appealing elements on your webpage.</p>
        <button>Click Me</button>
        <p class="highlight">This paragraph has a custom top border style.</p>
    </div>
</body>
</html>
```

In this example:

- **`.container`** uses border, border-radius, and box-shadow to create a distinct card-like style.
- **`button`** showcases rounded borders and a focused outline effect, enhancing interactivity.
- **`.highlight`** demonstrates a dashed top border for specific visual emphasis.

This example combines the border and outline properties to create a cohesive, visually appealing layout.
