NURSE PASSPORT — WEBSITE
========================
Static, deploy-anywhere (built for Netlify).

PAGES
  index.html          Landing page
  for-nurses.html     Nurse product page
  for-facilities.html Hospital / health-system page
  pricing.html        Pricing (free for nurses, 8–12% for facilities)
  about.html          Company / mission
  contact.html        Contact form (Netlify Forms ready)
  privacy.html        Privacy policy (template — have counsel review)
  terms.html          Terms of service (template — have counsel review)
  app.html            Sign-in / get-started gateway (front-end only)

SHARED
  styles.css          Entire design system + all components (edit once, every page updates)
  site.js             Mobile menu, scroll reveals, stat counters, FAQ
  assets/             Put hero-nurse.jpg here (see below)

TO DO BEFORE GOING LIVE
  1. Hero image: the landing page now uses a real cut-out nurse photo at
     assets/hero-nurse.png (extracted from your Switzerland flyer). An
     illustrated fallback is also included at assets/hero-nurse.svg.
     To swap in a different photo, replace assets/hero-nurse.png (a
     transparent-background PNG sits best on the right) — or change the
     hero <img> src in index.html. For a full-bleed photo-behind-text
     layout instead, ask and we'll switch the hero mode.
  2. app.html is the front-end gateway only — wire its form to your Supabase auth.
  3. Add a real og-image.png at site root for social previews.
  4. Legal pages are plain-language templates — review with counsel per jurisdiction.
  5. Contact form uses Netlify Forms (data-netlify="true"); it works automatically
     once deployed to Netlify. On other hosts, point the form action at your handler.

Nav and footer are repeated in each HTML file (standard for static sites).
Change them in one file, then copy into the others — or templatize later.
