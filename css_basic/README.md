# CSS Basic: Styling and Layout with Flexbox

In the previous project (`html_basic`), the website was built with HTML only. This project adds **CSS** to it: the same two pages (`index.html` and `tweets.html`) are connected to stylesheets, laid out with **CSS Flexbox**, made **responsive** for smartphones, and given a personal look.

This project is part of the [ALU](https://www.alueducation.com/) Software Engineering web development track.

---

## Table of Contents

- [Objectives](#objectives)
- [Files](#files)
- [How It Works](#how-it-works)
- [Tasks](#tasks)
- [Getting Started](#getting-started)
- [Requirements](#requirements)
- [Author](#author)

---

## Objectives

By the end of this project, I should be able to:

- Link external CSS files to an HTML page with the `<link>` tag
- Position the main parts of a page with **Flexbox** (`display: flex`, `flex-direction`, `flex`)
- Control scrolling inside a section with `overflow-y`
- Make a layout **responsive** with a viewport meta tag and a CSS class
- Style a page with colors, backgrounds, borders and typography without breaking the layout
- Keep the layout rules and the decorative rules clearly separated

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Home page, with the header / main / footer structure |
| `tweets.html` | Page showing an embedded tweet, using the same structure and the same stylesheets |
| `base.css` | General defaults and the responsive rules for small screens |
| `styles.css` | The flexbox layout and my own custom styling |
| `README.md` | This file |

## How It Works

Every page shares the same structure:

```
<body class="works_on_smartphone">
├── <header>    navigation list + logo
├── <main>
│   ├── <article>    page content   (2/3 of the width)
│   └── <aside>      side content   (1/3 of the width)
└── <footer>
```

**Layout (Flexbox), written in `styles.css`:**

| Element | Rule | Why |
| --- | --- | --- |
| `body` | `display: flex; flex-direction: column;` | Stacks header, main and footer vertically |
| `main` | `display: flex; flex-direction: row; flex: auto;` | Puts article and aside side by side, with automatic size |
| `article` | `flex: 2; overflow-y: auto;` | Takes 2/3 of the width and scrolls on its own |
| `aside` | `flex: 1; overflow-y: auto;` | Takes 1/3 of the width and scrolls on its own |

**Responsive design:**

- Both pages include `<meta name="viewport" content="width=device-width, initial-scale=1.0">`, so a smartphone does not show the page "zoomed out".
- The `works_on_smartphone` class on `<body>` activates the rules in `base.css` that stack the article and the aside on small screens, so the layout degrades nicely when the window is resized.

**Custom styling:** colors, backgrounds, borders, a logo character in the header and the look of the article content are all in `styles.css`. They only affect appearance, never the flexbox layout.

## Tasks

| # | Task | Status |
| --- | --- | --- |
| 0 | Some early styling: copy the HTML files, create `styles.css` and `base.css`, and link both in every page's `<head>` | Done |
| 1 | Positioning: header, main (article + aside) and footer laid out with Flexbox | Done |
| 2 | Responsive web design: `works_on_smartphone` class and the viewport meta tag | Done |
| 3 | Some more styling: custom CSS, a logo in the header, and a nicer look for both pages | Done |

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/hahmed2-crypto/alu-web-development.git
   cd alu-web-development/css_basic
   ```

2. **Open the site in a browser**
   ```bash
   # macOS
   open index.html
   # Linux
   xdg-open index.html
   # Windows
   start index.html
   ```
   Or open the folder in VS Code and use the **Live Server** extension.

3. **Test the responsive layout** by resizing the browser window, or use the device toolbar in the browser developer tools (`F12`, then `Ctrl+Shift+M`).

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`, `VS Code`
- All HTML files start with `<!DOCTYPE html>` and every page links both `base.css` and `styles.css`
- Every page has the same header / main / footer structure, with the article and aside inside `main`
- The layout strategy must stay Flexbox: only styling inside `<article>` may use other positioning
- A `README.md` file at the root of the project directory is **mandatory**

## Author

**Hassan Ahmed**: Software Engineering student at ALU, Kigali, Rwanda

GitHub: [hahmed2-crypto](https://github.com/hahmed2-crypto)
