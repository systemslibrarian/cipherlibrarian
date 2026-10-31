# Paul Clark — The Cipher Librarian

**Exploring cryptography, from historical ciphers to post-quantum security.**

Professional author website for **cipherlibrarian.com**, featuring *Secrets of the Cipher Museum*, a growing bookshelf, an About page, and connections to Cipher Museum and Crypto Lab.

## Publish with GitHub Pages

The site is ready to serve directly from this repository; no build service, package install, API key, or runtime server is required.

1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/(root)**, then **Save**.
4. Set the custom domain to **cipherlibrarian.com** and save it before changing DNS.
5. At the domain provider, set the following website DNS records:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | systemslibrarian.github.io |

Replace conflicting website records for those same names as appropriate. Keep mail and other unrelated records. Enable **Enforce HTTPS** when GitHub makes it available.

Official references: [GitHub Pages publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) · [Custom domain configuration](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).

These instructions prepare publication. Repository contents alone do not prove that Pages, DNS, or HTTPS is active.

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
