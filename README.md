# Digital Product Autopilot

**ProductPilot** is a lightweight, browser-based workspace for turning an early digital-product idea into a structured product brief.

## Live preview

Deploy this repository with [Cloudflare Pages](https://pages.cloudflare.com/) or open `index.html` locally.

## Current MVP features

- Create product briefs for templates, e-books, software, courses, services and other digital products.
- Capture the target audience, customer problem, desired outcome, features, price and notes.
- Generate a structured brief with positioning guidance and suggested launch steps.
- Save drafts in browser `localStorage`.
- Search and filter the product library.
- Open, delete and export briefs as Markdown.
- Responsive dashboard for desktop and mobile.

## Run locally

No build tools or dependencies are required.

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Create a product brief from the Product builder.

For a local development server, you can also run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Architecture

- `index.html` — application structure and views
- `styles.css` — responsive visual system
- `app.js` — product brief generation, local persistence, search, delete and Markdown export

The application is intentionally static and can be hosted on Cloudflare Pages without a build command. Use the repository root as the output directory.

## Important MVP limitations

This version uses deterministic, built-in templates. It does **not** currently connect to an AI model, perform live market research, publish products, create PDF files, synchronize data across devices, or run background automation. Product data stays in the current browser's local storage; clearing browser site data can remove it. Do not store sensitive information in product notes.

## Roadmap

1. Add optional AI-assisted brief generation through a secure server-side API.
2. Add validated market and competitor research with source links.
3. Add PDF and additional export formats.
4. Add account-based cloud storage and multi-device synchronization.
5. Add workflow automation and publishing integrations.

## Project status

MVP · Front-end prototype · Static deployment ready

## License

MIT
