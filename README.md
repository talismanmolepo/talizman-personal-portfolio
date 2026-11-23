<div align="center">

# Personal Portfolio Website

A responsive, single-page developer portfolio built with plain HTML, CSS and JavaScript.
No frameworks, no build step, no dependencies.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

[**Live demo**](https://YOUR-USERNAME.github.io/Personal-Portfolio-Website/) ·
[Report a bug](https://github.com/YOUR-USERNAME/Personal-Portfolio-Website/issues)

</div>

![The portfolio on desktop, laptop, tablet and phone](docs/mockup.png)

> The screenshot above uses sample content.

---

## Table of contents

- [About](#about)
- [Features](#features)
- [Built with](#built-with)
- [Project structure](#project-structure)
- [Getting started](#getting-started)
- [Deploying to GitHub Pages](#deploying-to-github-pages)
- [Customising the site](#customising-the-site)
- [Browser support](#browser-support)
- [Ideas for later](#ideas-for-later)
- [License](#license)
- [Contact](#contact)

## About

This is my personal portfolio. It introduces who I am, shows my background, skills and education,
lists the projects I have built, and makes it easy to get in touch. The whole site lives in a single
`index.html` file, so it is simple to read, edit and host anywhere.

## Features

- **Responsive layout** that adapts from large desktop screens down to phones.
- **Sticky navigation bar** with smooth scrolling, a hamburger menu on small screens, and automatic
  highlighting of the section you are viewing. The menu closes when you pick a link, click outside it
  or press `Esc`.
- **Hero section** with a short introduction and a *Download CV* button.
- **About section** with a profile card, quick-fact tiles, and Background, Skills and Education cards.
- **Project portfolio** shown as hoverable cards with a description, tools used and a link.
- **Contact section** with animated social cards for Email, LinkedIn and GitHub, plus a
  *Copy email* button.
- **Footer** with quick links, social links, an automatic copyright year and a back-to-top button.

## Built with

| Technology | Used for |
| --- | --- |
| HTML5 | Page structure |
| CSS3 (Flexbox, Grid, custom properties, transitions) | Layout, theme and animations |
| Vanilla JavaScript | Navigation menu, active-link highlighting, copy-to-clipboard, back-to-top |
| GitHub Pages | Hosting |

## Project structure

```text
Personal-Portfolio-Website/
├── index.html          # the whole site (HTML, CSS and JavaScript)
├── images/             # photos and project screenshots
│   ├── about-photo.jpg
│   └── profile.jpg
├── documents/
│   └── Firstname-Lastname-CV.pdf
│   
├── README.md
├── LICENSE
└── .gitignore
```

## Getting started

You do not need to install anything.

1. **Clone the repository**

   ```bash
   git clone https://github.com/YOUR-USERNAME/Personal-Portfolio-Website.git
   cd Personal-Portfolio-Website
   ```

2. **Open it in a browser.** Either double-click `index.html`, or serve it locally, which behaves
   more like the live site:

   ```bash
   # Python 3
   python -m http.server 8000
   # then visit http://localhost:8000
   ```

   Or use the **Live Server** extension in VS Code and choose *Open with Live Server*.

> **Tip:** all image and CV paths are relative (for example `images/hero.jpg`, with no leading `/`),
> so the site works the same locally, on a project site and on a user site.

## Deploying to GitHub Pages

1. Push the project to a GitHub repository, with `index.html` in the root of the `main` branch.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the `main`
   branch and the `/ (root)` folder, then click **Save**.
4. After a minute or two the site is live at
   `https://YOUR-USERNAME.github.io/Personal-Portfolio-Website/`.

For a shorter address, name the repository `YOUR-USERNAME.github.io`; it is then served at
`https://YOUR-USERNAME.github.io/`.

> **GitHub Pages is case-sensitive.** `Profile.JPG` and `profile.jpg` are different files, so match
> the capitalisation in `index.html` exactly, and avoid spaces in file names.

## Customising the site

Everything is in `index.html`. Use your editor's search to jump to the parts below.

| To change | Look for |
| --- | --- |
| Name, role and intro text | the `.myintro` block at the top |
| CV link | the `Download CV` link, and the file in `assets/` |
| Profile photo and bio | `.about-card` (photo: `images/profile.jpg`) |
| Quick facts (location, languages, availability) | the `.fact` lines inside `.facts` |
| Background, Skills, Education | the three `<article class="topic">` blocks |
| Projects | the `.card` blocks inside `#projects` |
| Email, LinkedIn and GitHub links | the `.social-card` blocks inside `#contact`; the email also appears in the `data-copy` attribute of the copy button |
| Footer links | the `<footer>` block |
| Colours | the main accent is `#482222` (maroon) and the highlight is `#f4b942` (gold); search and replace them |

## Browser support

The site uses standard modern CSS and JavaScript (Flexbox, Grid, `scroll-behavior`, the Clipboard API).
It was developed and tested in Chromium, including phone-sized viewports, and is expected to work in
current versions of Firefox, Safari and Edge. If the Clipboard API is unavailable, the *Copy email*
button falls back to opening your mail app.

## Ideas for later

- [ ] Dark mode toggle
- [ ] Filter projects by technology
- [ ] Add a blog or case-study page for each project
- [ ] Add social-sharing preview tags (Open Graph) for nicer link previews

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for details.

## Contact

**[Your Name]** · [your.email@example.com](mailto:your.email@example.com) ·
[LinkedIn](https://www.linkedin.com/in/YOUR-USERNAME) ·
[GitHub](https://github.com/YOUR-USERNAME)
