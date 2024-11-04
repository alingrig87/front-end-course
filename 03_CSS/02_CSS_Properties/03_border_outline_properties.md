
# CSS Border and Outline Properties

Borders and outlines are used to add visual boundaries to elements.

---

## 1. `border`
Defines the width, style, and color of an element’s border.

```css
p {
  border: 2px solid #000;
}
```

## 2. `border-radius`
Rounds the corners of an element’s border.

```css
button {
  border-radius: 5px;
}
```

## 3. `border-top`, `border-right`, `border-bottom`, `border-left`
Defines specific sides of an element's border.

```css
div {
  border-top: 2px solid black;
}
```

## 4. `outline`
Creates an outline around an element, without affecting its layout.

```css
input:focus {
  outline: 2px solid blue;
}
```

## 5. `outline-offset`
Adjusts the distance between the outline and the element’s border edge.

```css
button:focus {
  outline-offset: 3px;
}
```

## 6. `box-shadow`
Adds shadow around an element.

```css
.card {
  box-shadow: 2px 2px 5px grey;
}
```

---

Borders and outlines are essential for visually structuring elements on a webpage.
