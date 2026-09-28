# thecommitted.world

Static site for Committed. Hand-authored HTML, no build step.

Ported from the Lovable original in September 2026. Palette and type were
read off the live site so the port is visually identical: cream `#FAF6F0`,
warm cream `#F0E9E0`, green `#2B4A40`, dark green `#1D342D`, terracotta
`#C08E7C`, with Cormorant Garamond over DM Sans.

## Pages

| Path | File |
|---|---|
| `/` | `index.html` |
| `/apply/` | `apply/index.html` |
| `/partners/` | `partners/index.html` |
| `/partners/brands/` | `partners/brands/index.html` |
| `/partners/services/` | `partners/services/index.html` |

## The application form

`/apply/` embeds a Notion form (the "Form builder" view on the Apply
database). **Edit the questions in Notion, not here.** Nothing in this repo
needs to change when you do.

## Notes

- Paths are root-relative, so this only renders correctly at a domain root.
  Preview locally with `python3 -m http.server` rather than opening the files
  directly.
- The old site had a client-side password gate on the Partners pages. It did
  not actually protect anything, since the content shipped in the public JS
  bundle, so it was dropped deliberately rather than reimplemented.
