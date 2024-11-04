
# CSS Spacing Properties (Margin and Padding)

Margin and padding control the spacing inside and outside of elements.

---

## 1. `margin`
Sets the space outside the element's border. Can specify individual sides (top, right, bottom, left).

```css
div {
  margin: 20px;
}
```

## 2. `padding`
Adds space inside the element’s border, around its content.

```css
.container {
  padding: 10px;
}
```

## 3. `margin-top`, `margin-right`, `margin-bottom`, `margin-left`
Controls the margin on specific sides.

```css
p {
  margin-top: 15px;
}
```

## 4. `padding-top`, `padding-right`, `padding-bottom`, `padding-left`
Controls the padding on individual sides.

```css
div {
  padding-bottom: 5px;
}
```

## 5. `margin: auto`
Centers an element horizontally, typically used with `width`.

```css
.container {
  width: 50%;
  margin: auto;
}
```

## 6. `box-sizing`
Defines how the total width and height of an element are calculated.

```css
* {
  box-sizing: border-box;
}
```

---

Properly managing margin and padding is key to creating clean layouts.
