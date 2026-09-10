# Steven Vincent Psychotherapy website

A static, responsive four-page website built for free hosting on GitHub Pages or Cloudflare Pages.

## Pages
- `index.html` — Home
- `about.html` — About Steven
- `therapy.html` — Therapy
- `fees.html` — Fees & FAQ

## Before publishing
1. Open `script.js`.
2. Replace:
   `https://calendly.com/YOUR-LINK`
   with your real Calendly consultation URL.
3. If you have the original Psychology Today badge file and original bird logo, replace the cropped mockup versions in `/assets` using the same filenames.
4. Review the wording on all pages one last time.

## Publish with GitHub + Cloudflare Pages
1. Create a new GitHub repository, for example `steven-vincent-psychotherapy`.
2. Upload every file and the `assets` folder from this package.
3. In Cloudflare, go to **Workers & Pages → Create → Pages → Connect to Git**.
4. Select the GitHub repository.
5. This is a plain static site, so no build command is required.
6. Set the output/root directory to the repository root.
7. Deploy.
8. In the Cloudflare Pages project, add your custom domain.
9. Follow Cloudflare's DNS instructions for your domain registrar.

## Local preview
Double-click `index.html`, or run a tiny local server from this folder:
`python3 -m http.server 8000`

Then visit `http://localhost:8000`.

## Design
The same original forest-staircase photograph is used for the top and bottom of every page with different crop positions, creating the consistent visual system requested.


## Contact form

The contact form is now connected to Formspree using:

`https://formspree.io/f/xyeyllew`

Consultation requests submitted through `contact.html` will be sent through that Formspree form.
