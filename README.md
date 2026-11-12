# Hanif Al Fathoni — freelance website profile

Hugo + pinned PaperMod theme with local homepage, footer and CSS overrides. Indonesian content focuses on freelance website services; employment and education were updated from the LinkedIn PDF supplied by the owner on 8 November 2026. The private PDF is not included.

## Run locally

Use Hugo Extended 0.124.1 (matching `.github/workflows/hugo.yml`).

```sh
git submodule update --init --recursive
hugo server -D=false
```

Open the URL printed by Hugo. Production build: `hugo --minify`.

## Editing

- `layouts/index.html`: homepage layout, services, selected projects and workflow.
- `assets/css/extended/freelance.css`: responsive styling.
- `content/about.md`: current biography and experience.
- `content/portfolio.md`: project descriptions and screenshots.
- `hugo.yaml`: navigation, metadata and contact email.
- `layouts/partials/footer.html`: current-year footer.

Contact opens the owner's WhatsApp Business link with a short project enquiry. The phone number is present in the destination URL but not displayed as page text or an accessible label. No pricing, client testimonials or availability promises were invented. Certifications retain their recorded dates. Existing project screenshots are retained, and the unpublished blog draft remains a draft.

## Verification (8 November 2026)

- Hugo Extended 0.124.1 production build: passed.
- 151 internal links/assets/anchors across 9 generated HTML pages: passed.
- Chrome browser checks for `/`, `/about/`, `/portfolio/` at widths 1440, 390 and 320: passed; no horizontal overflow, broken images, browser errors or failed resources.
- Desktop and mobile homepage screenshots visually inspected.
- `git diff --check`: passed.

No production deployment or remote push performed. Email delivery, external profile/certificate availability and contact conversion have not been tested. Check project screenshots for any client information before publishing. The source ZIP includes the pinned theme so it can build without a submodule download.

## Anti-slop follow-up

The owner approved all eight findings from the AFTER audit. Homepage projects now use a compact list, decorative arrows were removed, navigation and standalone actions have at least 44px touch targets, and keyboard focus uses white on the navy contact panel. The image render hook obtains local image dimensions at build time and lazy-loads portfolio screenshots. CSS is consolidated and `DESIGN.md` records the visual decisions. Source changes were edited directly.

OBE-AI, Kerjaku and GenBI-Point now include the problem addressed and development scope based on source documentation. No publishable screenshots were found for these three projects in the inspected sources, so none were fabricated or added. The formal profile photo was supplied by the owner.

Latest verification: production Hugo build, 130 internal references, 12 responsive page/viewport checks, all homepage standalone targets, 13 keyboard stops, and all local portfolio image dimensions passed. Normal text palette contrasts range from 6.31:1 upwards; the contact focus indicator is 15.61:1 against navy. External-site availability and OS email handoff/delivery were not tested. Updated review reports and screenshots are provided separately in this chat's outputs folder.
