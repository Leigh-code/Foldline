# Foldline

Fold a packaging dieline into 3D in your browser. Add artwork, emboss, foil, Spot UV and plastic windows, then export a 3D model, still images or an animated sequence.

**Status: alpha.** It works, but expect rough edges. Completely and embarrassingly vibecoded. Please report problems.

Everything runs in your browser. Your files are never uploaded anywhere.

## Preparing your dieline

Export your dieline from Illustrator as an **SVG** with these layer names:

| Layer name | What it does |
|---|---|
| `Cuts` | Cut lines |
| `Folds` or `Creases` | Fold lines (each fold must run all the way to a cut line or another fold) |
| `Emboss` or `Deboss` | Raised or pressed areas (optional) |
| `Foil` | Foil areas (optional). Add a colour to the name to set it: `Gold foil`, `Copper foil`, `Holographic foil`, `Glitter foil` |
| `Spot UV` or `Varnish` | Clear gloss varnish areas (optional) |
| Any other layer | Printed artwork |

Tips:

- Convert text to outlines before exporting.
- Embed images rather than linking them.
- The colour of the emboss, foil and Spot UV shapes doesn't matter. Only their shape is used.

You can also add artwork, inside artwork, emboss maps and foil or Spot UV masks separately as PNG, JPG, SVG or PDF files. Export them from the same artboard as the dieline so they line up.

## Using it

- **File (SVG):** open a dieline and add artwork.
- **Set bottom:** click a panel to make it the base of the pack.
- **Substrate:** paper, carton board or corrugated, with real thickness and inside colour.
- **Add emboss** and **Foil / Spot UV:** surface finishes.
- **Plastic window:** click a window to fill it with clear film.
- **Dieline view:** click a fold's angle to change it. Positive angles fold away from the printed side; negative angles fold towards it.
- **Play bar:** fold and unfold the pack. The fit button frames the whole fold.

## Exports

- **Download 3D model:** a GLB file, one object per dieline piece, in metres. Works in Adobe Stager, Blender and most 3D tools.
- **Image (PNG):** a realistic or cel-shaded render at up to 3840 × 2160, with a transparent or coloured background.
- **Animated sequence:** a zip of numbered PNG frames of the pack folding or unfolding, for After Effects, Premiere or Keynote. Keep the tab in front while it renders.

## Credits

Built with these open-source projects:

- [three.js](https://threejs.org), MIT licence
- [Phosphor Icons](https://phosphoricons.com), MIT licence
- [PDF.js](https://mozilla.github.io/pdf.js/), Apache 2.0 licence
- [fflate](https://github.com/101arrowz/fflate), MIT licence
- [Archivo](https://fonts.google.com/specimen/Archivo) and [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono), SIL Open Font Licence

The libraries and fonts load from public CDNs, so the page needs an internet connection.
