# NEXT New Baby Expert Assistant — React POC

Mobile-first, interactive guided shopping POC for newborn essentials, designed as a conceptual companion to the NEXT Schoolwear AI assistant.

## Publish to GitHub Pages (important: avoid the blank screen)

1. Create a GitHub repository, e.g. `next-new-baby-assistant`, with default branch **main**.
2. Extract this ZIP. Upload **the contents** (not the containing folder) to the repository root. Preserve the **hidden `.github/workflows/deploy.yml`** directory.
3. Go to **Settings → Pages → Build and deployment → Source → GitHub Actions**. Do not select Deploy from a branch.
4. Open **Actions**, and wait for **Build and deploy New Baby Assistant** to turn green. It runs `npm install`, `npm run build`, and publishes `dist/`.
5. Visit `https://YOUR-USERNAME.github.io/next-new-baby-assistant/`. The Vite `base:'./'` setting handles repository subpaths.

If blank: check GitHub Actions logs, then browser developer console. `index.html` in the repository points at React source by design; only the *built dist folder* is served by Actions.

## Local setup

```bash
npm install
npm run dev
npm run build
npm run preview
```

## What is included

- Six-step journey: arrival timing, first-time parents, existing items, nursery space, budget, priority categories
- Editable answers and multi-select choices
- Dynamic checklists, completion ticks, filters and NEXT category recommendations
- Illustrated cards, illustrative shortlisting, and persistent in-session shopping list
- Safety notes with NHS and Lullaby Trust links
- Responsive desktop/mobile layout with NEXT-inspired styling

## Catalogue and accuracy

The category URLs, example clothing names and attributes are grounded in publicly accessible NEXT UK pages reviewed on 20 October 2026. Most nursery entries are **category-level suggestions** rather than verified individual SKUs. The only prices displayed in the demo are example starting prices for clothing and **are not a live feed**. Cart calculations are illustrative, not a checkout. Illustrations are emoji art and not actual product photography. Do not use product-level claims, compatibility, stock or pricing from this POC in production. Integration requires a live product feed and validated product attributes.

### Product data requirements for production

Category and subtype, SKU, name, brand, current price, availability, sizes, pack quantity, age suitability, material, fastening, colour, photo, dimensions, mattress compatibility, applicable standards, R129 approval where relevant, vehicle compatibility, assembly/installation documents, returns, delivery estimate, category mapping and direct PDP URL.

### Guidance

- NHS newborn essentials: https://www.nhs.uk/baby/caring-for-a-newborn/what-you-will-need-for-your-baby/
- NHS safer sleep: https://www.nhs.uk/best-start-in-life/baby/baby-basics/newborn-and-baby-sleeping-advice-for-parents/safe-sleep-advice-for-babies/
- Lullaby Trust: https://www.lullabytrust.org.uk/baby-safety/safer-sleep-information/keeping-a-clear-cot/
- NEXT nursery catalogue: https://www.next.co.uk/shop/home/nursery/nursery-and-baby
- NEXT bodysuits: https://www.next.co.uk/shop/baby/clothing/bodysuits
- NEXT sleepsuits: https://www.next.co.uk/shop/baby/nightwear/sleepwear/sleepsuits
- Baymard filtering: https://baymard.com/research-articles/current-state-product-list-and-filtering

**The safety information is generic and not a safety certification of individual products.**
