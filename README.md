# Pastel Brand For Quarto

A shared pastel identity for the Quarto extension documentation websites: a box of six soft pastels, colourful and playful but chalky and muted, with the paper tooth, tints, and dark-column tokens that go with it.

## Installation

```bash
quarto add mcanouil/quarto-pastel
```

This will install the extension under the `_extensions` subdirectory.
If you are using version control, you will want to check in this directory.

## Usage

Point the project at the brand, and add the stylesheet to the theme:

```yaml
brand: _extensions/mcanouil/pastel/brand.yml
format:
  atelier-html:
    theme:
      light:
        - brand
        - _extensions/mcanouil/pastel/pastel.scss
      dark:
        - brand
        - _extensions/mcanouil/pastel/pastel.scss
```

`brand.yml` alone gives the palette.
`pastel.scss` adds the paper tooth, the callout and table tints, and the dark-pinned column tokens that [atelier](https://github.com/mcanouil/quarto-atelier) exposes but does not derive from a brand.

## The idea

Six sticks rather than two or three, so the family reads as cheerful, but each one is greyed back to roughly 20 to 33 percent saturation, so it reads as chalk rather than as candy.
That is what a real box of soft pastels looks like: a wide, happy range of quiet colours.

A pastel behaves differently depending on what it is drawn on, and the palette uses both behaviours.
On light paper the pastel is a tint, and a deeper mix of the same hue carries text and links.
On the dark column and in dark mode the pastel is the ink.
That makes the dark scheme the more colourful one.

| Stick | Pastel | Deep | Chalk | Link light | Link dark |
| --- | --- | --- | --- | --- | --- |
| mint | `#A9DCC9` | `#1C7059` | `#9FD9C4` | 5.31 | 10.75 |
| sky | `#A6C9E2` | `#1D6790` | `#9CC6E2` | 5.49 | 9.44 |
| lemon | `#EFDDA0` | `#77620F` | `#E7D598` | 5.27 | 11.71 |
| coral | `#EDAFA8` | `#A04238` | `#EBA9A1` | 5.60 | 8.74 |
| peach | `#EFC6A3` | `#8E5720` | `#EAC09B` | 5.27 | 10.20 |
| sage | `#C3D3A8` | `#566B2E` | `#BCCEA0` | 5.27 | 10.16 |

Body text reaches 12.75 on light paper and 14.16 on night, both AAA.
Mint carries `primary`, so a link never competes with the coral and peach status colours in the output these sites demonstrate.

> [!IMPORTANT]
> The pastels measure 1.20 to 1.65 against the light paper, below even the 3:1 threshold for interface elements.
> They are decoration only in the light scheme: fills and tints, never text, and never a border that has to be seen for the page to work.

This extension styles HTML output.
It has no effect on PDF, Typst, or Word.

## Example

Here is the source code for a minimal example: [example.qmd](example.qmd).

Rendered output:

- [HTML](https://m.canouil.dev/quarto-pastel/).
