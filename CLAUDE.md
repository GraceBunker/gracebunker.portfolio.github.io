# Grace Bunker — portfolio site

Personal portfolio for Grace Bunker, an Applied Mathematics & Mechanics Engineering student at Queen's University (Class of 2028) targeting Canada's space and defence sector.

## Stack
- Plain static site: `index.html` + `styles.css` + `assets/`. No build step, no framework, no JavaScript.
- Fonts from Google Fonts: Archivo (display and body; the hero name uses `font-stretch: 125%`) and JetBrains Mono (labels, data).
- Preview locally with `python3 -m http.server 8000` and open http://localhost:8000.

## Design rules (Deep Field design system)
- Dark and monochrome: page `--void` #050505, panels `--surface-*`, 1px hairlines `--line`, text `--ink` / `--ink-muted` / `--ink-faint`.
- **One accent only: red `--signal` #ff3b30.** Use it sparingly: the logo square, the main CTA, the "live" dots, one highlighted stat, featured cards. No orange, yellow or other colours.
- Labels are mono, uppercase and indexed: `01 / MISSION LOG`.
- Headings are sentence case and end with a period: "Selected projects."
- Stats are a number plus a mono label (`$15M` / `CONTRACT PORTFOLIO COORDINATED`).
- Two corner styles: square for data (stats, experience rows, leadership and news grids), large rounded `--radius-lg` for project cards.
- No drop shadows, gradients, emoji or coloured left borders. Depth comes from surface steps and hairlines.
- Hero background is a static SVG star field with a few twinkling stars. Keep it subtle. Respect `prefers-reduced-motion`.
- Text contrast must stay at 4.5:1 or better. `--ink-faint` is for labels only, never paragraphs.

## Page order
Nav → Hero (name, intro, circular headshot) → Stats → 01 Experience → 02 Leadership → 03 Projects → 04 News → 05 Contact.
Keep the nav links and the section numbers in sync if sections move.

## Content source
All facts come from Grace's résumé (`assets/Grace_Bunker_Resume.pdf`) and her LinkedIn post about Linamar's *See it Be it STEM it*. Don't invent achievements, numbers or dates. Ask Grace if something is missing.

## Good next tasks
- Deploy (GitHub Pages, Netlify or Vercel all work as-is) and add a custom domain.
- Add a favicon (red square on black) and a proper 1200×630 Open Graph image.
- Add real project photos or CAD renders in place of the line drawings in `.card__media`.
- Optional: separate case-study pages for the battery enclosure and the ground-station tower.
