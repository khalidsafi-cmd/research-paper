# ANO Cleaning Company

A dependency-free, server-rendered bilingual PHP website for anocleaning.company. Persian is the default, with RTL layout; English lives at `/en/` and Persian at `/fa/`.

## Run

Requires PHP 8.0 or newer. From the repository root:

```sh
php -S 127.0.0.1:8080 router.php
```

## Brand assets

The chat images were not available as filesystem attachments during implementation. Copy the supplied horizontal logo to `assets/logo.png` and cleaning photograph to `assets/cleaning.jpg`. The template automatically uses these files when present. Until then, it displays a typographic brand and a decorative CSS interior illustration. No stock imagery or invented customer reviews are used.

## Deploy

Upload this repository to a PHP-enabled Apache document root with mod_rewrite enabled and AllowOverride configured for `.htaccess`. Enable HTTPS for anocleaning.company. On Nginx, route `/`, `/fa/`, and `/en/` to index.php, serve assets normally, and deny direct access to config.php and router.php. Unknown paths must return 404. The development PHP server is not for production.

Public company details and the canonical domain are in config.php. Contact links open telephone, email, or WhatsApp; there is no form backend or database. Confirm offered services with the business before launch. No analytics, cookies, external font requests or JavaScript are required.

## Search launch checklist

- Verify both language pages, HTTPS, phone and WhatsApp on the production host.
- Redirect HTTP and www to https://anocleaning.company at the host level.
- Verify domain ownership in Google Search Console and submit https://anocleaning.company/sitemap.xml.
- Request indexing of /fa/ and /en/. Indexing and rankings are decided by Google and cannot be guaranteed.
- Keep the business name, address and phone consistent across relevant local directories; use a Google Business Profile only if available and eligible in your region.
- Add the original brand assets above before launch. The map link searches the supplied address; verify the exact business pin separately.

Includes localized titles/descriptions, canonical URLs, hreflang, LocalBusiness structured data, robots.txt, XML sitemap, accessible native FAQ disclosures, reduced-motion support, mobile layouts, and keyboard focus styles.

Palette: navy #06275E; royal blue #075AAB; cyan #00B8F4; sky blue #0098DD; white #FFFFFF.
