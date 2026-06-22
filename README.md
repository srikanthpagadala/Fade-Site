# Fade Labs — website

![Fade Labs — Imagine it, and it Fades In.](social-preview.png)

> *Imagine it, and it Fades In.*

The single-page site for **Fade Labs, Inc.** — a stealth Pixel Search company. Fade looks at the
image first to find the exact thing you're picturing; denim is where we begin.

🔗 **Live:** [fadelabs.ai](https://fadelabs.ai)

---

## What's here

A self-contained static site — no build step, no framework, no dependencies.

| File | Purpose |
|------|---------|
| `index.html` | The entire site: markup, styles, and the animated demo, all inline. |
| `logo.svg` | The denim-pocket brand mark. Also used as the favicon and Apple touch icon. |
| `CNAME` | Custom-domain binding for GitHub Pages (`fadelabs.ai`). |

## Design notes

- **One continuous hero** that fills the viewport on any screen (`100svh`), re-centering as you resize.
- **A self-narrating search bar** — the demo types real queries and walks through the story:
  describe it → show it → say it → refine it → *…it Fades In.*
- **Caveat** handwritten headline over **Nunito** body copy; the wordmark is **JetBrains Mono**.
- **Indigo palette**, locked dark on every device for a consistent look (no light/dark flip).
- A subtle fullscreen toggle, top-right.

## Editing

Open `index.html` and edit — it's plain HTML/CSS/JS. Refresh the browser to preview. That's it.

## Deployment

Hosted free on **GitHub Pages**, served over HTTPS (Let's Encrypt) with *Enforce HTTPS* on.

Every push to `main` redeploys automatically:

```sh
git add -A
git commit -m "Update site"
git push
```

DNS lives at Squarespace (four `A` records → GitHub Pages, plus a `www` CNAME); email is on
Google Workspace and is unaffected by the web hosting.

## Analytics

The site reports to **Google Analytics 4** (Measurement ID `G-PXZ7EBKJJ6`), wired inline in the
`<head>` of `index.html`. No cookie banner — it tracks every visitor.

**Check the reports:** sign in at [analytics.google.com](https://analytics.google.com) with the
`fadelabs.ai` Google account, pick the **Fade Labs** property, then:

| Want to see… | Go to |
|---|---|
| Who's on the site *right now* | **Reports → Realtime** |
| Visitors, sessions, trends over time | **Reports → Life cycle → Acquisition** |
| Where they came from (search / social / direct / referral) | **Reports → Acquisition → Traffic acquisition** |
| Country, city, device, browser | **Reports → User → Demographics / Tech** |
| What they did on the page (scrolls, clicks, engagement) | **Reports → Engagement → Events** |

- **Enhanced Measurement** is on by default, so page views, scroll depth, outbound clicks, and
  engagement time are captured automatically — no extra code.
- Data shows up in **Realtime** within ~60 seconds; standard reports settle after 24–48 hours.
- Heads-up: **ad blockers** hide GA from a slice of technical visitors, so counts run a little low.

**Quick test that it's working:** open [fadelabs.ai](https://fadelabs.ai), then watch yourself appear
under **Reports → Realtime**.

---

© Fade Labs, Inc. · Stealth
