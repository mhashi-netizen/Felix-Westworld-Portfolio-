# TEAM FELIX — CONSCIOUSNESS ARCHIVES

Original static portfolio site for Honors 241 (Fall 2026), built as a fictional research-archive interface. This is not an official Delos Corporation website.

## Preview locally

Open `index.html` in your browser. For the most reliable local experience, run `python3 -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Website structure

- `index.html` — home, interactive philosophical lenses, archive navigation, and five member cards
- `micah.html`, `chloe.html`, `connor.html`, `kylie.html`, `sarah.html` — each author's Builds, Journals, Revision Trail
- `builds.html` — searchable/filterable archive of original Build texts
- `journals.html` — personal journal directory and space for team reflections
- `protocol.html` — mission and methodology
- `styles.css` — design system and responsive layouts
- `site.js` — all shared page templates, navigation, interactive features, content rendering
- `content.js` — **the only file you need to update to add writing**

## Adding content

Open `content.js` and populate the arrays. The site never makes up student work.

```js
window.FELIX_CONTENT={
  builds:[{
    title:'Build 1: Example title', author:'micah', kind:'individual',
    date:'2026-09-15', summary:'A short summary approved by the author.',
    html:'<p>Paste the author's full written Build here.</p>'
  },{
    title:'Team Build 2',author:'team',kind:'team', date:'2026-09-30',
    summary:'Team-approved description.',html:'<p>Full team writing.</p>'
  }],
  journals:[{
    title:'Journal 1', author:'micah', date:'2026-10-01',
    html:'<p>The full journal entry.</p>'
  }],
  reflections:[{
    title:'Semester Reflection',date:'2026-12-01',
    html:'<p>Team-approved reflection.</p>'
  }]
};
```

The site automatically adds these to the relevant pages. **Only add author-approved material** and ensure quotations/citations are accurately transferred. This public site should not contain private comments, peer feedback, phone numbers, or sensitive information without permission.

## Publishing on GitHub Pages

1. Create a new public GitHub repository (e.g. `felix-consciousness`).
2. Upload all files in this folder to the repository root and commit.
3. Open Settings → Pages → Build and deployment → Deploy from branch → `main` / `/ (root)` → Save.
4. Your site URL should be `https://YOUR-USERNAME.github.io/felix-consciousness/` when publishing finishes.

Do not overwrite the existing professor-owned repository without permission. If you later need the class's existing URL, coordinate with the instructor. The Google Doc agent might overwrite commits to the old repository.

## Accessibility and technical notes

The site uses no framework, build system, or proprietary assets. Keyboard-accessible navigation, search (⌘/Ctrl + K), interactive tabs, and reduced-motion support are included. Fonts load from Google Fonts, with system fallbacks. All icons/graphics are created in CSS/SVG; no copyrighted imagery or audio has been copied from the reference site.

The design was inspired by the *quality and structure* of Team Logan's portfolio, not its code, media, prose, or maze implementation.
