# Spud-frog (Spud & Frog) — Online Menu + Ordering

Static website hosted on GitHub Pages with a menu page and an order form that emails submissions via Formspree.

## Live Site
- https://spudnfrog.ca

## Repo Structure
- `index.html` — Landing page (links to Menu + Order)
- `menu.html` — Menu page (edit this whenever your menu changes)
- `form.html` — Order form page (submits to Formspree)
- `images/` — Logo + image assets
- `CNAME` — Custom domain for GitHub Pages (`spudnfrog.ca`)

## How Orders Work
Orders are submitted from `form.html` to Formspree. Formspree emails the order details to the address configured in the Formspree dashboard.

### Formspree Endpoint
In `form.html`, the form `action` should be set to your Formspree endpoint:

```html
<form action="https://formspree.io/f/YOUR_ID" method="POST">
