<h1>
  <span class="headline">CSS Grid</span>
  <span class="subhead">Responsive Grids</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to adapt grid layouts for different screen sizes using media queries.

## Media queries

The synergy between CSS Grid and media queries empowers developers to create responsive layouts that respond to changing screen sizes. By utilizing media queries, you can modify grid properties like `grid-template-columns`, `grid-template-rows`, and `grid-gap` to adjust the layout for different viewports.

Consider a two-column grid layout for desktop screens. To make this layout responsive, you can use media queries to transform it into a single-column layout for smaller devices.

```css
.grid-container {
  display: grid;
  grid-template-columns: 200px 1fr;
  grid-gap: 10px;
}

/* Media query for smaller screens */
@media (max-width: 500px) {
  .grid-container {
    grid-template-columns: 1fr;
  }
}
```

This code defines a two-column grid for larger screens. However, when the screen width is less than or equal to 500px, the media query overrides the default grid, converting it into a single-column layout.