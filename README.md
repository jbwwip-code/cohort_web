# cohort_web

Landing page for **Cohort** — the campus feed, group chat, and club board for UMD students who are tired of scrolling alone. No algorithm deciding who you meet, just your campus, out loud.

## What's on the page

1. **Campus Feed** — one big message board for the whole campus, shown as a chalkboard of pinned posts.
2. **Mutuals** — chat with friends you already know, or get matched with someone new who shares your interests.
3. **Communities** — boards for official orgs and unofficial crews, plus an all-campus events list.
4. **CTA** — closing "Your campus is louder than your feed." section.

## Project structure

```
.
├── index.html              # the whole page (HTML + inline CSS)
└── assets/
    ├── blackboard.png       # chalkboard in the Campus Feed section
    ├── brokenPaper.png      # torn-paper section edges
    └── bubbleBackground.png # sky background for the CTA section
```

## Running locally

It's a static page with no build step. Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

Deploy `index.html` together with the `assets/` folder — the images are referenced by relative path and won't load without it. Fonts (Bricolage Grotesque, Caveat) load from Google Fonts.
