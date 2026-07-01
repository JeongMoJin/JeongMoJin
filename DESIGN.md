# GitHub Profile README Design Tokens

## Atmosphere / Signature

`LearnAndRecord` should feel like an editorial dark creative-tech portfolio: calm, precise, cinematic, and grounded in real projects. The signature is a deep navy field with one amber signal color, supported by Korean/English copy and a data-to-experience rhythm.

## Color

| Token | Value | Role |
| --- | --- | --- |
| `--bg-deep` | `#0B1026` | Header/footer deep navy field |
| `--ink` | `#F8FAFC` | Light foreground on dark image widgets |
| `--primary` | `#315F72` | Main blue-green signal for badges, text animation, graph labels |
| `--accent` | `#F2B705` | Amber highlight for hero gradient, activity graph, streak ring |
| `--activity-point` | `#6FC3DF` | Cool cyan point color for graph detail |
| `--on-accent` | `#111111` | Dark text/icon color on amber badge surfaces |
| `--youtube` | `#FF0033` | YouTube brand badge |
| `--tistory` | `#FF5A4A` | Tistory badge |
| `--github` | `#181717` | GitHub badge |
| `--arcgis` | `#2C7AC3` | ArcGIS badge |
| `--autocad` | `#E51050` | AutoCAD badge |
| `--sketchup` | `#005F9E` | SketchUp badge |

Contrast note: body copy uses GitHub's native README colors. Tokenized colors are used inside externally rendered SVGs and badges.

## Typography

- Native README body: GitHub system Markdown typography.
- Hero image text: capsule-render default rendering with display size `56`, description size `18`.
- Typing SVG: `Inter`, weight `600`, size `22`, used only inside the generated SVG where the API requires a named font parameter.
- Code rhythm blocks: GitHub monospace rendering.

## Spacing

- README section rhythm: headings separated by Markdown blank lines and horizontal rule after the hero.
- Hero image height: `260`.
- Footer wave height: `150`.
- Stats cards: height `170`.
- Table columns: `50% / 50%`.
- Skill icon per-line rhythm: `9`, `8`, `8`, `8` by group.

## Components

- Hero: centered capsule-render image using `--bg-deep`, `--primary`, `--accent`, and `--ink`.
- Motion identity: centered readme-typing-svg using `--primary`.
- Link badges: Shields.io `for-the-badge` style for top-level identity links.
- Project wall: GitHub Markdown table with concise value copy.
- Stack groups: skill-icons grouped by purpose, with small Shields.io badges for tools not covered by skill-icons.
- Signal metrics: dynamic SVG cards with transparent backgrounds, hidden borders, and tokenized accent colors.
- Footer: capsule-render wave using the same palette as the hero.

## Motion

- Claimed motion is implemented through generated SVG services only:
  - capsule-render `animation=fadeIn`
  - readme-typing-svg line rotation
- No custom JavaScript motion is used.
- Reduced-motion cannot be controlled in third-party README SVG widgets, so motion is kept limited and non-essential.

## Depth

- No custom shadows or glassmorphism.
- Depth comes from GitHub's native Markdown rendering, image gradients, table boundaries, and SVG widget contrast.

## Superloopy Dials

- `DESIGN_VARIANCE`: 6
- `MOTION_INTENSITY`: 3
- `VISUAL_DENSITY`: 6

## Do / Don't

- Do use the navy, blue-green, amber, and cyan palette consistently.
- Do keep project copy specific and tied to real repositories.
- Do prefer useful dynamic widgets over novelty widgets.
- Don't use purple-blue glow gradients.
- Don't add fake screenshots, fake stats, placeholder projects, or generic AI portfolio claims.
- Don't add more automation until the README MVP is reviewed in GitHub.
