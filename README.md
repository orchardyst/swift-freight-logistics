# C & E Logistics

A simple static website for C & E Logistics: Home, Services, About, and Contact pages.

## Structure

- `index.html` – Home
- `services.html` – Services
- `about.html` – About
- `contact.html` – Contact (static form, no backend wired up yet)
- `styles.css` – Shared styling

## Running locally

No build step needed. Open `index.html` directly in a browser, or serve the folder with any static server, e.g.:

```
npx serve .
```

## Deploying

This is a plain static site, so it deploys as-is to either:

- **Netlify**: drag-and-drop the folder, or connect the GitHub repo. Build command: none. Publish directory: `.`
- **Vercel**: import the GitHub repo. Framework preset: "Other". Build command: none. Output directory: `.`

## Contact form note

The form on `contact.html` is static HTML only — it doesn't send anywhere yet. To make it functional:

- On Netlify, add `data-netlify="true"` and a hidden `form-name` input to enable [Netlify Forms](https://docs.netlify.com/forms/setup/).
- On Vercel (or anywhere else), wire it up to a service like Formspree, or a small serverless function.
