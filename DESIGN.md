# Photonics Design System

A restrained technical presentation system: white ground, ink text, one red title rule, and a gray footer band with a red page tab. It suits research talks and engineering reviews. Content sits on a strict two-column frame, and red marks structure rather than decoration.

All sizes are px on a 1920 × 1080 canvas. 1 px = 0.75 pt.

## Colors

| Token | Hex | Role |
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

Use Ink, Slate, or Brick for text. Red on White reaches 4.48:1, so keep it to large text and shapes. Never use Stone for text.

## Typography

Primary font: `FS PF BeauSans Pro`, falling back to `Fira Sans`, Arial, sans-serif.

Numeral font: `FS Magistral` Bold Italic, falling back to `Exo 2`, Arial, sans-serif.

| Role | Size | Line height | Weight | Tracking |
|---|---|---|---|---|
| Cover and section | 64 | 90 | 700 | -1.28 |
| Slide title | 60 | 84 | 700 | -1.2 |
| Stat value | 54 | 76 | 700 | -0.8 |
| Quote | 42.7 | 56 | 400 | 0 |
| Step numeral | 40 | 56 | 700 italic | 0 |
| Block heading | 38 | 53 | 700 | -0.37 |
| Step title | 38 | 53 | 400 | -0.37 |
| Body | 30 | 45 | 400 | 0 |
| Caption and note | 24 | 36 | 400 | 0 |
| Table header | 24 | 36 | 700 | 0.48 |
| Eyebrow | 24 | 34 | 700 caps | 1.92 |

Nothing is smaller than 24px.

## Layout

- Margin: 48.
- Title: x 48, y 25, left aligned.
- Title rule: x 48, y 117, 288 × 12, Red.
- Content starts at y 181.
- Left column: x 48 to 650, for text blocks.
- Right column: x 728 to 1856, for tables, figures, and panels.
- Note: x 48, y 889, 24px Slate.
- Footer band: x 0, y 1032, 1920 × 48, Stone.
- Page tab: x 1656, y 1032, 264 × 48, Hot, slightly rounded, with a 30px Bold White number at the right.

Cover and section slides center their text and omit the title rule. They keep the footer.

## Components

**Text block:** a 38px Bold heading, then 30px body with a 10px gap. Keep 26px between blocks. Use three blocks of at most two lines.

**Numbered step:** an 80 × 80 Red circle with a White numeral. A 38px Regular title sits 24px to its right, with a 24px description below. Use at most three steps.

**Table:** Panel header with 24px Bold text. Use 24px cells with 24px padding and horizontal 2px Mist rules only.

**Callout panel:** Panel fill, an 8px Red top edge, and a Brick eyebrow inset 32px. Inner boxes are White with a 2px Mist edge.

**Comparison:** a shared Panel strip above two 548 × 218 cards with a 32px gap. The reference card has a Mist edge, and the tested option has a Red edge. An 8px Red rule introduces the conclusion.

**Stat card:** 548 × 172 with a 2px Mist edge and no fill. Use a 54px Bold Brick value with a 24px label.

**Image area:** cover photos in plain rectangles. Use a Panel fill as the placeholder.

## Depth and shape

The system is flat. Use no shadows, gradients, or background textures. Corners are square, except the page tab and step circles.

## Citation

Cite as `Author et al. (year)`, for example `Macenski et al. (2020)`. Do not add a table or figure number or a `Source:` label. Style citations in Brick and underline them when linked. Put the full reference in the speaker notes.

## Do

- Give every content slide the same title position and red rule.
- Put text on the left and evidence on the right.
- State a status in words, such as "proposed" or "not published".
- Give each slide one message.

## Don't

- Don't fill a slide with Red or use a dark slide background.
- Don't use Hot anywhere but the page tab.
- Don't add colors, shadows, or a third typeface.
- Don't let content cross the footer at y 1032.
- Don't communicate status by color alone.
