# Artwork provenance

Author and maintainer: Shas Veeramani (GitHub: clear-built-dev).

The current edition contains three original native SVG illustrations:

- `artwork/london.svg`: Westminster, Big Ben, the London Eye and a red bus.
- `artwork/buckingham-palace.svg`: Buckingham Palace and the Victoria Memorial.
- `artwork/windsor-castle-phone-box.svg`: Windsor Castle and a red telephone box.

Each PNG in `backgrounds/` is rendered directly from the matching SVG at
**6144 × 3456 pixels**. The vector sources scale without enlarging a raster
image. No third-party photographs, downloaded wallpapers or font binaries are
included. The composed preview uses project artwork and generic text.

Original code and artwork are offered under the MIT license in LICENSE.
The illustrations are stylized scenes, not documentary views.

The first edition used AI-assisted pencil illustrations for Buckingham Palace
and Windsor Castle. Those have been replaced in this edition; their provenance
remains documented in Git history and they are preserved in the local development
archive, outside the active background rotation.

Regenerate any background after editing its source, for example:

```sh
rsvg-convert -w 6144 -h 3456 artwork/buckingham-palace.svg -o backgrounds/buckingham-palace.png
```
