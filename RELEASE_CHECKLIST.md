# Release checklist — Rohme Clipping v2.0.14 (clean repo, 23 Nov 2026)

Do these steps once, in order, on the GitHub account `gagang2325` (email `gagangaming25@gmail.com`). Nothing here publishes anything by itself.

**IMPORTANT — no GitHub Releases, ever.** GitHub auto-adds "Source code (zip)" / "Source code (tar.gz)" links to EVERY release and they cannot be removed. The friend download is hosted on Google Drive instead, and this repo holds ONLY the website files. Never push app source code to this repo, and never create a release here.

1. **Connect Muse to GitHub.** In the Muse chat, open the GitHub connect link and sign in as `gagang2325`. Then open the "Select repositories" link and install the Muse GitHub App — choose **All repositories** (there are none yet, so the repo created in step 2 is covered).
2. **Create the repo.** On GitHub, create a new **public** repository named `rohme-clipping`. Leave it empty (no README, no .gitignore, no licence).
3. **Upload these files.** Upload everything from this folder (`index.html`, `version.json`, `README.md`, `.nojekyll`, `RELEASE_CHECKLIST.md`, `favicon.svg`, `sitemap.xml`, `robots.txt`) to the repo's main branch. Nothing else — no app source, no zips, no Setup.exe.
4. **Enable GitHub Pages.** In the repo, go to Settings → Pages. Under "Build and deployment", choose "Deploy from a branch", branch `main`, folder `/ (root)`. Save. The site will be live at `https://gagang2325.github.io/rohme-clipping/`.
5. **Point the app at it.** In the Rohme Clipping app, open Settings → Updates and paste:
   - Update check URL: `https://gagang2325.github.io/rohme-clipping/version.json`
   - Download URL: `https://drive.google.com/file/d/1APDTBYrDNfBwHrc09JbK6YEnEQ6BDrDg/view?usp=drivesdk`
6. **Test.** Open the site, click Download, and confirm the Setup.exe downloads from Drive. In the app, use "Check for updates" and confirm it finds v2.0.14.

Notes:
- The app's in-app update check reads `version.json` from the Pages URL. The download itself comes from Google Drive (file shared "Anyone with the link").
- SEO: the page has a keyword title, meta description, canonical URL, Open Graph + Twitter cards, SoftwareApplication and FAQ structured data, `sitemap.xml` and `robots.txt`. Google still needs days to index a brand-new site — ranking first takes time and real links, it cannot be forced on day one.
- For the next version: upload the new Setup.exe to Google Drive, share it "Anyone with the link", then update `download_url` in `version.json` (and the version badge, download button and footer in `index.html`, plus the JSON-LD `softwareVersion` and `latest`), push to main. No release is ever created.
- History: the previous repo of this name was deleted on 23 Nov 2026 because its deleted `source` branch commits were still publicly reachable by SHA. This repo was recreated clean and has never held app source.
