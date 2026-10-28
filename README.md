# Wen Wang — Academic Website (static GitHub Pages version)

This is a NEW self-contained implementation inspired by the spare, research-first aesthetic of the Pascal Michaillat economist website. It is **not** a copy of the Hugo source. No Hugo build is required.

## Quick publishing instructions for `wenwang.github.io`

1. Download and unzip this package. Keep the **contents** of this folder ready.
2. In GitHub, open `https://github.com/wenwang/wenwang.github.io` (provided your GitHub username is `wenwang`). Download the existing repository as a backup first.
3. Replace the old Hugo project files in the repository with the contents of this package. **Do not delete the repository or rename it.** The easiest way is GitHub Desktop: clone, delete old files in the local repository directory (but keep `.git`), copy these files in, commit and push. If uploading via the GitHub browser, ensure old Hugo-related files/workflows are removed as well.
4. At **Settings > Pages**, set **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**. Save. Old Hugo Actions workflows must not keep deploying to Pages.
5. Visit `https://wenwang.github.io` once GitHub Actions shows a successful Pages deployment. The file `index.html` must be in the repository root.

## Edit your information
- `index.html`: biography, homepage and highlighted research.
- `research.html`: publications, working papers, research in progress.
- `teaching.html`: courses.
- `cv.html`: CV link (currently links to a public July 2025 PDF; replace with latest approved CV).
- `contact.html`: institution, email, links.
- `assets/style.css`: styling.
- Portrait: add `assets/portrait.jpg` and replace the `div class="photo"` placeholder on the homepage with `<img class="portrait-img" src="assets/portrait.jpg" alt="Wen Wang portrait">`.

**Before publishing:** Verify every publication year, title and authorship; check working paper circulation status. The content reflects a draft and has NOT been individually verified against your latest CV. Paper PDFs are not included; attach only documents you wish to share publicly. Review public professional details before launch.

## Connect an existing Wix-registered domain (optional; do this after github.io works)

1. Under **Settings > Pages > Custom domain** type your Wix-registered domain.
2. At Wix **Domains > Manage DNS records**, set GitHub Pages' current documented apex A records, and `www` CNAME to `wenwang.github.io`. Follow the current GitHub documentation at https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
3. Preserve email MX/SPF/DKIM records. Enable **Enforce HTTPS** once GitHub allows it.
4. If using a custom domain, create a file named `CNAME` (no extension) containing that domain. A `CNAME.example` is provided as illustration only and is not active. Update canonical URLs in the HTML to the new domain if desired.

Note: Uploading the ZIP as a single file to GitHub does not publish a website. Extract and upload its inner files.
