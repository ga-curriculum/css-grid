<h1>
  <span class="headline">CSS Grid</span>
  <span class="subhead">Setup</span>
</h1>

Open your Terminal application and navigate to your ~/code/sei/lectures directory:

```bash
cd ~/code/sei/lectures
```
Make a new directory called `css-grid`, then enter this directory:

```bash
mkdir css-grid
cd css-grid
```

Create a directory called `css`:

```bash
mkdir css
```

Then, create an `index.html` file, and a `style.css` file that lives inside the `css` directory. These files will hold your work for this lecture:

```bash
touch index.html css/style.css
```
With the files created, open the contents of the directory in VS Code:

```bash
code .
```

Open the `index.html` file and add HTML boilerplate by typing `!` and then hitting the `Tab` key. Then link the `style.css` file by adding this line inside the `<head>` tag:

```html
<link rel="stylesheet" href="./css/style.css">
```