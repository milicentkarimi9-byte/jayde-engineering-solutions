# Jayde Engineering Solutions Ltd — website

Static site. One file. No build step, no framework, no folders, nothing to install.
Smart locks, CCTV and gate automation.

`index.html` contains everything — the logo, the product photos and both background
videos are embedded inside it. There are no external assets, so nothing can break by
being uploaded to the wrong place.

## Publishing on GitHub Pages

1. Push `index.html` (and this README) to the repo root.
2. Repository **Settings → Pages**.
3. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save. Live at `https://<username>.github.io/<repo>/` within a minute or two.

## The background videos

Two sections play video behind their text: **Services** (a gate being opened by remote)
and **How a fitting goes** (a fitted lock being used). Both are silent, loop forever, and
start on their own — there is nothing to press. A dark tint sits over each one so the
text stays readable.

They are muted because browsers refuse to autoplay anything with sound. If a browser
blocks autoplay anyway, the first scroll or tap starts them. Anyone whose system is set
to reduce motion sees a still frame instead.

Together the videos are about 310 KB, which is why the page is roughly 0.9 MB.

## Things to change

Open `index.html` and search for `EDIT:`.

- **Phone** — several places, all `254725927169`. Digits only, country code first, no `+` or spaces.
- **Email** — currently a personal Gmail. Swap it the moment a business address exists.
- **Prices** — in the product cards, and again in the `products` list near the top of the
  script (the hero carousel reads from there, so change both or they'll disagree).
- **Areas served** — currently "Nairobi and surrounding counties".
- **Facebook** — currently a `/share/` link. Swap for the page's own URL when it has a handle.
- **`ENDPOINT`** — top of the script. Paste a [Formspree](https://formspree.io) or
  [Web3Forms](https://web3forms.com) URL and every enquiry is emailed as well as opening
  WhatsApp. Leave empty and the form is WhatsApp-only.

## How the enquiry form works

There is no server. The form writes the answers into a message and opens WhatsApp with it
ready to send — the visitor presses send. Setting `ENDPOINT` adds an emailed copy so nothing
is lost if they abandon at that step.

## Still missing

No CCTV footage. Locks and gates both appear on film; CCTV is described in text only.

## Still to verify with the client

Prices, the free-installation offer, "100 fingerprints per lock", and the service area were
taken from public listings rather than confirmed directly.
