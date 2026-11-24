# Serena Photography

One-page personal website for Serena, a freelance wedding and portrait photographer.
It is plain HTML and CSS with no build step.

## Structure

- `index.html` holds the whole page: hero, portfolio grid, about and contact.
- `photos/` holds the portfolio images.
- `vercel.json` sets headers and clean URLs for Vercel.

## Add photos

Put an image in `photos/`, then replace a placeholder tile in the portfolio grid of `index.html`:

```html
<li><figure><img class="ph" src="photos/your-photo.jpg" alt="Describe the photo" width="800" height="1000"><figcaption>Caption</figcaption></figure></li>
```

Tiles are 4:5, so photos are cropped to fit. Use files at least 1200px wide.

## Update the contact email

Change `hello@serenaphotography.com` in the contact section of `index.html` (it appears in the link and the visible text).

## Run locally

```sh
npx serve .
```

## Deploy on Vercel

1. Import this repository at https://vercel.com/new.
2. Leave the framework preset as **Other**. No build command is needed and the output directory is the repository root.
3. Click Deploy. Every push to `main` redeploys the site.
