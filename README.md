# Batangas — Beyond the Ordinary

An editorial travel-magazine concept site for Batangas, Philippines. Built with plain HTML5, CSS3, and vanilla JavaScript — no frameworks, build step, package manager, or backend.

## Run locally

No build or install is required. Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Structure

```
index.html              Page structure, sections, dialogs, inline SVG icons
css/style.css           Design tokens, layout, components, responsive rules, print styles
js/script.js            Navigation, filters, planner, lightbox, dialog/focus management
assets/images/          32 local photographs (Wikimedia Commons)
assets/icons/favicon.svg
```

## Features

- Cinematic hero, reading-progress bar, sticky header, and active-section navigation
- Filterable destination grid with detail dialogs
- 45-combination trip planner (5 landscapes × 3 durations × 3 paces)
- Accessible gallery lightbox (keyboard arrows, Escape, swipe, wrap-around)
- Scroll-triggered reveals and count-up statistics via `IntersectionObserver`
- Mobile navigation with focus trapping and Escape-to-close
- Native `<dialog>` modals, focus restoration, and body scroll locking
- Reduced-motion and print styles; responsive from 320 px upward

## Content notes

- Taal Volcano Island is a **Permanent Danger Zone**; the site presents it as a view from safe vantage points.
- Budget tiers are qualitative categories, not quoted prices.
- Travel times, routes, and schedules change; the site asks visitors to confirm locally.
- Contact details in the footer are clearly labelled placeholders.
- This is an independent editorial concept and is not affiliated with the Provincial Government of Batangas.

## Photography

All photographs are stored locally in `assets/images/`. Sources, authors, and licenses are listed in the in-page **Photo credits** dialog (footer → *Photo credits*) and link back to the original Wikimedia Commons files.

## Browser support

Modern evergreen browsers. Native `<dialog>` is used for the destination, gallery, and credits overlays, with a basic open/close fallback for browsers without `showModal`.
