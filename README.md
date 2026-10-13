# shua-kang.github.io

Personal academic homepage of **Xuhui (Joshua) Kang** — Ph.D. student in Computer Science
at the University of Virginia. Served with GitHub Pages at <https://shua-kang.github.io>.

## Credits

This site uses the **[Minimal Light](https://github.com/yaoyao-liu/minimal-light)** theme,
created by **[Yaoyao Liu](https://github.com/yaoyao-liu)**. Many thanks to the author for
building and sharing such a clean, elegant academic homepage theme (which itself builds on
[Minimal](https://github.com/orderedlist/minimal) by [Steve Smith / orderedlist](https://github.com/orderedlist)).

The theme's compiled stylesheets, fonts, and scripts are vendored here so the page is served
as plain static files — no build step required.

## Structure

- `index.html` — the page (about + publications with a **Selected / Full list** toggle)
- `assets/css/` — Minimal Light theme styles (`style.css`, `publications.css`, `font.css`) plus `custom.css` for the publication list and toggle
- `assets/js/` — theme helpers (`scale.fix.js`, `favicon-switcher.js`)
- `assets/img/` — profile photo and favicons

## Editing

- **Bio / research interests:** edit the `<section>` at the top of `index.html`.
- **Publications:** every paper is a `.pub-item` — a 16:9 media thumbnail on the left and
  the details on the right. *Selected* (`#pubs-selected`) holds first-author, non-workshop
  papers; *Full list* (`#pubs-full`) holds everything, grouped by `.pub-group-h` sections.
  Copy an existing `.pub-item`, then edit the badge, title, authors, venue, and links, and
  wrap your own name in `<strong>…</strong>`.
  - **Media** lives in `assets/img/covers/`. For the left thumbnail use one of:
    - an image — `<img class="cover-img" ...>` (auto-cropped to 16:9);
    - a 16:9 video — `<video class="cover-vid" autoplay loop muted playsinline>`;
    - a non-16:9 video — a `.blurfill` block with two `<video>` copies (`.bg` blurred +
      `.fg` centered) so the sides are filled instead of black-barred;
    - nothing — `<div class="cover-placeholder">…</div>`.
  - Keep videos small: re-encode with ffmpeg (strip audio, ~480p, ~24 fps, CRF 30).

To preview locally, just open `index.html` in a browser (light and dark modes follow your OS setting).
