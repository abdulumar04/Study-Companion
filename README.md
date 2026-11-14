# DBA Study Companion

A free study tool for business-school students: organise PDFs, Word files, slide decks and scans in folders; read them with highlighters, ink pens and notes; listen to them read aloud; keep your timetable and deadlines; and train your reading speed and comprehension.

- Works in Chrome, Edge and Safari on Windows, Mac, iPad, iPhone and Android.
- Installable as an app and works offline after the first visit.
- No accounts, no analytics and no server. Each person's materials, highlights, notes and calendar stay in their own browser on their own device. Optional sync stores them in a hidden app folder in the person's **own** Google Drive; nothing is ever sent to the maintainer.
- Open the **Guide** tab in the app for full instructions.

**Independent project.** Not affiliated with, or endorsed by, any school, university, Microsoft, Google or Apple. Provided "as is" with no warranty. See [legal.html](legal.html) for the terms of use and privacy notice.

## Licence

The app's own code is under the MIT License (`LICENSE`). Bundled third-party components (`vendor/`, `fonts/`) keep their own licences; see `THIRD-PARTY-NOTICES.txt`.

## Updating the app

1. Replace `index.html` (and anything else that changed) in this folder.
2. In GitHub Desktop: write a short summary, **Commit to main**, then **Push origin**.
3. Users get the new version the next time they open the app while online. Their data is not touched.

If you change any file in `vendor/` or `fonts/`, also change `VERSION` in `sw.js` (for example `dsc-v2` to `dsc-v3`) so devices fetch the new copy.

**Keep the repository name and your GitHub username unchanged.** Each person's data is tied to the exact web address.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `legal.html` | Terms of use, privacy notice, licences |
| `vendor/` | PDF, Word, PowerPoint and spreadsheet readers, loaded only when first needed |
| `fonts/` | Self-hosted fonts (no request to Google Fonts) |
| `sw.js` | Offline support |
| `manifest.webmanifest`, `icon-*.png` | Install as an app |
| `LICENSE`, `THIRD-PARTY-NOTICES.txt` | Licences |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
