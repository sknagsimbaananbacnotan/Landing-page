# SK Free-Wifi Nagsimbaanan — Connected Page

This is the "You're Connected!" confirmation page shown after someone
successfully connects, with a 5-star feedback rating and a Done button.

## Setting this up on GitHub Pages (free HTTPS hosting)

1. **Create a new repository** on GitHub (e.g. `sk-wifi-connected`). It can
   be public or private — public is required for the *free* tier of GitHub
   Pages unless you have GitHub Pro/Team/Enterprise.

2. **Upload these files** to the repository:
   - `index.html` (required — this is the page itself)
   - `.nojekyll` (required — tells GitHub not to run its Jekyll build step,
     which can otherwise interfere with plain HTML/CSS/JS sites)
   - `Saranggola.mp3` — **add this yourself**, it isn't included here. Just
     drag the mp3 file into the same repository, in the same folder as
     `index.html`.

   Easiest way: on the repo page, click **Add file → Upload files**, drag
   all three in, and commit.

3. **Enable GitHub Pages:**
   - Go to the repo's **Settings** tab
   - Click **Pages** in the left sidebar
   - Under **Source**, choose the branch (usually `main`) and folder `/ (root)`
   - Click **Save**

4. **Wait about a minute**, then refresh that Pages settings screen — GitHub
   will show your live HTTPS URL, in the form:

   ```
   https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPO-NAME/
   ```

5. **Use that URL as your Omada landing page** — paste it into whatever
   field in your Omada Portal settings controls where visitors land after
   `/portal/auth` succeeds (often called "Landing Page" or similar).

## Notes

- Every time you upload a changed `index.html` to this repo, GitHub Pages
  updates automatically within a minute or two — no need to reconfigure
  anything.
- If the page loads but the music doesn't play, double check
  `Saranggola.mp3` was actually uploaded and that its filename matches
  exactly (case-sensitive) what `index.html` expects.
- Both logos (SK seal and PLDT Enterprise) are already embedded directly
  inside `index.html`, so you don't need to upload any image files.
