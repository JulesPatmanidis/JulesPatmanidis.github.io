# CLAUDE.md

Static personal site: `index.html`, `style.css`, `images/`, `favicon.ico`. No framework, no build step, no package.json. GitHub Pages serves the repo root from `main` at https://julespatmanidis.github.io/ (repo `JulesPatmanidis.github.io`).

- Keep it that way. Do not add a bundler, framework or JS unless asked. The only JS is the theme toggle (inline in `index.html`).
- Projects are `<article class="project">` blocks in `index.html` (screenshot, date, title, summary, stack line, links). Screenshots go in `images/`, resized to at most 1400px wide.
- Colours are CSS variables in `style.css`. Dark is the default, and the light values are defined twice (OS preference media query and `[data-theme="light"]`), so change both when editing.
- Use relative asset paths (`images/x.jpg`), and keep them relative even though the site is served from the domain root.
- Content comes from the owner's CV at `../cv/master.md`. Only use numbers and claims that appear there.
- The earlier React/Vite version lives on the `vite-experiment` branch.
