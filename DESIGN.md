# Rose Meridian — design notes

## Identity

A small figure facing something vast and bright that it cannot predict. The three-body problem as a
feeling rather than a diagram: three suns, no stable orbit, civilizations that rise and fall at dawn.

**Should feel:** hazy, dusty, quiet, awed, slightly ominous, cinematic.
**Should not feel:** neon sci-fi, cosmic purple, starfield black, cheerful pastel, chrome.

## Palette source

Ground, text and accent are measured from two stills of the Netflix series *3 Body Problem* (season 1):
the pyramid at sunrise in the VR game (E01 48:55 and 49:03). Every other colour is measured from the
nine wallpapers, which are one warm family from mauve through rose and salmon to apricot and cream.
Nothing was invented to fill a slot, and colours that appear in no wallpaper are not in the theme.

| Colour | Hex | Source |
| --- | --- | --- |
| Silhouette (ground) | `#23221f` | the pyramid and dead tree in shadow |
| Sun (text) | `#fbe4c5` | the sun's core, 12.9:1 |
| Sunrise (accent) | `#ed9998` | the sun's rose rim |
| Mauve-grey sky (dim text) | `#9b9095` | the sky around the sun |
| Horizon sand (inactive border) | `#665f58` | the horizon under the sun |
| Dawn | `#cda0ad` | the pink haze |
| Rose | `#c8787b` | the sunrise rim, deeper |
| Salmon | `#f4a68e` | wallpapers, strongest colour at hue 20-40 |
| Apricot | `#fdca9f` | wallpapers, strongest colour at hue 60-80 |
| Sun gold | `#c6a573` | the cream of the suns in the wallpapers, darker (hue 77) |
| Blush | `#ebc5d1` | the dawn haze, lit |
| Lit sky | `#c1aab4` | the mauve-grey sky, lit |

Hue and chroma are measured; only lightness was placed, so the slots stay apart and readable.
Dark/bright variants and surfaces are lightness steps of the same colours.

## Roles

- **Ground, windows and bar** share one material: the pyramid's shadow. The bar is not a separate object.
- **Text** is the sun itself, at 12.9:1.
- **Accent** is the sun's rose edge. Selection is the dawn haze in shadow (`#583742`).
- **Terminal colours are one warm family**, not a rainbow. Slot names are schema labels: red is deep rose,
  orange salmon, yellow apricot, green the darker gold of the suns, cyan blush, blue the lit sky,
  magenta dawn. Errors (rose) and passes (sun gold) differ in hue and lightness.

## Surfaces as objects

- **Active window border — the sun disc:** rose rim, cream core, rose rim, running corner to corner (45°) so the colour changes at the corners.
- **Inactive border:** horizon sand at 60%.
- **Menu and launcher:** the selected row stands between two pillars, like the pendulum arches: sun-disc bars on the left and right ends only, rose at the ends and cream in the middle (vertical), with a faint sunrise wash.
- **Popups:** framed by the same diagonal sun disc as the windows.

## Wallpapers

Ten flat poster images (Codex image generation, flat vector style, at most a handful of flat colours), upscaled
for flat art and left in their generated colours, which already sit inside the palette: near-black ground,
mauve, plum, sand, rose, peach and the cream sun. A painted set was tried first and replaced so the pack has
one style. People appear only as small silhouettes; no faces. Order follows the story: the problem, the
attempts to predict it, the human computer, the eras, the signal, the screens, the escape.

## Boot unlock

`unlock.png` is the figure-eight: the one stable, repeating solution of the three-body problem, drawn from the
real orbit as a rose line with three equal bodies (cream, salmon, apricot) a third of a loop apart. Plymouth
draws it on the theme background with the sun-cream text colour. `preview-unlock.png` shows the result.

## Guardrails

- Keep the sun as the only bright warm light on screen; do not add a second lead accent.
- No line-plot or diagram overlays on the wallpapers. One wallpaper style per pack.
- Do not lift measured colours for style; only for failing contrast, lightness only.
- Never fill a terminal slot with a hue that is not in the wallpapers (no neon greens, blues or violets).
