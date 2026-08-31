# Jayde Engineering Solutions Ltd — website

Static site, one file. No build step, no framework, nothing to install.
Smart locks, CCTV and gate automation.

The logo and all product photos are embedded inside `index.html`, so there is
nothing else to upload and nothing that can break by being moved.

## Publishing on GitHub Pages

1. Push `index.html` to the root of a repository.
2. Repository **Settings → Pages**.
3. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save. The site appears at `https://<username>.github.io/<repo>/` in a minute or two.

## Things to change

Open `index.html` and search for `EDIT:`.

- **Phone** — three places, all `254725927169`. Digits only, country code first, no `+` or spaces.
- **Email**
- **Prices** — in the product cards, and again in the `products` list near the top of the script
  (the carousel reads its prices from there, so change both).
- **Areas served** — currently "Nairobi and surrounding counties".
- **Facebook** — no link yet. Add one in the socials block once the page URL is confirmed.
- **`ENDPOINT`** — top of the script. Paste a [Formspree](https://formspree.io) or
  [Web3Forms](https://web3forms.com) URL and every enquiry is emailed as well as opening
  WhatsApp. Leave it empty and the form is WhatsApp-only.

## How the enquiry form works

There is no server. The form collects the answers, writes them into a message and
opens WhatsApp with that message ready to send — the visitor presses send themselves.
Setting `ENDPOINT` adds an emailed copy so nothing is lost if they abandon at that step.

## Still to verify with the client

Prices, the free-installation offer, "100 fingerprints per lock", and the service area
were taken from public listings rather than confirmed directly.

## Browser support

Modern browsers. All motion is disabled automatically for anyone whose system is set
to reduce motion.
