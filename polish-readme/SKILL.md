---
name: polish-readme
description: Create or redesign repository READMEs with concise setup and useful visuals; handle repository descriptions, pushes and visibility changes only when requested.
---

# Polish README

Give the repository a clear, visually coherent front page that helps a new reader understand the project and start using it. Ground the presentation in the actual implementation.

## 1. Establish the facts

Read the existing README, repository instructions, entry points, manifests, configuration and relevant assets. Identify the audience, purpose, supported platforms, setup commands and material limitations. Use configuration as the source of truth for versions, counts and commands; verify rather than copy stale claims.

Preserve attribution, licensing and working instructions. Identify setup, permissions, recovery or troubleshooting material worth moving into a linked guide.

**Complete when:** the purpose and quick start are supported by repository evidence, and essential caveats have a clear home.

## 2. Build the front page

Use this preferred shape, adapting it to the project:

- A responsive SVG banner with the project name, a concrete tagline and a few factual highlights. Reuse the existing visual identity when one exists.
- A short purpose statement and the shortest complete quick start.
- A small feature list or comparison table where it makes choices easier to scan.
- One Mermaid workflow when the flow explains how the project works.
- Links to configuration, detailed usage and recovery instructions.

Aim for roughly 40–90 lines as a guide, not a quota. Keep platform requirements, administrator access, persistent permissions and important failure/recovery behavior visible near the relevant setup steps. Put the full procedures in a linked guide instead of deleting them to shorten the README.

For visuals:

- Prefer self-contained SVG for banners and existing screenshots for real UI. Label illustrative mockups as examples.
- Give SVGs a viewBox, an accessible title/description, readable contrast and essential text that stays legible at README width. Add useful image alt text.
- Use badges for verified facts; add a license badge only when that license exists.
- Choose diagrams and tables for explanation, rather than repeating decorative elements. Keep commands and essential information available as text.

**Complete when:** the opening explains what the project does, setup is runnable, and each visual contributes without introducing unsupported claims.

## 3. Validate the result

Check relative image/file links and heading anchors from the document containing them. When moving a guide, update its relative asset paths. Parse new SVGs as XML and render the visuals with tools permitted by the environment; inspect clipping and essential-text readability at desktop and narrow widths. Check Markdown with the target renderer when available.

Review the diff for lost setup or safety information and unintended runtime changes. Keep catalogues, descriptions and visual counts consistent with changed repository contents. Documentation-only changes need link, content and rendering checks; exercise runtime behavior when the task also changes it.

**Complete when:** links and anchors resolve, supported render checks pass, and any unverified rendering or behavior is identified explicitly.

## 4. Deliver within scope

For requested repository-description updates, commits/pushes or visibility changes, read [Publishing](references/publishing.md). A README request by itself authorizes preparing documentation, not those external actions.

Summarize the result with the repository or changed-document link, relevant checks and remaining limits. Report publication only after verifying the remote state.

**Complete when:** the requested artifacts are reviewable and every requested external action is either verified or reported with its concrete blocker.
