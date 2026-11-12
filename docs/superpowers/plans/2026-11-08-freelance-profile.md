# Freelance profile implementation plan

Goal: Turn the existing Hugo website into a personal brand for website development services.
Architecture: Keep the pinned PaperMod submodule; override the homepage and extend its CSS. Preserve existing content URLs and draft status.
Source: User-approved personal brand + website services direction; Profile.pdf supplied on 8 November 2026.

- [x] Build an Indonesian homepage with services, existing projects, process, about and contact.
- [x] Update About from the supplied LinkedIn profile; preserve project facts and translate portfolio.
- [x] Use the supplied email for contact; do not publish the PDF or add unverified claims, rates or availability.
- [x] Build using Hugo 0.124.1, check generated internal links and mobile/desktop layout where browser tooling allows.
- [x] Package a reviewable source archive and document verification and remaining limits.

Design: warm off-white, dark ink, orange accents, large editorial heading, rounded project previews. Lightweight static HTML/CSS, keyboard focus, responsive grids, reduced motion. Keep blog URLs but remove empty blog/tags from primary navigation. Keep employment clearly separate from freelance services. Dates come from the document, not its automatically calculated durations. No push or production deployment.
