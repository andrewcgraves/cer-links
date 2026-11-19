# Save Metrolink

A one-page link hub for speaking out against OCTA funding cuts to Metrolink. It collects the action letter, toolkits, canvassing script, email template and related articles in one place.

The site is plain HTML and CSS, built on [LittleLink](https://github.com/sethcottle/littlelink). There is no build step and no dependencies.

## Editing links

All links live in [`index.html`](index.html). To add one, copy an existing link in the right section, then change its `href` and label. To remove one, delete its element.

Styles are in [`css/`](css/), and fonts are self-hosted in [`fonts/`](fonts/).

## Running locally

Serve the repo root with any static file server, for example:

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080.

## Deploying

The site is deployed on [Vercel](https://vercel.com/). Every pull request gets a preview deployment, and merging to `main` deploys to production. Vercel Web Analytics is loaded from `/_vercel/insights/script.js`, so it only runs on Vercel.

The upstream LittleLink Docker setup is still in [`docker/`](docker/README.md) if you want to self-host instead.

## Credits

Built on [LittleLink](https://littlelink.io) by Seth Cottle, used under the [MIT License](LICENSE.md).
