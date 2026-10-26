# Artwork provenance

Architectural pen-and-pencil edition (2.0.1).
Author and maintainer: Shas Veeramani (GitHub: clear-built-dev).

The active wallpapers are exactly 6144 × 3456 pixels:

- `london.png`: rendered directly from original `artwork/london.svg`.
- `buckingham-palace.png`: a slate-blue static render of the Buckingham Palace drawing.
- `windsor-castle-phone-box.png`: a slate-blue static render of the Windsor Castle drawing.

The architectural drawings were created using OpenAI image generation, based on
the previously approved pencil compositions. Buildings, trees and clouds use pen
outlines and pencil hatching on light stone paper. Original sources are 1672 × 941;
6K exports use Lanczos resampling, a minimal centre crop and restrained sharpening.
These are 6K exports, not native 6K source detail. Superseded artwork is kept
in local recovery archives outside this release package.

The saved background PNGs are rendered in the slate-blue evening treatment,
so the carousel, static fallback and animated desktop share the same palette.
The two original source drawings remain in `artwork/` for reproducibility.
London Motion bundles sharpened 6K uncoloured render bases separately, enabling
time-of-day and weather changes without applying the colour mapping twice.

No third-party photograph downloads or font binaries are included. AI-assisted
portions are identified here. Offered under the MIT license to the extent the
author holds rights in the contents.

Rebuild London with `rsvg-convert -w 6144 -h 3456 artwork/london.svg -o backgrounds/london.png`.
Rebuild the plugin's uncoloured Buckingham render base, then export the static
wallpaper with London Motion in evening mode and flag rippling disabled:

```sh
magick artwork/buckingham-palace-pen-pencil-original.png -filter Lanczos -resize '6144x3456^' -gravity center -extent 6144x3456 -unsharp 0x0.65+0.45+0.02 ../omarchy-london-motion/assets/buckingham-palace-base.png
```
