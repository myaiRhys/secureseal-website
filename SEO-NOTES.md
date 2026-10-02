# SecureSeal — SEO Notes

On-page SEO and content optimisation applied to `index.html` plus supporting files.

## What was implemented

**Metadata & indexing**
- Keyword-led `<title>` and tightened meta description (~155 chars).
- `lang="en-ZA"`, canonical URL, `robots` directive, author, keywords.
- Local-SEO geo tags (region `ZA-WC`, Cape Town coordinates).
- Full Open Graph set (url, image, site_name, locale, product price/availability) + Twitter `summary_large_image`.

**Structured data (JSON-LD)** — drives Google rich results:
- `Product` with `Offer` (ZAR 199, InStock, 30-day return policy). No ratings or reviews until real, verifiable customer reviews exist.
- `FAQPage` mirroring the 7 visible FAQ items (eligible for FAQ rich snippets).
- `Organization` (legal name True Motives CC, Cape Town, area served South Africa).

**Content / keyword targeting**
- Hero kicker + sub-copy now carry primary terms: *fabric waterproofer, tent seam sealer, rooftop tent, awnings, canvas, tarps, made in South Africa*.
- "Works on" expanded with long-tail surfaces: bell tents, caravan awnings, ripstop & PVC, bakkie covers.
- Added "Do you ship across South Africa?" FAQ (kept page + schema in sync).

**Crawl & social assets**
- `favicon.svg` (SVG favicon), `og-image.svg` (1200×630 share card).
- `robots.txt` (+ sitemap reference) and `sitemap.xml`.

## Action items before / after launch

1. **Domain** — the site currently lives at `https://myairhys.github.io/secureseal-website/`, and every absolute URL (canonical, og:url, schema, `robots.txt`, `sitemap.xml`) points there so Google indexes the page that actually exists. When `secureseal.co.za` goes live, find/replace `https://myairhys.github.io/secureseal-website/` with `https://secureseal.co.za/` in `index.html`, `robots.txt` and `sitemap.xml`.
2. **Social image** — `og-image.jpg` (1200×630) is rendered from `og-image.svg`; social and product URLs use the JPG. Re-export it if the SVG changes.
3. **Search Console** — verify the property and submit `sitemap.xml`; create a Google Business Profile (Cape Town) for local/maps traffic.
4. **Reviews** — there are none yet. Only add a reviews section and `AggregateRating` once real customers have reviewed the product, and keep schema in sync with what's on the page.
5. **Validate** — run the page through Google Rich Results Test and the Schema Markup Validator after deploy.

## Off-page / traffic growth (not code)
- Target high-intent SA keywords with content: e.g. a short "how to waterproof a canvas tent" guide, "rooftop tent leaking fix".
- List in SA marketplaces / 4x4 & camping forums; partner with overlanding YouTubers.
- Collect and display verified customer reviews to strengthen rating signals.
