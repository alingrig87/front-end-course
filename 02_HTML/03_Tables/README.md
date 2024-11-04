# HTML Tables 

Tables in HTML allow you to present data in rows and columns, providing a clear and organized structure for information. Here, you’ll find both simple and advanced examples, including the use of `colspan`, `rowspan`, and complex table structures.

---

## Basic Table Structure

A simple table consists of rows (`<tr>`), columns or cells (`<td>`), and headers (`<th>`).

### Example: Simple Table

```html
<table>
  <tr>
    <th>Item</th>
    <th>Quantity</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>Apples</td>
    <td>5</td>
    <td>$3</td>
  </tr>
  <tr>
    <td>Oranges</td>
    <td>3</td>
    <td>$2.50</td>
  </tr>
</table>
```

---

## Adding Borders and Styling

Tables can be styled to improve readability.

### Example: Table with Borders

```html
<table border="1">
  <tr>
    <th>Item</th>
    <th>Quantity</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>Apples</td>
    <td>5</td>
    <td>$3</td>
  </tr>
  <tr>
    <td>Oranges</td>
    <td>3</td>
    <td>$2.50</td>
  </tr>
</table>
```

---

## Using `colspan`

The `colspan` attribute allows a cell to span multiple columns. This is useful for grouping headers or creating sections.

### Example: School Schedule with Colspan

```html
<table border="1">
  <tr>
    <th>Day</th>
    <th>8:00 - 9:00</th>
    <th>9:00 - 10:00</th>
    <th>10:00 - 11:00</th>
  </tr>
  <tr>
    <td>Monday</td>
    <td>Mathematics</td>
    <td colspan="2">Computer Lab</td>
  </tr>
  <tr>
    <td>Tuesday</td>
    <td>History</td>
    <td>Chemistry</td>
    <td>Physical Education</td>
  </tr>
</table>
```

In this example:

- The **Computer Lab** session on Monday spans two time slots, using `colspan="2"`.

---

## Using `rowspan`

The `rowspan` attribute allows a cell to span multiple rows, often useful for displaying hierarchical data.

### Example: Monthly Events Calendar with Rowspan

```html
<table border="1">
  <tr>
    <th>Date</th>
    <th>Event</th>
  </tr>
  <tr>
    <td>March 1 - 3</td>
    <td rowspan="3">Film Festival</td>
  </tr>
  <tr>
    <td>March 4</td>
  </tr>
  <tr>
    <td>March 5</td>
  </tr>
  <tr>
    <td>March 10</td>
    <td>Charity Marathon</td>
  </tr>
</table>
```

In this example:

- The **Film Festival** spans three days, so `rowspan="3"` is used to combine these dates.

---

## Combining `colspan` and `rowspan`

For more complex layouts, combining both `colspan` and `rowspan` can help organize multi-level data.

### Example: Sales Report by Region and Quarter

```html
<table border="1">
  <tr>
    <th rowspan="2">Product</th>
    <th colspan="2">Quarter 1</th>
    <th colspan="2">Quarter 2</th>
    <th rowspan="2">Total</th>
  </tr>
  <tr>
    <th>North</th>
    <th>South</th>
    <th>North</th>
    <th>South</th>
  </tr>
  <tr>
    <td>Product A</td>
    <td>$2000</td>
    <td>$1800</td>
    <td>$2500</td>
    <td>$2300</td>
    <td>$8600</td>
  </tr>
  <tr>
    <td>Product B</td>
    <td>$1500</td>
    <td>$1600</td>
    <td>$1700</td>
    <td>$1900</td>
    <td>$6700</td>
  </tr>
</table>
```

In this example:

- The **Product** column and **Total** column each span two rows with `rowspan="2"`.
- Each **Quarter** has two sub-columns (North and South) defined using `colspan="2"`.

---

## Scheduling Example with Merged Cells

### Example: Daily Meeting Schedule with `colspan` and `rowspan`

```html
<table border="1">
  <tr>
    <th>Time</th>
    <th colspan="3">Activity</th>
  </tr>
  <tr>
    <td>8:00 - 9:00</td>
    <td colspan="3">Morning Meeting</td>
  </tr>
  <tr>
    <td>9:00 - 10:00</td>
    <td>Project Discussions</td>
    <td rowspan="2">Workshop</td>
    <td>Consultations</td>
  </tr>
  <tr>
    <td>10:00 - 11:00</td>
    <td>Marketing Presentation</td>
    <td>Team Meetings</td>
  </tr>
</table>
```

In this example:

- The **Morning Meeting** occupies all three activity columns with `colspan="3"`.
- The **Workshop** spans two time slots with `rowspan="2"`.

---

## Using Table Head, Body, and Foot

Tables can be further organized by adding `<thead>`, `<tbody>`, and `<tfoot>` sections.

### Example: Financial Report Table

```html
<table border="1">
  <thead>
    <tr>
      <th>Item</th>
      <th>Cost</th>
      <th>Quarter</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Marketing</td>
      <td>$1,000</td>
      <td>Q1</td>
    </tr>
    <tr>
      <td>Development</td>
      <td>$2,500</td>
      <td>Q2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Total</td>
      <td>$3,500</td>
    </tr>
  </tfoot>
</table>
```

This table separates the header, body, and footer using `<thead>`, `<tbody>`, and `<tfoot>`. The footer row uses `colspan="2"` to cover the "Total" column.

---
