# Moore Electric — Work Portfolio

**What it is:** A gallery-first, single-page work portfolio for Moore Electric (Biloxi / Mississippi Gulf Coast). Every photograph is a real Moore Electric job photo from Devin's own library — no stock, no placeholders. Built to show the work and the proof: photos, the five named five-star Facebook reviews, and the HomeAdvisor rating, ending in one big call CTA.

**Page (`index.html`):**
- Hero — the golden-hour pier house photo, "Real work. Real photos.", call button.
- Rating badges — Facebook 100% Recommend · HomeAdvisor 4.9/5 (8 reviews, none below four stars) · written quotes.
- The Work — 10-photo gallery with captions (pier lighting, EV charger, panel replacement, the corroded meter-socket diagnostic find, security lighting, outdoor GFCI, ceiling fan/recessed, restaurant, shop build-out).
- Reviews — Michael Phan (Apr 2022), Diana Grant (Nov 2021), Pat Wylie (Oct 2021), Brandon Eldridge (Oct 2021), Henry Vanegas (Oct 2021), quoted from their Facebook reviews, plus the HomeAdvisor summary card.
- Services & service area — Biloxi, Gulfport, Ocean Springs, D'Iberville, Long Beach, Bay St. Louis.
- CTA band + footer linking the main site (https://228mooreelectric.com), Facebook (https://www.facebook.com/228MooreElectric), and (228) 224-9150 throughout.

**Tech:** Pure static HTML + one CSS file. No build step, no JavaScript, no external assets except Google Fonts (Anton / Inter / JetBrains Mono). Dark theme echoing 228mooreelectric.com (near-black, electric blue #19c8fa, volt #ffd400). Mobile-first with a sticky mobile call bar; semantic HTML, alt text on every photo.

**Images (`img/`):** Resized copies (max 1000px wide) of the curated gallery set from `mooreelectric-new/assets/gallery/`, plus:
- `og-image.jpg` — 1200×630 social card composited with PIL from `fb/photos/photo-040.jpg` (the pier house job photo).
- `hero.jpg` — 1600×900 crop of the same photo-040.

**Claims discipline:** Ratings and quotes are the recorded ones from the live site's review cards. No claim of state licensure, insurance, or an LLC appears anywhere (none is true yet).

**Publish:** Drop the folder contents on any static host. `og:image` is referenced as a relative path (`img/og-image.jpg`) — after publishing, swap it to the absolute published URL in `index.html` so social scrapers resolve it.
