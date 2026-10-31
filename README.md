# Paul Clark — The Cipher Librarian

**Exploring cryptography, from historical ciphers to post-quantum security.**

Professional author website for **cipherlibrarian.com**, featuring *Secrets of the Cipher Museum*, a growing bookshelf, an About page, and connections to Cipher Museum and Crypto Lab.

## Publish with GitHub Actions

The deployment workflow is `.github/workflows/pages.yml`. It runs on every push to `main` and can also be started manually from the **Actions** tab. It regenerates the static pages, stages only website files, uploads the Pages artifact, and deploys it to the `github-pages` environment.

1. Open **Settings → Pages** and select **GitHub Actions** as the source.
2. In the same settings, set the custom domain to **cipherlibrarian.com**. With Actions, this repository’s `CNAME` file documents the intended domain; the domain must also be set in Pages settings.
3. At GoDaddy, use these website DNS records:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | systemslibrarian.github.io |

Keep mail and unrelated DNS records. Enable **Enforce HTTPS** when GitHub makes it available. Confirm a successful run in **Actions → Deploy author website to GitHub Pages** before treating a push as published.

No package install, API key, or runtime server is required. The workflow uses the repository’s scoped GitHub token and GitHub’s Pages deployment actions.

Official references: [Custom GitHub Pages workflows](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages) · [Custom domain configuration](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).

## Edit and maintain

- The published HTML, CSS, images, and fonts are committed at the repository root.
- Edit page copy in `scripts/build.py` and run `python3 scripts/build.py` to regenerate the HTML.
- Edit styles in `assets/site.css` and the mobile navigation in `assets/site.js`.
- Add new, real book titles to the bookshelf as they are ready. Keep release dates, prices, and purchase links factual.
- Replace the typographic author card with an approved real portrait when one is available. No stock or generated person is represented as Paul.

## Included pages

- Home
- Books
- Secrets of the Cipher Museum
- About Paul, including a brief statement of Christian faith
- Privacy and a custom 404 page

## Content and assets

The current book title, subtitle, description, excerpt, and cover came from Paul’s book files and the existing public museum companion on October 31, 2026. The book is marked **Forthcoming**. There are no invented reviews, prices, release dates, or purchase links.

Original code-native SVG illustrations connect historical ciphers and modern security. Images and fonts are served locally. DM Sans and Newsreader are included under their SIL Open Font Licenses in `assets/`.

© 2026 Paul Clark. Book text, cover, and site content are reserved by their respective rightsholders. Font licenses remain with the included font files.
