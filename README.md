# BadAss Captcha

Static marketing and API-example site for the BadAss Captcha 2Captcha-compatible service.

**Live:** https://badasscaptcha.com/

## Contents

- `index.html` — complete landing page with supported methods, rates, and copyable API examples.
- `assets/` — shared and site-specific CSS and browser JavaScript.
- `deploy/badasscaptcha.conf` — production Nginx virtual host with HTTPS.

No build step or external runtime is required for the marketing site; deploy these files directly to a static web root. The `/in.php` and `/res.php` API routes require the separate CAPTCHA backend.

## Backend

The CAPTCHA reseller backend is available at: https://github.com/bensblueprints/captcha-reseller-api

It supports both CapSolver and 2Captcha as upstream providers.

## Production

Served by Nginx on Hetzner `144.76.78.158` from `/srv/badass-websites/dist/badasscaptcha.com`. HTTPS uses a Let's Encrypt certificate managed by Certbot.
