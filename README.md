# Spider Man - Brand New Day ![Static Badge](https://img.shields.io/badge/Build%3A%20Completed-brightgreen)

<img width="1877" height="911" alt="image" src="https://github.com/user-attachments/assets/147883e0-cc71-4643-b621-879b0e5b21e5" />

A cinematic landing page inspired by the official Marvel website used to promote ticket sales for the Spider-Man movie. It features a hero section where the background image blends with the other elements, responsive SVG shapes exported from Figma, and clip-path masks applied straight from CSS.

This project was developed purely for learning purposes, together with **Gustavo Campelo** during a live event he hosted. The session covered the whole process, from designing the interface in Figma to generating and refining the final code with the help of AI.

> ⚠️ This is a non-commercial fan project. Spider-Man and all related characters, names and imagery belong to Marvel, Sony Pictures and their respective owners. No copyright infringement is intended.


<br>


## Overview

The goal of the event was not just to teach how to build this specific page, but to show **how to think about a project like a professional**, so that the same process can be used to create new projects independently.

The project was built in three main stages:

1. **Design in Figma** – The interface was designed in Figma. It wasn't created entirely from scratch: it was inspired by Marvel's official Spider-Man ticket page, with additional layouts and images from Pinterest used as references and inspiration.
2. **Preparing the design for AI** – Several frames were created in Figma so the AI could clearly understand the final layout and how each animation should behave.
3. **AI-assisted development** – The code was generated with AI from the Figma design. A big part of the event focused on writing good prompts, since modern developers need to communicate clearly with AI tools to get the expected result.


<br>


## Online Project

🔗 [Access the Project](LINK_HERE)


<br>


## Technologies

- HTML5
- CSS3
- JavaScript
- GSAP
- SVG
- Figma
- AI-assisted development (prompt engineering)


<br>


## Features

- Hero section with the background image blended into other elements using `mix-blend-mode`
- Custom SVG shapes designed and exported from Figma
- Responsive SVG clip paths using `clipPathUnits="objectBoundingBox"`
- Masking effects applied to images through CSS `clip-path`
- Animations and layout defined frame by frame in Figma
- Interface designed in Figma before development


<br>


## Learnings

During the development of this project, I practiced:

- Thinking through a project like a professional, from the initial idea to the final code
- Using real websites and Pinterest references as inspiration without copying them
- Preparing Figma frames so an AI can understand layouts and animations
- Writing clear, detailed prompts to get the expected result from AI
- Blending background images with other elements using CSS `mix-blend-mode`
- Creating SVGs in Figma and exporting them for the web
- Making SVG clip paths responsive with `objectBoundingBox` (`clipPathUnits` in HTML)
- Defining a `<clipPath>` in the HTML and applying it from CSS with `clip-path: url(#id)`

### Quick example

```html
<svg width="0" height="0">
  <clipPath id="hero-shape" clipPathUnits="objectBoundingBox">
    <path d="M0,0 H1 V0.85 L0.5,1 L0,0.85 Z" />
  </clipPath>
</svg>
```

```css
.hero-image {
  clip-path: url(#hero-shape);
}

.hero-overlay {
  mix-blend-mode: multiply;
}
```

With `objectBoundingBox`, the path coordinates go from `0` to `1`, relative to the element's size, so the shape adapts to any screen.


<br>


## Author

Project developed by Gustavo Campelo.
🔗 [YouTube](https://www.youtube.com/@gucampelo)
