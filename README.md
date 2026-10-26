# London

A dark Omarchy theme inspired by an evening on the Thames: slate blue,
Portland stone, warm brass, and restrained London red.

![London theme preview](preview.png)

## Install

```sh
omarchy theme install https://github.com/clear-built-dev/omarchy-london-theme
```

The package contains exactly three wallpapers:

- **London** — Westminster, Big Ben, the London Eye, and a red double-decker.
- **Buckingham Palace** — a spacious, rough pencil sketch on dark slate paper.
- **Windsor Castle** — a matching sketch with a classic red telephone box.

Cycle backgrounds with `omarchy theme bg next`.

## Optional animation

Install the separate [London Motion plugin](https://github.com/clear-built-dev/omarchy-london-motion)
for a moving bus, rotating London Eye, and gently waving palace and castle flags.
Installing this theme alone displays still wallpapers. The marketplace does
not install bundled plugin code, so the animation is a separate, explicit step.

## Palette and font

| Role | Colour |
| --- | --- |
| Background | `#18232d` |
| Raised surface | `#263541` |
| Text | `#dedbd2` |
| Focus / accent | `#d4b477` |
| Blue | `#8eafc7` |
| Red | `#df7776` |
| Green | `#99b391` |

Recommended: **JetBrainsMono Nerd Font**, Regular weight, already the default
on the tested Omarchy installation. Theme installation does not change fonts.

```sh
omarchy font set "JetBrainsMono Nerd Font"
```

Omarchy generates application colours from `colors.toml`. Tested with Omarchy
4.0.6-1; other releases have not been verified.

## Artwork and license

The London skyline is original SVG artwork; its editable source is
`artwork/london.svg`. Buckingham Palace and Windsor Castle were generated with
OpenAI image generation and refined under the author's direction. They are
illustrations, not documentary photographs. See [ARTWORK.md](ARTWORK.md).

The preview is a composed demonstration of the palette and wallpaper, not a
screenshot of a private desktop. No font files are bundled.

MIT license; see [LICENSE](LICENSE). Independent community theme, unaffiliated
with Omarchy or the institutions depicted.
