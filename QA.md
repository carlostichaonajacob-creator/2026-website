# Verification — 20 October 2026

## Passed
- JavaScript and local preview server syntax checks.
- All local links, image/style/script references, anchor targets and unique IDs across index.html, privacy.html, terms.html and 404.html.
- Vercel configuration parses successfully.
- Headless Microsoft Edge rendering at widths 320, 375, 390, 650, 768, 1024, 1440 and 1920 pixels. No horizontal overflow at these widths. Every homepage image loaded successfully.
- Mobile navigation opens, closes on selecting a link and updates aria-expanded.
- Interactive canvas remix, project-note modal opening and Escape dismissal, and native FAQ expansion.
- Simulated Formspree error preserves the message. Simulated success displays confirmation and resets the form. No actual submission was sent.
- Homepage heading and native form action remain available without JavaScript. Mobile navigation has a no-JavaScript fallback.
- Reduced-motion mode keeps the heading visible and disables transition effects.
- Supporting pages render at mobile width without overflow.
- No browser JavaScript errors recorded.
- Desktop and mobile full-page captures visually inspected; lazy-loaded images were explicitly loaded before capture.

## Evidence
- qa/results.json
- qa/home-1440.png
- qa/home-390.png
- qa-check.cjs: browser checks, using the installed Playwright and Edge. Runtime import is specific to this computer.
- verify.cjs: portable static-reference checks (`node verify.cjs`).

## Limits
No production deployment, real Formspree submission, live outbound-link availability check, Safari/iOS-device test, screen-reader audit, or Lighthouse measurement was performed. Legal document wording is retained from the original pages and has not received a legal review. Previous alternate HTML drafts remain archived design references and are outside the active-page checks.
