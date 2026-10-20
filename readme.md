# CJJacob Design Studio

Studio-led portfolio rebuilt October 2026. Buildless HTML, CSS and vanilla JavaScript. Edit files directly; no dependency installation or build step is required.

## Pages
- index.html: responsive homepage, interactive graphic, project-note dialogs, services, process, FAQs and enquiry form.
- privacy.html and terms.html: original document text retained, styled to match the studio. Review the business-policy wording before publishing; January 2025 dates remain because the legal content was not revised.
- indexv2.html, index3.html and inex4.html: previous standalone design experiments retained.
- assets/css/styles.css and assets/js/script.js: active shared assets.

## Preview
Run `node preview.cjs` from this directory and open http://127.0.0.1:4173. Stop with Ctrl+C.

## Contact
The original Formspree endpoint is retained. JavaScript adds success, failure and timeout feedback; unsuccessful submissions retain entered content. Native form POST remains available without JavaScript. Email and WhatsApp are alternatives. Verify the Formspree account is active and complete one authorized real enquiry before production launch.

## Design and accessibility
Responsive layouts at 650px and 1000px; wider layouts are constrained at 1600px. Semantic headings and content render without JavaScript. Native FAQ disclosure controls, keyboard focus indicators, a skip link, modal dialogs and reduced-motion support are included. Google Fonts are optional with local fallback fonts. No GSAP, Lenis, icon library or runtime framework is required.

## Deployment
Existing Vercel configuration retained in simplified static form. Assets revalidate instead of caching forever under unchanged filenames. Backups are excluded with .vercelignore and blocked by the local preview server. No deployment has been performed.

## Preservation
A timestamped copy of the replaced files and original assets lives in backups/. Keep it local. Do not upload backups to another host. Older alternate HTML drafts have not been rewritten.

## Validation
See QA.md for checks performed and limitations. Performance scores are not claimed without measurements.
