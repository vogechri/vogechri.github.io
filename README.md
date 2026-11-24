# Personal homepage

Static, single-file homepage (`index.html`), no build step.

## Publish with GitHub Pages
1. Sign in to your **personal** GitHub account (`vogechri`), not the Microsoft-managed account.
2. Create a public repository named `vogechri.github.io`.
3. Push this folder:
   ```bash
   git init -b main
   git add index.html README.md
   git commit -m "Add homepage"
   git remote add origin https://github.com/vogechri/vogechri.github.io.git
   git push -u origin main
   ```
4. In the repository, open **Settings → Pages** and select **Deploy from a branch**, `main`, `/ (root)`.
5. The site appears at https://vogechri.github.io after about a minute.

## Editing
- Publications are plain HTML blocks inside `index.html`; copy an existing `<div class="pub">` block to add one.
- Paper thumbnails live in `images/` (cropped from each paper's first figure); reference them with
  `<img class="thumb" src="images/<name>.jpg" alt="...">` in place of a `venue-tag` div.
- Profile photo: `images/photo.jpg` is shown by default; `images/photo_hover.jpg` fades in on mouse-over.
  Replace either file (square images work best) to change them.
