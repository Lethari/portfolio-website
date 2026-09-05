# Phildah Lekalakala Portfolio

This four-page portfolio introduces Phildah Lekalakala, an aspiring web developer, and presents her background, technical skills, projects, and contact details. It is a small static site designed to be clear, responsive, and easy to navigate.

## Summary of Issues Found [Full issued noted issues identified](design/issues-identified.txt)

- The starter pages lacked semantic landmarks, navigation, metadata, and consistent structure.
- The home image path and one project image filename were invalid.
- Images had weak or generic alternative text, and the skills table was missing.
- The contact form had no labels, useful input types, or browser validation.
- The footer on the contact page was incorrectly nested.
- The original CSS had poor contrast, limited selectors, no responsive layout, and incomplete form, table, and box-model styling.
- There was no repository structure everything was places on the main folder- no clear indication of grouping.

## Fixes Implemented

- All pages now use `header`, `nav`, `main`, `section`, `article`, and `footer` landmarks with a consistent four-link menu.
- Asset paths were corrected, four project cards were retained, and every image has descriptive `alt` text. About includes a captioned, headed table with scoped column headings.
- Contact uses labelled fields, `fieldset` and `legend`, five input types (`text`, `tel`, `email`, `url`, and `date`), required fields, minimum length, autocomplete, and a message textarea.
- Created a repository stucture as per reccomendation.

## HTML and CSS

- The HTML keeps content in logical sections and uses articles for repeated projects.
- `css/styles.css` defines reusable colour variables, a constrained layout, grid and flexbox, responsive breakpoints, typography hierarchy, focus states, table styling, and form controls.
- It also demonstrates element, class, descendant, grouped, attribute, pseudo-class, and media-query selectors. Padding, margins, borders, sizing, and box shadows visibly demonstrate the box model.

## Accessibility

Pages declare language, character encoding, viewport, and author metadata. Form labels connect to inputs, headings provide hierarchy, table headers use `scope`, images have alt text, keyboard focus is visible, and link contrast is maintained. External links use `noopener noreferrer`.

## View Locally

Use VS Code Live Server:

1. Install the `Live Server` extension by **Ritwick Dey** from the Extensions view.
2. Open the project folder, `foundational_starter_code`, in VS Code.
3. Open `index.html` and click **Go Live** in the status bar.
4. Your browser will open the portfolio at a localhost address, usually `http://127.0.0.1:5500/index.html`.

Use the navigation menu to open About, Projects, and Contact. Stop the server by clicking the localhost port in the status bar.

## Screenshots

- [Homepage](screenshots/homepage.png)
- [About and table](screenshots/about.png)
- [Contact form](screenshots/form.png)
- [Projects](screenshots/projects.png)
- [Navigation](screenshots/navigation.png)
- [Mobile layout](screenshots/mobile.png)

The four-page layout is also shown in [the wireframe](design/wireframe.png)/ pdf wireframe as per request is attached as a pdf in classroom.
Alternatively also available for viewing on figma: https://www.figma.com/design/OKZIIcvRM4mhw9yMGRkpoM/Portfolio?node-id=0-1&t=t3PnTAECC2sGSq0l-1

## Reflection

The main debugging challenge was separating content problems from a stylesheet loading failure. Checking the file tree exposed the incorrect CSS path first; checking image filenames then exposed case, spacing, and location mismatches. I fixed those references before styling, validated the HTML through editor diagnostics, and used shared selectors so the same corrections apply consistently across all pages.


