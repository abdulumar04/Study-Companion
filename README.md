# DBA Study Companion

A study companion for DBA students: organise PDFs, Word files, slide decks and scans in folders; read them with highlighters, ink pens and notes; keep your timetable and deadlines; and train your reading speed and comprehension.

- Works in Chrome, Edge and Safari on Windows, Mac, iPad, iPhone and Android.
- Installable as an app and works offline after the first visit.
- No accounts and no servers: each person's materials, highlights, notes and calendar stay in their own browser on their own device. Nothing is uploaded.
- Open the **Guide** tab in the app for full instructions.

## Publish it with GitHub Desktop (one time)

1. In GitHub Desktop: **File → Add local repository…**, choose this folder. When asked, choose **create a repository**, then **Create repository**.
2. Press **Publish repository**. Untick **Keep this code private** (free GitHub Pages needs a public repository; the code is public, but nobody's data is in it).
3. On github.com, open the repository → **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, **Branch** to `main` and folder `/ (root)`, then **Save**.
4. After a minute or two the address appears at the top of that page, like `https://YOUR-USERNAME.github.io/dba-study-companion/`. That is the link to share.

**Choose the repository name once and keep it.** Each person's data is tied to the exact web address. If you rename the repository or change your GitHub username, the address changes and everyone's app will look empty (their data is still in the browser under the old address, but they would need to restore a backup at the new one).

## Updating the app

1. Replace `index.html` (and anything else that changed) in this folder.
2. In GitHub Desktop: write a short summary, **Commit to main**, then **Push origin**.
3. Users get the new version the next time they open the app while online. No hard refresh is needed, and their data is not touched.

If you change any file in `vendor/`, also change `VERSION` in `sw.js` (for example `dsc-v1` to `dsc-v2`) so devices fetch the new copy.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `vendor/` | PDF, Word, PowerPoint and spreadsheet readers, loaded only when first needed |
| `sw.js` | Offline support |
| `manifest.webmanifest`, `icon-*.png` | Install as an app |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
