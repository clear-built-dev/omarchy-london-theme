# Artwork provenance

Author and maintainer: Shas Veeramani (GitHub: clear-built-dev).

- `backgrounds/london.png`: rendered from the original `artwork/london.svg`
  created for this theme. 3840 × 2160 pixels.
- `backgrounds/buckingham-palace.png`: AI-assisted pencil illustration created
  with OpenAI's built-in image-generation tool, refined using the Windsor
  illustration as a style reference. 1672 × 941 pixels.
- `backgrounds/windsor-castle-phone-box.png`: AI-assisted pencil illustration
  created with OpenAI's built-in image-generation tool. 1672 × 941 pixels.
- `preview.png`: composed from the London artwork, palette, and generic text.
  No private desktop capture or third-party photograph is included.

The project is offered under the MIT license to the extent the author holds
rights in its contents. AI-generated portions are identified here rather than
represented as manually drawn artwork. No third-party wallpaper downloads or
font binaries are included.

The illustrations were created on 26 October 2026. Earlier revisions and
unused backgrounds are excluded from this release.

Regenerate the original London PNG after editing the SVG:

```sh
rsvg-convert -w 3840 -h 2160 artwork/london.svg -o backgrounds/london.png
```
