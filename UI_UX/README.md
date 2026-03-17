# PromptCraft — UI/UX Design Prompts

> A curated library of AI prompts for generating production-ready UI components across every major design aesthetic.

![HTML](https://img.shields.io/badge/HTML-Single%20File-c4521a?style=flat-square)
![Prompts](https://img.shields.io/badge/Prompts-36%2B-1a1714?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-4a9e6b?style=flat-square)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-5a8ed4?style=flat-square)

---

## What is this?

**PromptCraft** is a single-file HTML web app that provides ready-to-use AI prompts for frontend UI/UX development. Each prompt is crafted to help developers and designers generate specific UI components — buttons, cards, navbars, forms, modals, and more — in a particular design aesthetic like Glassmorphism, Neumorphism, Brutalism, or Minimalism.

Instead of writing vague prompts like *"make a button"*, PromptCraft gives you precise, technical prompts that produce consistent, high-quality results when used with AI tools like Claude, ChatGPT, Cursor, or GitHub Copilot.

---

## Demo

Open `ui-prompts-site.html` directly in any browser — no server, no build step, no dependencies.

---

## Features

- **36+ curated prompts** covering 9 component categories
- **12 design aesthetics** represented across prompts
- **Live search** — filter by title, style, tags, or prompt content
- **Category filter pills** — browse by component type
- **One-click copy** button on every prompt card
- **Fully static** — single HTML file, zero dependencies, works offline
- **Responsive** — works on mobile and desktop

---

## Component Categories

| Category | Description |
|---|---|
| **Buttons** | CTAs, ghost buttons, ripple effects, 3D beveled styles |
| **Cards** | Content cards, profile cards, stats cards, product cards |
| **Navbars** | Sticky navs, sidebars, pill navbars, editorial navbars |
| **Forms** | Inputs, floating labels, multi-step forms, validation states |
| **Modals** | Confirmation dialogs, command palettes, lightboxes |
| **Hero Sections** | Split-screen heroes, gradient mesh heroes, newspaper layouts |
| **Dashboards** | Analytics layouts, SaaS admin panels, dark dashboards |
| **Badges & Tags** | Status badges, neon tags, semantic color sets |
| **Loaders** | Skeleton screens, dot pulse loaders, shimmer effects |
| **Tooltips** | Pure CSS directional tooltips, 4-direction support |

---

## Design Aesthetics Covered

Each prompt specifies a target aesthetic so AI tools know exactly what visual language to apply:

- **Minimalism** — whitespace-first, sharp edges, restrained palette
- **Glassmorphism** — frosted glass, backdrop blur, semi-transparent layers
- **Neumorphism** — dual shadows, soft extruded surfaces, tactile feel
- **Skeuomorphism** — real-world textures and material mimicry
- **Flat Design** — bold colors, 2D shapes, no gradients
- **Material Design** — Google's elevation system, ripple effects, paper metaphor
- **Brutalism** — thick borders, offset shadows, raw typography
- **Aurora / Gradient Mesh** — animated multi-color gradient backgrounds
- **Dark UI** — deep backgrounds, neon accents, developer-tool aesthetics
- **Claymorphism** — inflated 3D bubbly shapes, pastel palette
- **Retro / Y2K** — CRT vibes, neon on black, pixel fonts
- **Swiss / International** — strict grids, type hierarchies, editorial precision

---

## Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/your-username/promptcraft-ui.git
cd promptcraft-ui
```

### 2. Open the file

```bash
open ui-prompts-site.html
# or just double-click it in your file explorer
```

No npm install. No build process. No config files. It opens instantly.

### 3. Use a prompt

1. Browse or search for a component you need
2. Click **Copy prompt** on any card
3. Paste it into Claude, ChatGPT, Cursor, or any AI tool
4. Get production-ready UI code

---

## How the Prompts are Structured

Every prompt in the library follows a consistent structure to ensure AI tools generate precise, usable output:

```
[Component description] + [Visual/aesthetic specs] + [Interaction behavior] + [Technical implementation hints]
```

**Example — Glassmorphism CTA Button:**
> *Design a CTA button using glassmorphism: backdrop-filter blur(12px), semi-transparent white background (rgba 255,255,255,0.15), 1px border with rgba white at 30% opacity. Add a soft inner glow on hover using box-shadow with a white inset. Works best on gradient or image backgrounds.*

This level of specificity tells the AI exactly what CSS properties to use, what the hover state should do, and what context it's designed for.

---

## Adding Your Own Prompts

The prompts live in a JavaScript array inside `ui-prompts-site.html`. Each prompt object follows this schema:

```javascript
{
  category: "Buttons",         // One of the 10 component categories
  style: "Glassmorphism",      // The design aesthetic
  difficulty: "Medium",        // Easy | Medium | Hard
  title: "Frosted glass CTA",  // Short descriptive title
  tags: ["glass", "blur"],     // Searchable keyword tags
  prompt: `Full prompt text...` // The actual AI prompt
}
```

To add a new prompt, open the HTML file, find the `const PROMPTS = [` array, and append your object following the schema above. The UI re-renders automatically.

---

## Recommended AI Tools to Use With This

These prompts work well with:

- [**Claude**](https://claude.ai) — excellent for detailed CSS, component architecture, and accessibility-aware code
- [**ChatGPT**](https://chatgpt.com) — strong general-purpose UI code generation
- [**Cursor**](https://cursor.sh) — paste prompts directly into your codebase with inline AI editing
- [**GitHub Copilot**](https://github.com/features/copilot) — works well for generating component code within existing projects
- [**v0 by Vercel**](https://v0.dev) — specialized for generating React + Tailwind UI components

---

## Project Structure

```
promptcraft-ui/
│
├── ui-prompts-site.html   # The entire app — HTML, CSS, and JS in one file
└── README.md              # This file
```

The app is intentionally kept as a single file for maximum portability. You can host it on GitHub Pages, Netlify Drop, or just share the HTML file directly.

---

## Hosting on GitHub Pages

1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://your-username.github.io/promptcraft-ui/ui-prompts-site.html`

---

## Contributing

Contributions are welcome! If you have a great prompt that consistently produces high-quality UI output, open a pull request.

**Guidelines for new prompts:**
- The prompt must be specific enough to produce consistent results across different AI tools
- Include CSS property names, values, or techniques where relevant
- Specify interaction states (hover, active, focus) where applicable
- Test your prompt with at least one AI tool before submitting
- Follow the existing schema — `category`, `style`, `difficulty`, `title`, `tags`, `prompt`

---

## Roadmap

- [ ] Expand to 100+ prompts
- [ ] Add React / Tailwind-specific prompt variants
- [ ] Add a difficulty filter (Easy / Medium / Hard)
- [ ] Add a "Run with Claude" button that opens the prompt directly in claude.ai
- [ ] Dark mode for the site itself
- [ ] Export prompt collection as JSON

---

## License

MIT — free to use, modify, and distribute. Attribution appreciated but not required.

---

*Built with care for designers and developers who want to ship beautiful interfaces faster.*
