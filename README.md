# k-eet.github.io

Source for my personal site, published with GitHub Pages at **<https://k-eet.github.io/>**.

It is a single self-contained page: a contact card and a short list of selected work,
built to be opened on a phone after meeting someone in person.

## What's in here

| Path | What it is |
| --- | --- |
| `index.html` | The whole site — markup, inline CSS and a small script, no build step |
| `fonts.css` | Cormorant Garamond + Lora, inlined as base64 woff2 so the page makes zero external requests |
| `_config.yml` | Jekyll config (`jekyll-theme-minimal`). `index.html` takes precedence, so the theme is effectively unused |
| `og-image.png` | 1200×630 link preview card, rendered from `index.html`'s palette and fonts |
| `assets/` | CV and certificate files served by the page |

The page offers a WhatsApp message, a generated `.vcf` contact download, an email link,
the CV as a download, and links out to LinkedIn and GitHub.

## Selected work

The projects linked from the page live in a separate repository,
[K-eet/Portfolio_Projects](https://github.com/K-eet/Portfolio_Projects):

- [UK Tech Outbound](https://github.com/K-eet/Portfolio_Projects/tree/main/UK%20Tech%20Outbound) — ideal-customer-profile and target-account scoring over the Companies House register
- [Ecommerce Data Analytics](https://github.com/K-eet/Portfolio_Projects/tree/main/Ecommerce%20Data%20Analytics) — ETL design, customer lifetime value and churn analysis on transactional retail data
- [Financial Analysis](https://github.com/K-eet/Portfolio_Projects/tree/main/Financial%20Analysis) — Tesla, BYD and Ford compared from SEC EDGAR filings

## CV and certifications

- [Lee-Keet-Men-CV.pdf](assets/Lee-Keet-Men-CV.pdf) — the CV the site links to
- [Google Data Analytics certificate](assets/Coursera_Google_Data_Analytics_Certificate.pdf) ([image](assets/Data_Analytics_Cert.jpg))

## Working on it

There is no build step. Open `index.html` in a browser, or serve the folder:

```sh
python -m http.server 8000
```

To update the site: edit the markup in `index.html` directly, and replace
`assets/Lee-Keet-Men-CV.pdf` to publish a new CV. Pushing to `main` deploys.
