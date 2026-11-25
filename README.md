# Key Tag Maker – ไทย / English

A browser tool that turns a word (Thai or English) and an optional picture into a 3D-printable key tag (70 × 30 × 4 mm), downloaded as a multi-colour `.3mf` file.

**Use it:** open `index.html` from a web server (for example GitHub Pages). Opening the file directly from disk will not work, because the text engine is loaded as a module.

**Live site:** https://ommi14.github.io/key-tag-maker/

## Features

- Thai and English text, one or two lines, with an on-screen Thai keyboard
- Fonts: Sarabun Bold, DM Serif Display, Tahoma, Browallia New, Cordia New, Dillenia UPC, Iris UPC, Jasmin UPC and Microsoft Sans Serif
- **Picture:** add a PNG or JPG (a logo, icon or drawing). It is traced into a one-colour shape that prints white, like the letters. You can place it left or right of the text, or use it alone, and set its size, the light/dark cut-off and invert.
- Border line on/off, letter thickness, side space
- 1, 4 or 8 tags per file

## Printing

Print face up with no supports.

| Height | Colour |
|---|---|
| 0 – 2.8 mm | White base |
| 2.8 – 3.4 mm | Burgundy panel |
| 3.4 – 4.0 mm | White raised letters, picture and border |

- One-colour printer: change filament at 2.8 mm (burgundy) and at 3.4 mm (white).
- AMS / multi-colour: each tag has 3 parts already named by colour.

## Libraries

Bundled in `lib/`: [Clipper](https://sourceforge.net/projects/jsclipper/) (polygon maths), [earcut](https://github.com/mapbox/earcut) (triangulation), [JSZip](https://stuk.github.io/jszip/), [HarfBuzz](https://harfbuzz.github.io/) / harfbuzzjs (text shaping). `lib/assets.js` holds the tag geometry, the HarfBuzz WebAssembly build and the fonts (Sarabun and DM Serif Display, SIL Open Font License).
