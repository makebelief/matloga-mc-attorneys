# Matloga MC Attorneys Inc. — independent website concept

## Design and technology
Static HTML + CSS + vanilla JavaScript. Faithfully adapted from the established Wakili wa Tech South African production architecture. DM Sans body, Manrope headings. No build step. Nine pages including 404.

## Verification and approvals
**Independent, unapproved concept.** All pages remain noindex while robots.txt permits social preview crawlers to read public pages and the Open Graph image. Do not publicly index or call the official firm site until the client approves.

- User supplied: firm logo designs and three attorney photographs. Each different portrait is used exactly once: Home, About, Our Attorney. Logo repeats for branding. Photo ownership and publication consent must be confirmed.
- Public Facebook listing https://www.facebook.com/61589848811852/ identifies firm as Matloga MC Attorneys Inc., Centurion, phone +27 71 566 7001, public email matlogamcattorneys@gmail.com and criminal law, civil law, family law, labour matters, unlawful arrest.
- A publicly indexed LinkedIn profile for Matloga Mahlatsi reports Matloga MC Attorneys Inc. as an employer, but we do **not** attribute the pictured attorney’s identity, qualifications or admission status; firm should confirm.
- Unconfirmed: attorney's full identity & biography, precise office address, office hours, actual WhatsApp registration, rights to supplied portrait/brand, practice particulars and firm approval. Do not use contact details of similarly named Matloga/NG Matloga law firms.
- Contact form creates a **mailto: email draft** to matlogamcattorneys@gmail.com. The visitor must send the message in their email client; there is no backend email processing. Call button works via tel:. WhatsApp floating button uses publicly listed phone number but **WhatsApp account availability not verified**.
- Embedded Google Maps displays Centurion area only — NOT an accurate office pin. Update when street address confirmed.
- Pexels stock photo URLs have distinct image IDs across every content slot. External availability/license not independently validated; see PHOTO-SOURCES.md. Stock people are NOT firm staff.
- Google Fonts and Maps depend on internet connection.

## Preview
In root run: `python3 -m http.server 8000`. Open http://localhost:8000/. No npm or build needed.

## Publication / SEO
After actual client consent: verify assets and firm details, replace general map with verified address, choose official host, update page-specific canonical and OG URLs / JSON-LD @id / sitemap, remove noindex only after consent, confirm the approved final canonical host, and rebuild sitemap.

## GitHub / Vercel
Run `gh repo create matloga-mc-attorneys --private --source=. --remote=origin --push` in the checked-out project after normal git commit if no repo exists; then `npx vercel --yes` for a preview. Never create a public repo, publish production, or enable indexing before permissions.


## WhatsApp / Facebook link preview (version 3)
- All eight primary pages and 404 include absolute HTTPS Open Graph / Twitter image URLs pointing to `/assets/matloga-mc-share-v3.jpg`. The 1200×630 JPEG contains the verified client-supplied firm logo and the client-supplied attorney photo without replacing either.
- `robots.txt` allows social crawlers to fetch the pages/image. `meta name="robots" content="noindex,..."` continues to protect this unapproved outreach concept from Google indexing; these are separate settings.
- Test `https://matloga-mc-attorneys.vercel.app/` AND `https://matloga-mc-attorneys.vercel.app/assets/matloga-mc-share-v3.jpg` after **production** deployment. Verify the WhatsApp thumbnail on a fresh share; platform cache can delay updates. To request a new URL from WhatsApp, try sharing `https://matloga-mc-attorneys.vercel.app/?share=v3`.
- This is a configuration fix and package QA, not proof of a WhatsApp preview until tested from a deployed site in the WhatsApp app.
