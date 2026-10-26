# Artwork provenance

Architectural pen-and-pencil edition (2.0.0).
Author and maintainer: Shas Veeramani (GitHub: clear-built-dev).

The active wallpapers are exactly 6144 × 3456 pixels:

- `london.png`: rendered directly from original `artwork/london.svg`.
- `buckingham-palace.png`: exported from `artwork/buckingham-palace-pen-pencil-original.png`.
- `windsor-castle-phone-box.png`: exported from `artwork/windsor-castle-pen-pencil-original.png`.

The architectural drawings were created using OpenAI image generation, based on
the previously approved pencil compositions. Buildings, trees and clouds use pen
outlines and pencil hatching on light stone paper. Original sources are 1672 × 941;
6K exports use Lanczos resampling, a minimal centre crop and restrained sharpening.
These are 6K exports, not native 6K source detail. Superseded artwork is kept
in local recovery archives outside this release package.

The companion London Motion renderer maps the drawings into an atmospheric
slate-blue palette while retaining their linework. These source PNGs show the
original light-paper artwork when used without the renderer.

No third-party photograph downloads or font binaries are included. AI-assisted
portions are identified here. Offered under the MIT license to the extent the
author holds rights in the contents.

Rebuild London with `rsvg-convert -w 6144 -h 3456 artwork/london.svg -o backgrounds/london.png`.
Rebuild a sketch export:

```sh
magick artwork/buckingham-palace-pen-pencil-original.png -filter Lanczos -resize '6144x3456^' -gravity center -extent 6144x3456 -unsharp 0x0.65+0.45+0.02 backgrounds/buckingham-palace.png
```
