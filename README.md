# hackathon

**Jak przetrwać hackathon AI?** A step-by-step guide for kids taking part in an AI hackathon, in Polish.

Live: https://workszop.github.io/hackathon/

## What's inside

- **Introduction:** what an AI hackathon is, what to expect and how to prepare.
- **The project process in 5 steps:** idea, planning, building, testing, presentation, with time hints for each step.
- **Troubleshooting:** what to do when something breaks or you run out of ideas.
- **Summary.**

## Features

- Sticky table of contents that highlights the current section and shows reading progress.
- On phones the contents become a slide-out menu (the "Spis treści" button); `Esc` closes it.
- Each section has its own colour, and the side menu uses the same colours as a key.
- A step timeline for the process, priority levels for project scope, and a presentation time bar sized to each part's length.

## Tech

- One self-contained `index.html` (inline CSS and JS, no build step).
- Styled with the **edulab** design system ("Editorial Color" tokens; fonts: Outfit, IBM Plex Sans, Roboto Mono from Google Fonts).
- Icons: [Lucide](https://lucide.dev), loaded from unpkg and pinned to `lucide@1.48.0`.
- Deployed with GitHub Pages from `main`.

## Run locally

Open `index.html` in a browser.

## Editing

- **Colours** are CSS custom properties in the `:root` block at the top of the `<style>`. Use the tokens, not raw hex values.
- **Section colour:** add `acc-yellow`, `acc-blue`, `acc-green`, `acc-grape`, `acc-berry` or `acc-red` to a `<section class="sec ...">`. Its icons, chips, tiles and card icons pick up that colour. Give the matching `<li>` in the table of contents the same class.
- **Icons:** use `<i data-lucide="icon-name"></i>` with any name from [lucide.dev/icons](https://lucide.dev/icons).
- **New section:** add a `<section class="sec acc-..." id="...">` and a link to it in the `<nav class="toc">` list. Scroll tracking picks it up automatically.
- The table of contents exposes its state as `data-active-section` and `data-progress` on `<nav id="toc">`, for automated checks.
