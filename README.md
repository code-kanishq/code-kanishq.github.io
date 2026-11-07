# Kanishq Singhal — Portfolio

A self-building portfolio site. When it loads, coloured "agent" cursors draw selection boxes and type in every part of the page, while it scrolls through itself. A small bar at the bottom lets visitors pause the tour, change speed, skip to the end, or replay.

It's plain HTML, CSS and JavaScript, so there's nothing to install or build.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole website: content, styles and animation |
| `assets/kanishq.png` | My photo: a black-and-white cut-out. The coloured background behind it comes from the theme |
| `assets/og.jpg` | The preview image LinkedIn and WhatsApp show when the link is shared |
| `resume.pdf` | The file the "Resume" and "Download Resume" buttons open |

## Light and dark themes

The site opens in the light **paper** theme. The sun/moon button in the top bar lets visitors switch to dark **midnight**, and their browser remembers the choice.

To change which two themes the button switches between, open `index.html` and edit line 2:

```html
<html lang="en" data-theme="paper" data-light="paper" data-dark="midnight">
```

- `data-theme` is the theme a first-time visitor sees.
- `data-light` and `data-dark` are the two themes the button switches between.
