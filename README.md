# Zayan Iqbal — Islamic Creative Portfolio

Four-page responsive, dark editorial portfolio with pricing in PKR/USD, Islamic flyer add-on (Rs. 4,000 / $30), services, booking inquiry, and editable Git-based CMS.

## Preview locally

1. Open a terminal in this folder.
2. Run `python -m http.server 8000` (Python must be installed).
3. Open http://localhost:8000

**Do not open HTML files with a `file://` URL:** browsers restrict the JSON content fetching used here.

## Publish FREE (subject to provider terms/limits)

1. Create a GitHub repository and upload *all* files/folders **including hidden `.pages.yml`**.
2. Connect GitHub repo to [Cloudflare Pages](https://pages.cloudflare.com/). Use no build command, output directory `/` (root) for this static site.
3. Cloudflare issues a public `*.pages.dev` URL. Optionally add your own purchased domain.
4. Sign in at [Pages CMS](https://app.pagescms.org/) with GitHub; authorize your repository. The `.pages.yml` enables editing Site settings, homepage hero image, project images, packages, and flyer price.
5. Make your content edits in Pages CMS; CMS commits changes to GitHub, then Cloudflare auto-deploys.
6. Replace all project placeholders with YOUR OWN portfolio images and set a real contact email, Instagram, LinkedIn, WhatsApp and (optionally) Calendly booking URL.
7. For Search Console, submit the deployed public URL and domain. A sitemap can be added once the canonical domain is known.

## Editing home banner

Pages CMS → Site settings & homepage → Homepage hero banner image → upload → Save.

## Editing portfolio

Pages CMS → Portfolio projects → Projects → add/edit an item, including category, image, featured toggle → Save. The home page uses `featured=true`, portfolio shows all.

## Booking limitation

The booking form is intentionally `mailto:` based, **not an automated backend**. Nothing is emailed to you until visitor sends the prepared message in their email application. Connect a real serverless form handler or a third-party hosted form service for automatic lead submissions. Add your Calendly link to Site settings for appointments.

## Pricing clarification

PKR and USD prices are separately configured market-facing starting rates, not live foreign-exchange conversions. Flyer starting price is Rs. 4,000 in Pakistan and $30 internationally, negotiable. Bundles are per creative package, not monthly recurring unless you update content.

## Technical/SEO notes

Static HTML/CSS/JS, no tracking scripts or third-party analytics. Google Fonts CDN used; self-host fonts if desired. Responsive, accessible form labels, search descriptions. Add a custom canonical URL, sitemap and Search Console verification after publishing. Pages CMS permissions rely on your GitHub permissions. Keep your GitHub login protected with 2FA.
