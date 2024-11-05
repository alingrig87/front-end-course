
# CSS Interview Answers

This document provides answers to the CSS interview questions covering text properties, background properties, border and outline properties, box model properties, and display & visibility properties.

---

## Text Properties

1. **The `color` property** controls the color of text in an element. It can accept named colors (e.g., `red`), hex codes (e.g., `#333333`), RGB values (e.g., `rgb(51, 51, 51)`), and HSL values (e.g., `hsl(0, 0%, 20%)`).
2. **`em`** is a relative unit based on the font size of the parent element, while **`rem`** is relative to the root font size, providing more consistency in responsive design.
3. To make text uppercase in CSS, use the **`text-transform: uppercase;`** property.
4. The **`letter-spacing`** property adjusts the spacing between characters. It can accept positive or negative values to increase or decrease spacing.

---

## Background Properties

5. Use the **`background-image`** property with `url()` to set an image as the background, e.g., `background-image: url('image.jpg');`.
6. The **`background-repeat`** property controls if and how a background image repeats. Possible values include `repeat`, `no-repeat`, `repeat-x`, and `repeat-y`.
7. **`background-size: cover`** scales the background image to cover the entire element, potentially cropping parts of it, while **`background-size: contain`** scales the image to fit within the element without cropping.
8. The **`background-attachment`** property controls whether a background image scrolls with the content (`scroll`) or stays fixed in place (`fixed`).

---

## Border and Outline Properties

9. **`border`** is part of the box model and affects layout, while **`outline`** does not affect layout and is used for focus or emphasis, especially in accessibility.
10. **`border-radius`** rounds the corners of an element, creating a softer, more modern appearance.
11. **`outline-offset`** controls the distance between an element's outline and its border, useful for adding extra space around the outline for emphasis.
12. Use the **`box-shadow`** property to add a shadow around an element, specifying offset, blur radius, and color.

---

## Box Model Properties

13. The CSS box model consists of **content, padding, border, and margin**. It defines the space an element occupies and how it interacts with other elements.
14. **`box-sizing: border-box`** includes padding and border in an element's total width and height, making layout calculations simpler.
15. Use **`max-width`** to ensure an element does not exceed a certain width, allowing it to scale down if needed.
16. **`margin: auto`** centers an element horizontally within its container, commonly used with a defined `width` for layouts.

---

## Display and Visibility Properties

17. **`display: none`** removes the element from the document flow, making it invisible, while **`visibility: hidden`** keeps the element in the flow but hides it visually.
18. **`display: inline-block`** allows elements to sit inline with others while respecting width and height settings, unlike `inline` (no width/height) and `block` (new line).
19. **`z-index`** controls the stacking order of positioned elements. Higher `z-index` values appear on top of lower ones, useful for layering modals or tooltips.
20. **`float`** positions an element to the left or right of its container, allowing other content to wrap around it, while **`clear`** moves an element below floated elements.

---

