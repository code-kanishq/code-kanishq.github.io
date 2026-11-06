# Kanishq Singhal — Portfolio

A self-building portfolio site. When it loads, coloured "agent" cursors draw selection boxes and type in every part of the page, while it scrolls through itself. A small bar at the bottom lets visitors pause the tour, change speed, skip to the end, or replay.

It's plain HTML, CSS and JavaScript, so there's nothing to install or build.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole website: content, styles and animation |
| `assets/kanishq.png` | Your photo: a black-and-white cut-out. The coloured background behind it comes from the theme |
| `assets/og.jpg` | The preview image LinkedIn and WhatsApp show when the link is shared |
| `resume.pdf` | The file the "Resume" and "Download Resume" buttons open |

## Put it online with GitHub Pages (free)

1. Go to **github.com** and sign in as `code-kanishq`.
2. Click **+** (top right), then **New repository**.
3. In **Repository name**, type exactly: `code-kanishq.github.io`
4. Leave it **Public** and click **Create repository**.
5. On the new empty repo page, click the link **uploading an existing file**.
6. Drag in everything from this folder: `index.html`, `resume.pdf`, `README.md` and the whole `assets` folder. Wait for the uploads to finish.
7. Scroll down and click **Commit changes**.
8. Click **Settings** (top of the repo), then **Pages** in the left sidebar.
9. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Set **Branch** to **main** and the folder to **/ (root)**, then click **Save**.
10. Wait 1–2 minutes and open **https://code-kanishq.github.io**.

Because the repo is named `code-kanishq.github.io`, your site gets the short address with nothing after the slash.

## Optional: also put it on Vercel

Vercel gives you a second address and a free visitor counter.

1. Go to **vercel.com** and click **Sign Up**, then **Continue with GitHub**.
2. Click **Add New…**, then **Project**.
3. Find `code-kanishq.github.io` and click **Import**.
4. Leave all settings as they are and click **Deploy**.
5. Optional: in the project, open **Analytics** and turn it on to see how many people visit.

Every time you change a file on GitHub, Vercel updates automatically.

## Light and dark themes

The site opens in the light **paper** theme. The sun/moon button in the top bar lets visitors switch to dark **midnight**, and their browser remembers the choice.

To change which two themes the button switches between, open `index.html` and edit line 2:

```html
<html lang="en" data-theme="paper" data-light="paper" data-dark="midnight">
```

- `data-theme` is the theme a first-time visitor sees.
- `data-light` and `data-dark` are the two themes the button switches between.

| Theme | Look | Background colour |
|---|---|---|
| `paper` | Warm off-white with red (light) | `#f5f1ea` |
| `midnight` | Deep navy with coral red | `#0a0e1a` |
| `ember` | Pure black with red, like the original sample | `#070707` |
| `charcoal` | Warm dark grey with amber orange | `#110f0d` |
| `mint` | Dark slate with mint green | `#0a1113` |

If you change `data-theme`, also set `<meta name="theme-color" content="…">` to that theme's background colour. This sets the colour of the browser bar on phones.

## Making changes later

- **Edit text:** open `index.html` on GitHub, click the pencil icon, and change the words between the tags. Then click **Commit changes**.
- **Swap your resume:** upload a new file with the same name, `resume.pdf`. It replaces the old one.
- **Change the photo:** upload a new `assets/kanishq.png` with a transparent background, portrait shape, about 450 × 580 px.
- **Different site address:** if your site doesn't live at `code-kanishq.github.io`, open `index.html` and update the two `og:` links near the top so the share preview still works.
- **Add a project:** copy one whole `<article class="card" …> … </article>` block in the "WORK" section, paste it below, and edit the text. The build animation picks it up automatically.

## Good to know

- Visitors who have "reduce motion" turned on see the finished page straight away, with no animation.
- If someone opens a link like `…/#contact`, the build is skipped so they land on that section at once.
- Fonts load from Google Fonts. No other outside services are used.
