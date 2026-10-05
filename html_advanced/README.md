# HTML Advanced: Headphone Company Webpage

A from-scratch implementation of a webpage from a designer file (Figma), built with **pure semantic HTML**: no CSS, no styling, just a clean and meaningful page structure.

This project is part of the [ALU](https://www.alueducation.com/) Software Engineering web development track, and it is the first step of a series: the HTML structure built here will be styled with CSS in the coming projects.

---

## Table of Contents

- [Objectives](#objectives)
- [The Design](#the-design)
- [Fonts](#fonts)
- [Requirements](#requirements)
- [Page Structure](#page-structure)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Tasks](#tasks)
- [Author](#author)

---

## Objectives

By the end of this project, I should be able to:

- Read a designer file in Figma and translate it into an HTML structure
- Write **semantic HTML** using the right tag for the right job (`header`, `main`, `section`, `footer`, headings, lists, links, images, ...)
- Build a page layout structure that is ready to be styled later
- Extract assets and values (text, images, dimensions) from a Figma design
- Keep structure and presentation separate: **HTML now, CSS later**

## The Design

The page to implement is the **Headphone company** design, available on Figma:

- **Page in Figma**: open the link from the project page on the intranet
- **Fig file**: downloadable from the same page

To inspect every detail of the design (spacing, text, assets), open the Figma page and use **"Duplicate to your Drafts"** from the file menu. This gives you full access to the design details, not just a view-only preview.

> Some values in Figma are floats. Feel free to round them.

## Fonts

The Figma design uses these two fonts. If they are missing on your computer, install them so the design renders as intended:

- **Source Sans Pro**
- **Spin Cycle OT**

The download links for both fonts are provided on the project page on the intranet.

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`, `VS Code`
- All files are written in **HTML5** and must be valid
- No CSS and no inline styles: structure only
- Use semantic tags wherever they apply
- A `README.md` file at the root of the project directory is **mandatory**
- Pages are viewed in a modern browser (Chrome, Firefox, Edge, Safari)

## Page Structure

The page, for the fictional brand **Aurora Audio**, is made of a header, a `<main>` with five sections, and a footer:

| Part | Tag | Content |
| --- | --- | --- |
| Header | `<header>` | Clickable logo and a block of 3 navigation links (Videos, Membership, FAQ) |
| Banner | `<section>` | Main heading, intro text, call-to-action button, and a block of 4 feature cards (image, heading, text) |
| Quote | `<section>` | Portrait image, customer `<blockquote>`, author name and subtitle |
| Videos | `<section id="videos">` | 4 video cards, each with a thumbnail, title, description, author and a 5-star rating |
| Membership | `<section id="membership">` | 4 benefit cards (image, heading, text) and a sign-up button |
| FAQ | `<section id="faq">` | 2 rows of 2 questions, each with a heading and an answer |
| Footer | `<footer>` | Logo, social media links with icons, and a copyright line |

```
<body>
├── <header>
└── <main>
│   ├── <section>   Banner
│   ├── <section>   Quote
│   ├── <section>   Videos
│   ├── <section>   Membership
│   └── <section>   FAQ
└── <footer>
```

## Project Structure

```
alu-web-development/
└── html_advanced/
    ├── README.md        # This file
    ├── index.html       # Main page (semantic structure only)
    └── images/          # 25 image assets used by index.html
```

> The files in `images/` are **temporary placeholders** with the same filenames the page expects. They are replaced by the real assets exported from Figma without any change to `index.html`.

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/hahmed2-crypto/alu-web-development.git
   cd alu-web-development/html_advanced
   ```

2. **Open the design** in Figma and duplicate it to your Drafts.

3. **Open the page in your browser**
   ```bash
   # macOS
   open index.html
   # Linux
   xdg-open index.html
   # Windows
   start index.html
   ```
   Or open the folder in VS Code and use the **Live Server** extension.

4. **Validate your HTML** with the [W3C Markup Validator](https://validator.w3.org/) before pushing.

## Tasks

| # | Task | Status |
| --- | --- | --- |
| 0 | README and objectives | Done |
| 1 | Header: skeleton, clickable logo, 3 links | Done |
| 2 | Banner: heading, text, button and 4 feature cards | Done |
| 3 | Quote: image, blockquote, author and subtitle | Done |
| 4 | Videos: 4 video cards with author and star rating | Done |
| 5 | Membership: 4 benefit cards and a button | Done |
| 6 | FAQ: 2 rows of 2 questions | Done |
| 7 | Footer: logo, social links and copyright | Done |

## Author

**Calm**: Software Engineering student at ALU, Kigali, Rwanda

GitHub: [hahmed2-crypto](https://github.com/hahmed2-crypto)
