# Reliable Tech Solutions (RTS) website

Static HTML5/CSS3/Bootstrap 5/vanilla JavaScript website for Reliable Tech Solutions, Kenya. Brand asset: the uploaded official logo is preserved unchanged at `assets/images/logo/rts-logo.jpeg`.

## Run locally
Use any static web server so the reusable navbar/footer components can load with `fetch`:

- XAMPP: copy `rts-website` to `htdocs` and open `http://localhost/rts-website/`.
- Python: run `python -m http.server 8000` from this folder, then open `http://localhost:8000/`.

Opening HTML directly as `file://` may prevent browser component loading because of local-file security rules.

## Pages
`index.html`, `about.html`, `products.html`, `product-details.html`, `services.html`, `projects.html`, `quotation.html`, and `contact.html` are linked from the navbar and footer. `components/navbar.html` and `components/footer.html` are reusable fragments loaded by `assets/js/script.js`.

## Features
- Official RTS logo in navbar, hero, footer, about, contact and quote-related website flow.
- Navy/royal blue/orange/white visual system.
- Product search and category filtering.
- Product detail view using `product-details.html?id=...`.
- Dynamic WhatsApp product/service messages using `254758865075`.
- Quote form with client-side validation and confirmation summary.
- Contact form validation and integration-ready success state.
- Service and project sections with filters, CTAs, placeholder artwork and clear content markers.
- Sticky responsive navbar, dropdowns, floating WhatsApp/call buttons, back-to-top button, accessible labels and responsive Bootstrap grids.
- SEO titles, descriptions, Open Graph metadata, canonical placeholder, sitemap and robots file.

## Images
The uploaded official logo is the only supplied brand image and is used unchanged. Product/service/project imagery is original SVG placeholder artwork created for the demo and clearly labeled as placeholder content. Replace these files with RTS-owned or properly licensed photographs before publication. Keep descriptive alt text for every image.

## Front-end security notes
This version intentionally has no passwords, API secrets or private credentials. Client-side validation improves usability but is not security. Before connecting forms to PHP/MySQL or email, add PDO prepared statements, CSRF protection, server-side validation, output escaping, rate limiting, secure sessions, spam controls and access controls. Never trust product price/specifications from the browser; validate on the server.

## Future PHP/MySQL modules
The stable IDs/classes and data arrays are designed to map to `products`, `categories`, `services`, `customers`, `quotations`, `orders`, `contact_messages`, `projects`, `users` and `admins`. Replace the JS arrays with server-rendered JSON or PHP templates, preserving `id`, `category`, `name`, `description`, `features` and inquiry flows. A future admin panel can implement CRUD for each module with role checks and prepared SQL.

## Content review before publishing
Confirm current product specifications, availability, pricing, business hours, official social-media URLs, testimonials, street address (if desired), project photography, and all claims with RTS. The current social links are intentionally placeholders and testimonials are marked as demo placeholders.
