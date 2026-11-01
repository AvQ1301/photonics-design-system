# Photonics Design System

A slide design system with a white ground, a red title rule, and a gray footer band. Its values were measured from the shapes, text runs, and theme of a 24-slide source deck.

## Contents

| Path | Purpose |
|---|---|
| `DESIGN.md` | The whole system in one file, for design tools and AI agents |
| `tokens/tokens.json` | Colors, type, layout, and component values |
| `tokens/tokens.css` | The same values as CSS custom properties |
| `guidelines/layout.md` | Slide frame, columns, and footer |
| `guidelines/components.md` | Reusable slide patterns |
| `guidelines/citation.md` | Citation format |
| `templates/photonics-template.pptx` | Seven editable PowerPoint slides |
| `examples/index.html` | Browser preview of the tokens and components |

## Quick start

For PowerPoint, install the fonts below, open `templates/photonics-template.pptx`, and duplicate the slide that fits your content. Page numbers update automatically.

For the web, link the tokens and use the variables:

```html
<link rel="stylesheet" href="tokens/tokens.css">
<h1 style="font: 700 var(--pds-size-title)/var(--pds-line-title) var(--pds-font-sans); color: var(--pds-ink)">Slide Title</h1>
```

To preview the system, open `examples/index.html` in a browser.

## Canvas and units

All sizes are px on a 1920 × 1080 canvas. The PowerPoint slide is 20 × 11.25 in, so 1 px = 0.75 pt = 9525 EMU.

## Fonts

| Role | Font | Fallback |
|---|---|---|
| All text | FS PF BeauSans Pro | Fira Sans, Arial |
| Step numerals | FS Magistral Bold Italic | Exo 2, Arial |

FS PF BeauSans Pro and FS Magistral are not included here. Obtain them under your own license and install them locally. `.gitignore` excludes font files so they are not committed by accident.

Fira Sans and Exo 2 are close stand-ins with different letter widths, so check text fit if you use them.

## Colors

| Token | Hex | Use |
|---|---|---|
| White | `#FFFFFF` | Slide ground, boxes on panels |
| Ink | `#171B1F` | Titles and body text |
| Slate | `#515A61` | Notes, quotes, secondary text |
| Stone | `#B5B4B4` | Footer band |
| Mist | `#D7D9DA` | Hairlines and table rules |
| Panel | `#F3F4F4` | Panels and table headers |
| Red | `#DF3621` | Title rule, step circles, panel edges |
| Brick | `#AC2818` | Links, citations, eyebrows, task labels |
| Hot | `#EE0033` | Page tab only |

Contrast ratios, by the WCAG formula:

| Pair | Ratio | Guidance |
|---|---|---|
| Ink on White | 17.31:1 | Any text |
| Slate on White | 7.04:1 | Any text |
| Slate on Panel | 6.38:1 | Any text |
| Brick on White | 6.84:1 | Any text |
| Brick on Panel | 6.21:1 | Any text |
| Red on White | 4.48:1 | Large text and shapes only |
| White on Hot | 4.48:1 | Bold 30px page number only |
| White on Red | 4.48:1 | Bold 40px step numeral only |
| Stone on White | 2.07:1 | Not for text |

## Rules

1. Each content slide opens with the same title and red rule.
2. The footer band and page tab appear on every slide.
3. Text goes on the left. Tables, figures, and panels go on the right.
4. Red is for structure, never a slide fill.
5. State a status in words, such as "proposed" or "not published".

## License

No license has been chosen yet. Add a `LICENSE` file before publishing. It covers only this repository, not the fonts.
