# Steven Vincent Psychotherapy — six-page redesign (integrated)

This is a separate deployment-ready static-site candidate, derived from the approved
mockups and the original GitHub repository ZIP. It DOES NOT change the live site.

Pages: `index.html`, `about.html`, `therapy.html`, `tools-for-change.html`,
`fees.html`, `contact.html`.

## Integration completed
- Original Formspree action retained: `https://formspree.io/f/xyeyllew`.
- Original contact form POST fields retained: `name`, `email`, `phone`,
  `preferred_contact`, `message`, and `_subject`.
- Original therapy room photograph reused (`assets/therapy-room.webp`).
- Exact transparent Psychology Today badge from your existing site reused
  (`assets/psychology-today-badge.png`).
- Existing Cloudflare Pages `_headers` file retained.
- Homepage forest image has a subtle zoom; all five other pages have static forest images.
- Approved page wording retained, including text-only Tools for Change without a subtitle.
- Existing birds / branches and obsolete duplicated site pages not included.

## IMPORTANT: Before publishing
1. Back up the current production branch. Keep this in a staging/preview deployment
   until you are happy with the result.
2. Inspect the six pages on desktop and phone, especially image cropping, text size,
   and CTA links. The new consultation links direct to `contact.html`.
3. The contact form now uses the REAL Formspree endpoint. A submitted test message
   will be a REAL form submission. Test end-to-end after deploying to a preview URL;
   verify receipt in your inbox or Formspree dashboard.
4. Check any required professional/registration claims and current fees before launch.
5. After approval, replace the production site and confirm Cloudflare deployment
   and domain routing. This ZIP itself has not been uploaded to GitHub/Cloudflare.

## Local preview
Unzip the package and double-click `index.html` or, from the folder,
run `python3 -m http.server 8000` and open http://localhost:8000.
Fonts use Google Fonts with local fallback fonts. No font files are included.

## Deployment structure
Use the **contents** of this folder as the root of the GitHub repository;
no build command is needed for Cloudflare Pages.


## Revision v2 (2026-11-08)
- Homepage staircase zoom is now substantially more noticeable (scale 1.01 to 1.18 over 18 seconds, reversing smoothly). Only Home animates; visitors with reduced-motion preferences see a static hero.
- Replaced the old 474×637 therapy-room thumbnail with the user-uploaded 2048×1542 photo, without retouching.
- On desktop, the About Me photo is visually height-matched to its text column using CSS cropping; original file remains intact.
- On desktop, the Therapy page photo is tall but not forced to match the entire much longer text column, to avoid an overly narrow crop that would conceal much of the room. The original landscape photo is preserved in assets and the browser controls the crop.
- Mobile photos use their natural aspect ratios and are not height matched.
- Your original Formspree configuration and existing six-page content are unchanged.


## Version 3 mobile refinements (2026-11-09)
- Replaced the mobile Menu/Close text with an accessible three-line hamburger icon that animates to an X on opening.
- Reduced the mobile hero headline scaling to keep “Psychotherapy” inside the screen, including narrow phones.
- Adjusted mobile subtitle sizing so “(Qualifying)” fits or wraps normally instead of clipping.
- Desktop presentation, images, content, and form integration are unchanged.

## Version 4 mobile typography adjustment (2026-11-09)
- Reduced only the homepage Welcome heading on narrow/mobile screens so it remains a little smaller than the Steven Vincent Psychotherapy hero title. Desktop typography unchanged.
