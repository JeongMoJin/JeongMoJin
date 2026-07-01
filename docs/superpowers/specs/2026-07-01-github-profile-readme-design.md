# GitHub Profile README Redesign

Date: 2026-07-01
Owner: JeongMoJin
Theme: Recording Creative Tech Builder

## Goal

Redesign the profile `README.md` for `JeongMoJin/JeongMoJin` so the GitHub profile feels artistic, current, memorable, and credible. The profile should present Jeong Mo Jin as a builder who records, analyzes, designs, and ships creative technology projects across public data, AI, web products, Unity media art, and visual storytelling.

## Current Context

- The repository currently contains only `README.md`.
- The existing README has a simple greeting, a capsule-render header, a top languages card, and a large commented-out badge list.
- Public profile signals include:
  - Display name: `LearnAndRecord`
  - Location: Daegu, South Korea
  - Links: Tistory blog and YouTube
  - Recent repositories: `jangbogi365`, `kyo-map`, `Flag_MediaFrame`, `intraflow`, `Buyeo_Cheongyang_Flood_Project`, `eum-culture-contest`, `jeju8760`, and other contest/data/product projects.

## Non-Goals

- Do not rewrite unrelated files.
- Do not add source code for a separate website.
- Do not add npm, Python, or other runtime dependencies.
- Do not copy old source code from other projects.
- Do not overload the page with every possible widget if it harms clarity or elegance.

## Design Direction

Use a curated, premium GitHub profile style:

1. Hero
   - Use `capsule-render` for a cinematic header.
   - Pair it with `readme-typing-svg` for a concise animated identity line.
   - Lead with `LearnAndRecord` and a clear Creative Tech Builder message.

2. Identity
   - Present a short bilingual Korean/English introduction.
   - Emphasize the loop: data -> product -> media art -> record.
   - Keep copy specific, confident, and not too long.

3. Links
   - Use `shields.io` badges for GitHub, Tistory, YouTube, and location/focus labels.
   - Keep badge colors consistent with the overall palette.

4. Featured Work
   - Highlight 4 to 6 public projects as a curated portfolio wall.
   - Prioritize recent and distinctive work:
     - `jangbogi365`
     - `Flag_MediaFrame`
     - `intraflow`
     - `Buyeo_Cheongyang_Flood_Project`
     - `eum-culture-contest`
     - `jeju8760`
   - Each item should have one short line explaining the value, not just the tech.

5. Stack
   - Use `skill-icons` for the main engineering stack.
   - Use selected `shields.io` badges where icons are missing or more expressive.
   - Group by purpose rather than dumping every technology:
     - Build
     - Data
     - Creative / Media
     - Tools

6. Metrics
   - Use dynamic cards selectively:
     - GitHub Stats Extended for stats and top languages
     - Streak Stats for contribution continuity
     - GitHub Readme Activity Graph for recent movement
     - Profile Trophy as a compact achievement strip
   - Prefer transparent or cohesive themes and hide borders where possible.
   - Avoid adding too many cards above the fold.

7. Motion / Signature
   - Add a tasteful footer wave via `capsule-render`.
   - Optionally add contribution snake later through GitHub Actions, because it requires generated assets and repository workflow permissions.

## Initial MVP

Update only `README.md` with the curated static/dynamic profile layout. Keep it self-contained and functional without requiring GitHub Actions.

## Optional Follow-Up

Add a separate GitHub Actions workflow for contribution snake or generated summary assets after the README redesign is reviewed. This keeps the first implementation small and avoids mixing visual redesign with automation setup.

## Acceptance Criteria

- `README.md` renders as a polished GitHub profile page.
- The first viewport clearly communicates `LearnAndRecord` and the Creative Tech Builder identity.
- Links point to the correct profile, blog, and YouTube destinations where known.
- Dynamic widgets use the `JeongMoJin` username.
- Project descriptions are accurate based on public repository descriptions.
- The page remains readable if external widget services temporarily fail.
- No unrelated files are modified during the MVP implementation.

## Verification Method

- Inspect the Markdown for broken tags, invalid links, and malformed query strings.
- Run a local Markdown/link sanity check where practical.
- Review `git diff` to ensure only intended files changed.
- If possible, preview the README through GitHub or a Markdown renderer after pushing.

## Self-Review Notes

- Scope is intentionally limited to a README MVP.
- Workflow automation is deferred to a follow-up task to keep the first change reviewable.
- The design uses many high-quality GitHub README tools, but only where they support the profile story.
