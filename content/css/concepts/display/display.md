---
Title: 'display'
Description: 'Specifies the display behavior of an elements rendering box.'
Subjects:
  - 'Web Development'
  - 'Web Design'
Tags:
  - 'Box Model'
  - 'Layout'
CatalogContent:
  - 'learn-css'
  - 'paths/front-end-engineer-career-path'
  - 'paths/full-stack-engineer-career-path'
---

The CSS `display` property is a fundamental attribute that controls how an HTML element is rendered on a webpage. It determines the type of box used for an element and influences its layout and positioning within the document.

Understanding the different values of the `display` property is crucial for building well-structured and responsive web layouts. By choosing the appropriate value, you can control the flow of elements, create grids, and adjust the visibility of specific elements.





## Syntax

```css
display: <value>;
```

The following values can be appplied to the `display` property:

- `inline`
- `block`
- `contents`
- `flex`
- `grid`
- `inline-block`
- `inline-flex`
- `inline-grid`
- `list-item`
- `run-in`
- `table`
- `table-caption`
- `table-column-group`
- `table-header-group`
- `table-footer-group`
- `table-row-group`
- `table-cell`
- `table-column`
- `table-row`
- `none`
- `initial`
- `inherit`

## Differences between display values

The display property in CSS allows you to control how elements are rendered on a webpage. Here are the commonly used display values and their descriptions:

### 1. Display: block

Elements with `display: block;` are rendered as block-level elements. They create a line break after the element and occupy the full width of their parent container.

```css
.block-element {
  display: block;
}
```

### 2. Display: inline

Elements with `display: inline;` are rendered as inline elements. They don't create line breaks and occupy only the necessary width and height based on their content.

```css
.inline-element {
  display: inline;
}
```

### 3. Display: inline-block

  Elements with display: inline-block; are rendered as inline-level block elements. They behave like inline elements but allow you to set width, height, padding, and margins.
```css
.inline-block-element {
  display: inline-block;
}
```
### 4. Display: none

 Elements with display: none; are not rendered and are completely hidden from the page. They don't take up any space in the document flow.
```css
.hidden-element {
  display: none;
}
```
### 5. Display: flex

 Elements with display: flex; create a flex container, allowing you to build flexible and responsive layouts. Flex items inside the container can be positioned and resized using flexbox properties.
```css
.flex-container {
  display: flex;
}
```
### 6. Display: grid

Elements with display: grid; create a grid container that enables you to define rows and columns, creating a two-dimensional grid system. Child elements inside the container can be placed in specific cells and adjusted for size and alignment.
```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 10px;
}
```























## Overriding display values:

CSS specificity allows you to override default display values of elements. Here's an example of overriding display:

```css
/* Original CSS */
.element {
  display: inline;
}

/* Overriding with higher specificity */
.container .element {
  display: block;
}

```

## Responsive design considerations

The display property can be combined with media queries to create responsive designs. Here's an example:

```css
@media (max-width: 768px) {
  .element {
    display: none; /* Hide element on smaller screens */
  }
}

@media (min-width: 768px) {
  .element {
    display: block; /* Display element on larger screens */
  }
}


```

## `display: grid` and `display: flex` Comparison

CSS Grid and Flexbox are powerful layout tools. Here's an example comparing the two:

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 10px;
}

.flex-container {
  display: flex;
  justify-content: space-between;
}


```



## Example 1

Setting a `div` element to behave like a flex box.

```html
<div class="flexdiv">
  <p>First item</p>
  <p>Second item</p>
</div>
```

```css
.flexdiv {
  display: flex;
}
```


