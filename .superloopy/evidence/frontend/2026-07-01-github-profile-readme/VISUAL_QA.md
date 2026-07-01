# Visual QA Evidence

Target: `README.md`

Environment: GitHub profile README Markdown. This is not a local web app, so there is no dev server or app route to screenshot before pushing. QA focused on Markdown structure, external image/link availability, design-token traceability, and anti-slop review.

## Render Structure

- `div` tags: 4 open / 4 close
- `table` tags: 1 open / 1 close
- `tr` tags: 2 open / 2 close
- `td` tags: 4 open / 4 close

## Link And Widget Checks

- capsule-render header/footer: HTTP 200
- readme-typing-svg: HTTP 200
- Shields.io badges: HTTP 200
- skill-icons groups: HTTP 200
- GitHub Stats Extended cards: HTTP 200
- Streak Stats card: HTTP 200
- Activity Graph: HTTP 200
- GitHub repository/profile links: HTTP 200
- Tistory link: HTTP 200
- YouTube link: HTTP 200
- Original `github-profile-trophy.vercel.app` returned HTTP 402, so it was replaced with the working public mirror `https://trophy.ryglcloud.net`.
- Final pass: all 34 README URLs responded successfully.
- Token pass: every hex color visible in `README.md` is declared in `DESIGN.md`.

## Superloopy Anti-Slop Pre-Flight

- [x] Zero em-dashes anywhere visible in `README.md`.
- [x] Eyebrow count is within limit: no uppercase tracked label system.
- [x] No AI-purple/glow default.
- [x] Typography is deliberate within Markdown/SVG constraints.
- [x] No premium beige/brass palette.
- [x] Color/theme consistency locks hold.
- [x] Layout families vary: hero, intro copy, code rhythm, table, badges/icons, metrics, footer.
- [x] No div-based fake screenshots.
- [x] Copy avoids banned AI cliches and fake-perfect stats.
- [x] No micro-tell catalogue items used.
- [x] Motion claimed is implemented through actual SVG services.
- [x] Colors trace to `DESIGN.md`; URL hex values are required by external SVG APIs.
- [x] Interactive states are GitHub-native link behavior.
- [x] No custom layout likely to introduce horizontal scroll; GitHub Markdown tables may scroll natively on small screens if needed.

## Result

PASS for a GitHub README MVP. Final browser-level QA should be done on the live GitHub profile after the commit is pushed.
