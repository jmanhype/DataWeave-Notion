# DataWeave-Notion

A modern, responsive landing page built with Astro and TypeScript, featuring a clean UI component library and Tailwind CSS styling.

## 🌟 Features

- **Modern Stack**: Built with Astro 4.0+ and TypeScript
- **UI Components**: Reusable component library including:
  - Navigation bar with search and cart functionality
  - Hero section with call-to-action
  - Card components with headers and content sections
  - Data tables with sorting capabilities
  - Line charts for data visualization
  - Badges and buttons
  - Avatar components
  - SVG icon library (Menu, Search, Shopping Cart, Social Media icons, etc.)
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Type-Safe**: Strict TypeScript configuration for enhanced developer experience
- **Performance Optimized**: Leverages Astro's static site generation for fast page loads

## 🚀 Project Structure

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Card.astro
│   │   ├── Footer.astro
│   │   ├── HeroSection.astro
│   │   ├── NavBar.astro
│   │   └── ui/
│   │       ├── Avatar.astro
│   │       ├── Badge.astro
│   │       ├── Button.astro
│   │       ├── Card.astro
│   │       ├── CardContent.astro
│   │       ├── CardHeader.astro
│   │       ├── CardTitle.astro
│   │       ├── icons.ts
│   │       ├── LineChart.astro
│   │       ├── Table.astro
│   │       ├── TableBody.astro
│   │       ├── TableCell.astro
│   │       ├── TableHead.astro
│   │       ├── TableHeader.astro
│   │       └── TableRow.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 🛠️ Development

This project uses:
- **Astro**: Static site generation framework
- **TypeScript**: Type-safe development with strict mode enabled
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development

### Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. Open your browser and navigate to `http://localhost:4321`

### Building for Production

To create a production build:

```bash
npm run build
```

The optimized static files will be generated in the `./dist/` directory.

## 📦 Component Usage

### Icons

The project includes a TypeScript-based icon library with proper type definitions:

```astro
---
import { MenuIcon, SearchIcon, ShoppingCartIcon } from '../components/ui/icons.ts';
---

<MenuIcon class="w-6 h-6" />
<SearchIcon class="text-gray-500" />
```

### UI Components

Reusable UI components are available in `src/components/ui/`:

```astro
---
import Button from '../components/ui/Button.astro';
import Card, { CardHeader, CardContent, CardTitle } from '../components/ui/Card.astro';
---

<Card>
  <CardHeader>
    <CardTitle>Card Title</CardTitle>
  </CardHeader>
  <CardContent>
    Card content goes here
  </CardContent>
</Card>
```

## 📝 License

This project is open source and available under the MIT License.

## 👀 Want to learn more?

- [Astro Documentation](https://docs.astro.build)
- [Astro Discord Server](https://astro.build/chat)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
