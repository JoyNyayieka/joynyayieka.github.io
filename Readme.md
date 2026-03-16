#### DevFolio Portfolio
This project is a customized version of the DevFolio Bootstrap template, adapted and restructured to serve as my personal portfolio website.

The goal was not just to “fill in a template,” but to refactor it into a cleaner, scalable structure while keeping it lightweight and fast.

#### Project Overview

Originally, the template shipped as a single large HTML file with multiple sections (Home, Resume, Projects, Services, etc.).

I restructured it into a maintainable multi-page static site using Eleventy (11ty) as a static site generator.

##### What Changed

&rarr; Split large index.html into separate logical pages:
-  Home (/)
- Resume (/resume/)
-   Projects (/projects/)

&rarr; Converted the template’s starter-page.html into a reusable base layout
&rarr; Introduced layout inheritance 
&rarr; Added a build configuration using Eleventy

##### Tech Stack

1. HTML5
2. Bootstrap
3. JavaScript
4. Eleventy (11ty) for static site generation
5. Node.js (for build tooling only)

#### Why Eleventy?

- Instead of duplicating header/footer across pages, I implemented a layout-based structure:

    - starter-page.html acts as the base layout
    - Individual pages inject content into it
    - Shared UI components remain centralized

This improves maintainability and follows professional best practices without introducing heavy frontend frameworks.

##### Development
1. Dependancies - `npm install`
2. Run locally - `npx @11ty/eleventy --serve`
3. Build for production - `npx @11ty/eleventy`

The site generated will be in `_site/`

##### Project Design 
This project intentionally avoids heavy frameworks. The focus was:
- Simplicity
- Maintainability
- Performance
- Clear structure
- Clean separation of layout and content

