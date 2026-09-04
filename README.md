# Dance Foundations — OER Course Collection (GitHub Pages)

This folder is a ready-to-publish static website version of the Word document,
converted to HTML with a table of contents, styling, and the original images.

## How to publish it on GitHub Pages

1. **Create a new repository** on GitHub (e.g. `dance-foundations-oer`). Public repos get free GitHub Pages hosting.
2. **Add these files to the repo**, keeping the folder structure exactly as-is:
   ```
   index.html
   assets/style.css
   assets/images/img1.jpg ... img6.jpg
   ```
   You can drag-and-drop them in the GitHub web UI ("Add file" → "Upload files"), or use git:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
3. **Enable Pages**: In the repo, go to **Settings → Pages**. Under "Build and deployment", set
   **Source** to "Deploy from a branch," pick the **main** branch and **/ (root)** folder, then Save.
4. Wait a minute or two, then your site will be live at:
   `https://<your-username>.github.io/<your-repo>/`

No build step, Jekyll config, or extra tooling is required — it's plain HTML/CSS.

## Notes / things worth checking before you publish

- A few internal Word comments/tracked-changes markers may not have carried over — worth a skim of `index.html`.
- External links (YouTube videos, articles, the Microsoft Sway weekly lessons) were preserved as-is.
- If you'd rather have each chapter (Ballet I, Tap I, Hip Hop I, etc.) as its own page instead of one long
  scrolling page, that's a straightforward follow-up — just ask.
