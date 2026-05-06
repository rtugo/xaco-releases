# XACO screenshots

Public-facing screenshots served by GitHub Pages and referenced from
`../index.html` (and any future blog / release notes content in this
repo). Reachable at:

```
https://rtugo.github.io/xaco-releases/screenshots/<file>
```

## Conventions

- **Format:** PNG (preferred) or JPG. No HEIC, no TIFF — browsers don't
  render those reliably.
- **Size cap:** keep each file under ~400 KB. Convert PNG → WebP if you
  have many shots or hit the limit. macOS Preview can export both.
- **Naming:** `<view>-<state>-<theme>.png`
  - `view` — `gallery`, `preview`, `map`, `inspector`, `export-panel`, etc.
  - `state` — what's notable about this shot (e.g., `crop-session`,
    `vault-filter-active`, `empty`).
  - `theme` — `light` or `dark`. Skip if not theme-relevant.

  Examples:
  - `gallery-default-light.png`
  - `gallery-default-dark.png`
  - `preview-crop-session-light.png`
  - `map-overlay-dark.png`
  - `inspector-tone-edits-light.png`

- **Originals** (full-resolution, lossless) live in the private source
  repo at `docs/handoff/screenshots/`. This `xaco-releases/screenshots/`
  folder holds only the **web-optimized** copies that are actually
  served to visitors.

## Adding a new screenshot

1. Capture (⌘⇧4 on macOS, save into the private repo's
   `docs/handoff/screenshots/`).
2. Optimize: shrink to display width × 2 (Retina) and re-export at
   ~80% quality.
3. Drop the optimized copy here under the naming convention above.
4. Reference from `../index.html` as
   `<img src="screenshots/<file>" alt="...">`.
5. Commit + push — GitHub Pages picks it up within ~1 minute.
