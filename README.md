# -followgut

personal website — one HTML file, zero frameworks, published with GitHub Pages.

## what's inside

- **project showcase** — every project gets a browser-style card with a *real production screenshot* and its own *website icon* in the address bar, stacked in a scroll deck (cards pile up + dim as you scroll, screenshots drift with a small parallax)
- live github stats, repository index (with per-repo icons) + activity feed
- youtube (@CubeCometYT) live subscriber counter + latest videos
- paintable contribution field — click / drag to paint your own streak
- command palette — press `⌘K` (or `/`) to jump anywhere or open any project
- paper / ink themes, reduced-motion friendly

## structure

```
index.html        # the whole site
assets/
├── shots/        # live screenshot per project card
└── icons/        # website icon (favicon) per project + apple-touch-icon
```

## editing the showcase

cards are rendered from the `PROJECTS` array near the top of the `<script>` in
`index.html` — add an object with `name / repo / lang / url / icon / shot / desc`
and it joins the deck automatically (the command palette picks it up too).
