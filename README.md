# Justin Lebon — UX Research Portfolio

A static site (plain HTML/CSS/JS, no build step) built from your UX research
portfolio deck. Five pages: `index.html` (home) plus one page per case study.

## Files

```
index.html                 Home page (hero + case study grid + about)
club-peloton.html           Case study: Club Peloton
subscription-revenue.html   Case study: Dual App Sign-up
post-class.html              Case study: Post Class Concepts
oculus-vr.html                Case study: Oculus Pro Usability
style.css                   All styling
script.js                   Scroll-reveal animation
```

## Before you publish

1. **Swap the placeholder email.** Every page uses `hello@justinlebon.com` —
   find-and-replace it with your real email in all five `.html` files.
2. **Add a LinkedIn/resume link** in the nav or footer if you'd like one —
   currently only an email contact link is included.
3. Optional: add real screenshots/mockups from your Figma files into each
   case study — right now the site is text/data-only, matching the deck.

## Deploy with GitHub Pages (free)

1. Go to [github.com/new](https://github.com/new) and create a new repository
   (e.g. `portfolio`). Keep it public.
2. Upload all the files in this folder to the repo — either drag-and-drop
   them on the GitHub website ("Add file" → "Upload files"), or via git:
   ```
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch",
   branch `main`, folder `/ (root)`. Save.
5. Wait 1–2 minutes, then your site will be live at:
   `https://YOUR-USERNAME.github.io/portfolio/`

## Custom domain (optional)

In **Settings → Pages**, add your domain under "Custom domain" and follow
GitHub's DNS instructions (a `CNAME` record pointing to
`YOUR-USERNAME.github.io`). GitHub issues a free HTTPS certificate
automatically once DNS propagates.

## Making changes later

Everything is plain HTML/CSS — no build tools required. Edit the `.html`
files directly (each case study's content lives right in its own file), edit
`style.css` for design changes, then commit and push — GitHub Pages
redeploys automatically within a minute or two of any push to `main`.
