# DataWeave-Notion

Static landing page built with Astro 4 and Tailwind CSS. Contains a component library of common UI elements (tables, charts, cards, badges, avatars, buttons) styled for a data-dashboard aesthetic.

Despite the repository name, this project does not integrate with the Notion API. It is a frontend template.

## What It Contains

A single-page Astro site with 14 reusable `.astro` components:

| Component | File | Description |
|-----------|------|-------------|
| Card | `src/components/ui/Card.astro` | Container with header, content, title slots |
| Table | `src/components/ui/Table.astro` | Data table with head, body, row, cell |
| LineChart | `src/components/ui/LineChart.astro` | Static chart component |
| Badge | `src/components/ui/Badge.astro` | Status/label indicator |
| Button | `src/components/ui/Button.astro` | Action button |
| Avatar | `src/components/ui/Avatar.astro` | User avatar |
| HeroSection | `src/components/HeroSection.astro` | Page hero block |
| NavBar | `src/components/NavBar.astro` | Navigation bar |
| Footer | `src/components/Footer.astro` | Page footer |

Icons are defined in `src/components/ui/icons.ts` (Menu, Search, ShoppingCart, Facebook, Twitter, Linkedin, Play, Flag, SwissFranc).

## Tech Stack

| Tool | Version |
|------|---------|
| Astro | 4.0.6 |
| TypeScript | 5.3 |
| Tailwind CSS | 3.3.6 |
| @astrojs/check | 0.3.3 |

## Setup

```bash
npm install
npm run dev       # Dev server at localhost:4321
npm run build     # Production build to ./dist/
npm run preview   # Preview production build
```

## Project Structure

```
src/
  components/
    ui/           # 9 reusable UI components + icons
    Card.astro    # Page-level card (separate from ui/Card)
    HeroSection.astro
    NavBar.astro
    Footer.astro
  layouts/
    Layout.astro  # Root HTML layout
  pages/
    index.astro   # Single page, composes all components
public/
  favicon.svg
```

## Limitations

- Single page only -- no routing
- No Notion API integration despite the repo name
- Chart component renders static markup, not interactive charts
- No data fetching or backend connectivity
- Components are not published as a standalone package

## License

Not specified.
