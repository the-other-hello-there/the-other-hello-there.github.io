# Main personal website preferences

This repository is Henry Luo's personal landing page, separate from the engineering portfolio repository.

- Match the engineering portfolio's dark navy palette, cyan accents, serif typography, rounded buttons, and restrained styling.
- Keep the homepage a simple gateway to published portfolios. Do not add project galleries, work experience, a resume, or detailed credentials here.
- Currently show only the Engineering Portfolio link at /HenryLuo-Portfolio/.
- The user plans a music portfolio in the future. Remember this when extending the navigation, but do not mention music, future portfolios, placeholders, or coming-soon content on the website until explicitly requested.
- These notes are repository instructions, not homepage copy. They are not private if the repository/site is public.

## Keep styling synchronized across both websites

Explicit user preference: the personal landing page and engineering portfolio must have identical shared visual styling. A styling change in either repository must lead to the corresponding change in the other during the same task, unless the user explicitly requests an exception.

- Engineering portfolio: ../EngineeringPortfolio/index.html and ../EngineeringPortfolio/assets/css/styles.css.
- Personal landing page: ../LandingPage/index.html (currently uses inline CSS).
- Keep shared colors, typography, branding, buttons, borders, radii, focus/hover states, and responsive styling consistent. Inspect both implementations before editing; do not update only the active repository and overlook the counterpart.
- Preserve each page's purpose and appropriate layout. Synchronizing styling does not mean copying projects, experience, resume content, or portfolio-specific components onto the landing page.
- Check both pages after shared styling changes. If the other repository is unavailable or a write is blocked, report that synchronization remains incomplete rather than claiming both were updated.
- This is a standing instruction for future edits, not an automatic file synchronization mechanism.

## Local repository locations

- Shared parent: `C:\Users\rrenkit\OneDrive\Github Pages`.
- Personal landing repository: `LandingPage`.
- Engineering portfolio repository: `EngineeringPortfolio`.
- These replace the former folders under `OneDrive\ME`.
- Local renaming does not change GitHub repository names or published URLs.
- Preserve `https://the-other-hello-there.github.io/` and its `/HenryLuo-Portfolio/` website path unless separately requested.

## Agent context files

- AGENTS.md is the single source of agent context for this repository. Record all agent instructions, preferences, and project notes here only.
- Do not create or update agent-specific context files (for example CLAUDE.md, CLAUDE.local.md, GEMINI.md, .cursorrules, .cursor/rules/, or .github/copilot-instructions.md). They are git-ignored and not shared. If one exists locally, move any useful content into AGENTS.md.
- AI session and local tool settings (for example .claude/, .cursor/, .codex/, .gemini/) are git-ignored and must not be committed.
