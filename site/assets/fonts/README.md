# Fonts

The font files are **not stored in this repository**. Aeonik and Aeonik Fono are commercial typefaces from CoType Foundry, and their license does not allow them to be published publicly.

The client supplies these files separately, and they are included in the final handoff package. Place them in this folder with exactly these names:

| File | Typeface | Weight |
|---|---|---|
| `aeonik-regular.woff2` | Aeonik | 400 |
| `aeonik-medium.woff2` | Aeonik | 500 |
| `aeonik-bold.woff2` | Aeonik | 700 |
| `aeonikfono-medium.woff2` | Aeonik Fono | 500 |
| `aeonikfono-semibold.woff2` | Aeonik Fono | 600 |

The site's CSS loads the fonts from this folder by these exact filenames. Renamed or missing files will cause the site to fall back to a system font.
