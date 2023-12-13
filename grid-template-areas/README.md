# ![CSS Grid - Grid Template Area](./assets/hero.png)


## Understanding `grid-template-area`

`grid-template-area` allows us to create a grid layout in a more intuitive way. We define areas of the grid and assign them names, making it easier to place items exactly where we want. 


We can use `grid-template-area` to easily place all of our page sections correctly. To test this, use the following CSS:

```css
body {
  display: grid;
  font-family: sans-serif;
  font-size: 24px;
  grid-template-rows: auto 1fr auto;
  grid-template-columns: 1fr 2fr; 
  grid-template-areas: 
    "nav nav nav"  /* place area name in cells you want to fill */
    "aside main main"
    "footer footer footer"; 
  min-height: 100vh;
  margin: 0;
  padding: 0;
}

aside {
  background-color: #38b18a;
  grid-area: aside; /* name of area */
}

main {
  background-color: #92d97c;
  grid-area: main; /* name of area */
}

nav {
  grid-area: nav; /* name of area */
}

footer {
  background-color: #f9f871;
  grid-area: footer; /* name of area */
}

footer, nav {
  min-height: 60px
}

a {
  text-decoration: none;
  color: black;
}

```

## Flexbox + Grid

Flexbox can be effectively used within CSS Grid cells to center items. While Grid arranges the overall layout, Flexbox excels in aligning and centering content inside Grid cells. This combination offers precise control, making layouts both flexible and visually balanced.

Let's make a stylistic change by creating a class that will center the text of our elements. Add this to your CSS file:

```css
.flex-container {
  display: flex;
  align-items: center;
  justify-content: center;
}
```

Now add the class `flex-container` to the semantic HTML elements `<aside>`, `<main>`, & `<footer>`. 

Ta-da! We just created our first grid layout!