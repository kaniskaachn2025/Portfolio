# B.S. Kaniskaa — Portfolio

A single-page portfolio site built from my resume: profile, skills, education,
one deployed AWS project, certifications, and achievements.

**Live structure:**
- `index.html` — page content
- `style.css` — design system (colors, type, layout)
- `script.js` — footer year + gentle scroll-reveal
- `assets/BS_Kaniskaa_Resume.pdf` — downloadable résumé (linked from the nav and hero)

## Publish it on GitHub Pages (free hosting)

**1. Create the repository**
- Go to [github.com/new](https://github.com/new)
- Repository name: `portfolio` (or anything — see naming note below)
- Set it to **Public**
- Don't initialize with a README (you already have one)
- Click **Create repository**

**2. Upload the files**
Easiest way (no terminal needed):
- On your new repo's page, click **"uploading an existing file"**
- Drag in `index.html`, `style.css`, `script.js`, `README.md`, and the `assets` folder
- Commit the files

Or with Git from your computer:
```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/<your-username>/portfolio.git
git push -u origin main
```

**3. Turn on GitHub Pages**
- In your repo, go to **Settings → Pages**
- Under "Build and deployment", set **Source** to `Deploy from a branch`
- Branch: `main`, folder: `/ (root)` → **Save**
- GitHub will give you a live URL after a minute, usually:
  `https://<your-username>.github.io/portfolio/`

**Naming note:** if you name the repo `<your-username>.github.io` exactly,
your site becomes your root domain (`https://<your-username>.github.io/`)
instead of living under a `/portfolio/` sub-path.

## Editing later
- Update your résumé PDF anytime by replacing the file in `assets/` (keep the same filename, or update the link in `index.html`).
- Colors and fonts live at the top of `style.css` under `:root` if you want to retheme.
- Add a new project by copying the `<section id="project">` block in `index.html`.
