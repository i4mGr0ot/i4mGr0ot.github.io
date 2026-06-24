# Ashray Saxena — Personal Website

A fast, static, multi-page personal site. No build step, no frameworks, just HTML and CSS, so it loads instantly and hosts anywhere.

## Pages
- `index.html` — Home (hero, currently/upcoming, selected work, about)
- `research.html` — Research
- `projects.html` — Projects
- `entrepreneurship.html` — Entrepreneurship
- `experience.html` — Experience, Leadership, Teaching, Achievements, Contact

## Before you publish — 3 quick edits

1. **Add your photo.** Replace `assets/img/portrait.jpg` with your own portrait. Keep the same filename, or update the `src` in `index.html`. A vertical (4:5) image around 900×1125 px looks best.

2. **LinkedIn and GitHub links are already wired in** (linkedin.com/in/ashraysaxena and github.com/i4mGr0ot). Edit them in the `.html` files only if they change.

3. **Add your CV when ready.** Drop the PDF into `assets/`, then add a button wherever you like, for example in the hero of `index.html`:
   `<a class="btn btn-ghost" href="assets/Ashray_Saxena_CV.pdf" target="_blank">Download CV</a>`

## Publish on GitHub Pages

1. Create a new public repo. For a site at `https://YOUR-USERNAME.github.io`, name the repo exactly `YOUR-USERNAME.github.io`. (Any other name gives `https://YOUR-USERNAME.github.io/repo-name/`.)
2. Upload the **contents** of this folder (so `index.html` sits at the repo root, not inside a subfolder).
3. In the repo, go to **Settings → Pages**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`, and save.
4. Wait a minute, then visit your URL. Done.

### Using git from the command line
```bash
cd website
git init
git add .
git commit -m "Personal site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```

## Custom domain (optional)
In Settings → Pages add your domain, then create a `CNAME` file in the repo containing just the domain. Point your domain's DNS to GitHub Pages per their docs.

## Notes
- Fonts (Fraunces + Inter) load from Google Fonts; an internet connection shows them, otherwise the site falls back to system fonts gracefully.
- All figures are your own research and project outputs.
- Colours, spacing and type live in `assets/css/style.css` if you want to tweak the look.
