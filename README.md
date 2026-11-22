# Rex & Pooja reception invitation

Static site, no build step. Deploy this folder as-is.

## Deploy to Cloudflare Pages
- Dashboard: Workers & Pages > Create > Pages > Upload assets, then drop this folder.
- Or Git: framework preset "None", build command empty, output directory `/`.
- Or CLI: `npx wrangler pages deploy . --project-name rex-pooja-invite`

## Editing
- Wedding details live in the `INVITE` object at the top of the `<script>` in `index.html`.
- The text on the card is part of `assets/card.webp` and `assets/card-mobile.webp`.
  If a date, time or venue changes, update the images as well as `INVITE`.
- `_headers` sets long-lived caching for `/assets/*`. Rename an asset when you replace it.
- Fonts (Instrument Serif, Hanken Grotesk) load from Google Fonts.
