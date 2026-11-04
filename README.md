# Personal research website

A plain HTML/CSS academic homepage. No build step: edit the files and push.

## Files

- `index.html`: all page content (about, news, publications, projects, teaching)
- `style.css`: styling. Change `--accent` at the top to set your color.
- `assets/`: images. Replace `profile.svg` with your photo (e.g. `profile.jpg`) and update the `src` in `index.html`.
- `cv.pdf`: add your CV here (the CV links already point to it)
- `.nojekyll`: tells GitHub Pages to serve the files as-is

## Deploy on GitHub Pages

1. Create a new **public** repo on GitHub named exactly `<your-username>.github.io`.
2. Push these files to it:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**.
4. After a minute or so the site is live at `https://<your-username>.github.io`.

Every later `git push` updates the site.

## Adding a publication

Copy one `<li class="pub">…</li>` block in `index.html`, then edit the title, authors, venue and links. Wrap your own name in `<span class="me">` so it shows in bold.
