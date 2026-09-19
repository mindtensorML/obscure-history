# Obscure History

Public site for **Obscure History** — an archive of translated old stories, told chapter by chapter, and the written companion to the YouTube channel.

This is a **static GitHub Pages** site: HTML, CSS, and a few lines of JavaScript for the mobile menu. No CMS, no build step, no database, no paid host.

## Live URL

https://mindtensorml.github.io/obscure-history/

Pages is served from the `main` branch, root folder.

## YouTube

https://www.youtube.com/@obscurehistorystoriesfromworld

Handle: `@obscurehistorystoriesfromworld`

## Story structure

```
stories/
  index.html                 # lists every story
  some-story-slug/
    index.html               # lists chapters
    chapter-01.html
    chapter-02.html
```

The home page also lists stories. Archive cards are **placeholders only** — do not present them as real translations.

To add a finished story later:

1. Copy a placeholder folder under `stories/`.
2. Give it a slug, a title, and one `chapter-NN.html` per chapter.
3. Link it from `index.html` and `stories/index.html`.

## Branding

Swap art without a redesign:

| File | Used as |
| --- | --- |
| `assets/avatar.jpg` | Header and footer logo |
| `assets/banner.jpg` | Home hero banner (cropped with `object-fit`, not stretched) |
| `assets/favicon.jpg` | Tab icon |

Brand colors live at the top of `styles.css` as `--brand-*` variables (`--brand-paper`, `--brand-ink`, `--brand-accent`, `--brand-gilt`, `--logo-size`, `--banner-height`). Change those tokens when new assets arrive.
