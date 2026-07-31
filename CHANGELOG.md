# Changelog

## Unreleased

## 0.1.0 (2026-07-31)

### New Features

- feat: Initial release.
- feat: Add `brand.yml`, a box of six soft pastels (mint, sky, lemon, coral, peach, sage) on soft off-white paper. Colourful and playful in range, chalky and muted in saturation. Each stick has a deep hue for light-scheme text and a chalk variant for the dark scheme; body text reaches AAA in both schemes and every link reaches AA.
- feat: Add `pastel.scss`, which applies the palette across the page rather than only through `primary`. Headings take mint, sky, and peach; inline code takes coral on a blush tint; the table of contents becomes a tinted panel with a real active state; table headers take a lemon tint; and callouts, tabsets, striped tables, and blockquotes are tinted. Horizontal rules sweep all six sticks. Code blocks are deliberately left to `code-window` and `atelier`.
- feat: Re-point the `--atelier-navbar-*` and `--atelier-sidebar-*` tokens at the palette, with mint as the accent.
- fix: Restore `strong` to full-strength foreground at weight 700; the theme leaves it at 0.6 alpha, making emphasis fainter than the text it emphasises.
- fix: Give links a hover state, which Quarto ships without.
- feat: Add a paper-tooth texture, inlined as a fractal-noise data URI and applied as a fixed overlay at 7 percent opacity. It is hidden under `prefers-reduced-transparency: reduce`.
- fix: Colour the table of contents panel from the dark-pinned column rather than from the page. Tinting it from the light paper left the column's pinned light-on-dark text at 1.02 contrast against it, and the panel heading and Quarto's own "Edit this page" and "Report an issue" links at 1.9 and 1.22.

### Documentation

- docs: Every colour pair is verified against WCAG from the compiled stylesheet, in both schemes, rather than from the palette table alone.
