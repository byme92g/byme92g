# CLAUDE.md — AI Assistant Guide for byme92g/byme92g

## Repository Overview

This is a **GitHub profile repository** for Jeremy ([@byme92g](https://github.com/byme92g)), a software developer from Peru. GitHub treats the `byme92g/byme92g` repository specially: its `README.md` is displayed directly on the user's GitHub profile page.

## Repository Structure

```
byme92g/
└── README.md   # GitHub profile page (rendered on github.com/byme92g)
```

There are no source files, build systems, tests, or dependencies — this is a purely static documentation repository.

## File Purposes

### `README.md`
The sole file in this repository. It renders as the GitHub profile landing page and contains:
- Personal introduction and interests
- Skill set organized in a two-column HTML table (Frontend / Backend)
- Technology badges using external SVG/PNG image URLs
- Contact links (GitHub, LinkedIn, Gmail) via shield.io badge images

## Content Conventions

### Layout
- Uses raw HTML (`<table>`, `<tr>`, `<td>`, `<div align="center">`) inside Markdown for multi-column layout
- Skill icons are `<img>` tags with `height="50"` and `title` attributes for tooltips
- Images are sourced from CDNs: `cdn.worldvectorlogo.com`, `www.vectorlogo.zone`, `profilinator.rishav.dev`, `raw.githubusercontent.com`

### Adding New Skills
When adding a technology icon, follow the existing pattern:
```html
<img src="<CDN_URL>" alt="<Technology Name>" height="50" title="<Technology Name>" />
```
- Keep `height="50"` consistent across all icons
- Include both `alt` (accessibility) and `title` (tooltip on hover)
- Place under the appropriate section heading (`### Frontend`, `### Backend`, etc.)

### Sections
| Section | Location | Contains |
|---|---|---|
| Frontend | Left column (`width="50%"`) | HTML, CSS, JS, TS + frontend frameworks |
| Libraries & Frameworks (Frontend) | Left column | jQuery, Sass, Vue, Bootstrap, Tailwind, Svelte, Vuetify |
| Design Tools | Left column | Figma, Adobe XD, InVision |
| Web Build Tools | Left column | Webpack, Vite |
| Backend | Right column (`width="50%"`) | TypeScript, PHP, Java, Kotlin, C# |
| Libraries & Frameworks (Backend) | Right column | Node.js, Laravel, .NET Core |
| Content Manager | Right column | WordPress, Umbraco CMS |
| Other Tools | Right column | ChartJS, Git, GitLab, AWS, Docker, MySQL, MS SQL Server, Linux, Postman |

## Development Workflow

### Branching
- Default branch: `master` / `main`
- Feature branches follow the pattern: `claude/<description>-<id>` (used by AI assistants)

### Making Changes
Since there is no build step, changes are immediate:
1. Edit `README.md`
2. Commit with a descriptive message
3. Push — changes appear live on the GitHub profile

### Commit Style
Historical commits use the message `"Update README.md"`. Prefer more descriptive messages when making substantive changes, e.g.:
- `"Add React to Frontend skills"`
- `"Update contact section with new LinkedIn URL"`

## Key Constraints

- **No build system** — do not introduce one unless the project scope changes significantly
- **No tests** — not applicable for a static profile README
- **Image heights** — keep all skill icons at `height="50"` for visual consistency
- **Column balance** — try to keep the two `<td>` columns roughly balanced in height
- **External images** — all skill icons rely on external CDN URLs; verify URLs are accessible before adding new ones

## Owner Information

- **Name:** Jeremy Pando
- **Location:** Peru
- **Email:** byme92g@gmail.com
- **LinkedIn:** https://www.linkedin.com/in/jeremy-pando/
- **GitHub:** https://github.com/byme92g
