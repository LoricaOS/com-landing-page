# com-landing-page

The commercial / enterprise landing page for **[AspisOS](https://github.com/AspisOS)**,
served at **[aspisos.com](https://aspisos.com)** via GitHub Pages.

Counterpart to [`org-landing-page`](https://github.com/AspisOS/org-landing-page)
(the open project at aspisos.org). Static HTML/CSS, no build step. Same dark
brand, a teal "assurance" accent to mark the enterprise side.

## Message

Open core, paid assurance — the model is honest and the mission is the pitch:
revenue funds independent security audits and paid driver/kernel/userspace
engineering that lands in the open core. Built to break even, not to extract.

## Layout

```
index.html      the page (hero, model, mission, enterprise offerings, contact)
style.css       styling (dark brand, teal accent)
assets/         shared brand art (logo, wallpaper, favicon)
CNAME           aspisos.com
.github/workflows/deploy.yml   publishes to GitHub Pages on push to main
```

## Deploying

Push to `main` runs the Pages deploy. One-time: repo Settings → Pages → Source =
GitHub Actions. DNS for aspisos.com (apex A records to Pages + `www` CNAME) is set
separately; the `CNAME` file claims the domain. The contact CTA points at
`enterprise@aspisos.com` — wire that mailbox up when ready.

## Local preview

```sh
python3 -m http.server 8001
```
