<!-- Please update value in the {}  -->

<h1 align="center">Simple FAQ Master | devChallenges</h1>

<div align="center">
   Solution for a challenge <a href="https://devchallenges.io/challenge/simple-faq-challenge" target="_blank">Simple FAQ</a> from <a href="http://devchallenges.io" target="_blank">devChallenges.io</a>.
</div>

<div align="center">
  <h3>
    <a href="https://cptlynx.github.io/simple-fag-master/">
      Demo
    </a>
    <span> | </span>
    <a href="https://github.com/CptLynx/simple-fag-master">
      Solution
    </a>
    <span> | </span>
    <a href="https://devchallenges.io/challenge/simple-faq-challenge">
      Challenge
    </a>
  </h3>
</div>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Overview](#overview)
  <!-- README for the Simple FAQ challenge submission -->

  # Simple FAQ — devChallenges

  Solution for the Simple FAQ challenge from devChallenges.io.

  Demo: [Open index.html](./index.html)  |  Solution: https://github.com/CptLynx/simple-fag-master  |  Challenge: https://devchallenges.io/challenge/simple-faq-challenge

  ## Table of contents

  - [Overview](#overview)
  - [What I learned](#what-i-learned)
  - [Built with](#built-with)
  - [Features](#features)
  - [How to run](#how-to-run)
  - [Demo GIF](#demo-gif)
  - [GitHub Pages workflow](#github-pages-workflow)
  - [Contact](#contact)
  - [Acknowledgements](#acknowledgements)

  ## Overview

  A small, responsive FAQ page built as a submission for the Simple FAQ challenge on devChallenges. The UI is a lightweight, accessible accordion that works without JavaScript for the toggle state (and includes a small JS enhancement where available).

  ![thumbnail](./thumbnail.jpg)

  ### What I learned

  - How to build an accessible accordion using semantic HTML and ARIA attributes.
  - Small, focused responsive layout techniques with Flexbox and CSS Grid.
  - Progressive enhancement: the page works with plain HTML/CSS and gains small interactive improvements with JS.

  ## Built with

  - HTML5
  - CSS3 (custom properties, Flexbox, Grid)
  - Vanilla JavaScript (small enhancement for animation and state)

  ## Features

  - Responsive design (mobile, tablet, desktop)
  - Accessible accordion pattern (keyboard navigable, ARIA attributes)
  - Small footprint — no build step required

  ## How to run

  1. Open `index.html` in your browser (double-click or use your browser's File -> Open).
  2. Or serve the folder with a static server (recommended for local testing):

    Example using Python 3 (macOS):

    ```bash
    python3 -m http.server 8000
    # then open http://localhost:8000 in your browser
    ```

  ## Demo GIF

  Add a short demo GIF next to the README so visitors can quickly preview the UI.

  - Put the file at `./demo.gif` (this repo currently includes `thumbnail.jpg`; replace or add `demo.gif`).
  - To create a GIF on macOS using QuickTime + ffmpeg:

    1. Record a screen clip with QuickTime Player (File → New Screen Recording). Save as `clip.mov`.
    2. Convert to GIF with ffmpeg (install via Homebrew: `brew install ffmpeg`):

      ```bash
      ffmpeg -i clip.mov -vf "fps=15,scale=960:-1:flags=lanczos" -loop 0 demo.gif
      ```

  - Alternatively, use an animated PNG or a short MP4; GitHub README displays GIFs and MP4s differently — GIF is simplest.

  Example markdown to show the GIF in this README:

  ```markdown
  ![demo](./demo.gif)
  ```

  ## GitHub Pages workflow

  This repository includes a GitHub Actions workflow that will deploy the repository root to the `gh-pages` branch and publish to GitHub Pages on every push to `main`.

  - Workflow file: `.github/workflows/pages-deploy.yml`
  - Behavior: on push to `main` the action will checkout the repo and publish the repository contents to `gh-pages` using the `GITHUB_TOKEN`.
  - After the first successful run, the site will be available at `https://<your-username>.github.io/<your-repo>` (you can confirm or change the Pages settings in your repository settings).

  If you want the workflow to publish a subfolder (for example `docs/`), update the `publish_dir` value in the workflow file.

  ## Contact

  - GitHub: https://github.com/CptLynx

  ## Acknowledgements

  - devChallenges — challenge prompt and design
  - Accessibility resources and patterns (WAI-ARIA) that guided the accordion implementation

  ---

  If you'd like, I can:

  - copy this content into `README.md` at the repository root, 
  - create a small demo GIF for you from a short recording you provide, or
  - change the workflow to publish from a different branch or folder.
