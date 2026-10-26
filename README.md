# ca-case-studies

Conversion Advantage case study pages, published with GitHub Pages.

Live site: https://conversionadvantage00.github.io/ca-case-studies/

| Page | URL |
|---|---|
| Index | https://conversionadvantage00.github.io/ca-case-studies/ |
| Shamwari | https://conversionadvantage00.github.io/ca-case-studies/shamwari-case-study.html |
| Mantis Collection | https://conversionadvantage00.github.io/ca-case-studies/mantis-collection-case-study.html |
| La Motte | https://conversionadvantage00.github.io/ca-case-studies/la-motte-case-study.html |
| Volkswagen | https://conversionadvantage00.github.io/ca-case-studies/volkswagen-case-study.html |

- Each page is one self-contained HTML file, with fonts and images embedded, so there are no other folders to upload.
- Every page has `noindex`, so search engines don't list them. They're meant to be shared directly with prospects.
- Each case study's "more success stories" button links back to the index page.
- The outreach email's "read the case study" links point to these URLs. **Don't rename the files**, or those links will break.
- Master copies and build notes live in Google Drive: `Claude Code/conversion-advantage/Outreach/`.

## Landing page (index.html)

`index.html` is the success stories hub. It has a large "success stories." heading, a 2×2 grid of results cards and a "want results like these?" section. Editing notes are at the top of the `<body>` in a comment. Change only the card copy, images, links and video attributes; leave the styles and structure alone.

**Card figures must match the case study page each card links to:**

| Card | Figure on the card |
|---|---|
| shamwari | +84.55% conversions from Google Ads in 6 months |
| mantis collection | +10.6% total sales, 2024 vs 2025, with the first measurable revenue from Google Ads |
| la motte | +113% revenue in 6 months from a full digital retainer |
| volkswagen | +119% click-through rate from Google Ads in 6 months |

### Adding video to a tile

Every tile already supports video. Each `<a class="tile">` has two empty attributes:

- `data-video="…"`: the URL of an MP4 or WebM file. It plays muted, loops, and only plays while the tile is on screen.
- `data-youtube="…"`: a YouTube video ID or link. It plays as a muted, looping background.

Fill in one of them and leave the `<img>` in place. The photo stays as the poster frame, and it's what shows if the video can't play (reduced-motion setting, data saver, autoplay blocked).

Videos already on the staging site, for later:

| Client | Source on staging |
|---|---|
| Shamwari | YouTube `ALjTPC-LVJ8` |
| Mantis | `wp-content/uploads/2026/03/A-collection-of-curated-destinations-inspired-by-sustainable-adventures-welcome-to-Mantis.mp4` |

Video files must live at a public URL. The staging site is temporary, so host final videos on the live website, on YouTube, or in this repo. GitHub rejects files over 100 MB, so keep MP4s small.
