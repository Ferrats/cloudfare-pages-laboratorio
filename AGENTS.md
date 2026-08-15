# Project instructions

This repository is a small Astro experiment used to validate the workflow from Codex to GitHub and Cloudflare Pages.

## Architecture

- Keep the site statically generated with Astro.
- Prefer Astro components, semantic HTML and CSS over client-side JavaScript.
- Keep page composition in `src/pages`, reusable UI in `src/components` and global styles in `src/styles`.
- Do not add frameworks, databases, APIs, CMSs or runtime services unless the experiment explicitly requires them.
- Avoid dependencies that do not provide clear value to the current test.

## Design

- Preserve the editorial, high-contrast visual language and generous spacing.
- Use the existing design tokens before introducing new colors, spacing or typography values.
- Make layouts work from small mobile screens through large desktop screens.
- Prefer content clarity and hierarchy over decorative effects.

## Accessibility

- Use semantic landmarks and a logical heading hierarchy.
- Maintain visible keyboard focus and sufficient color contrast.
- Do not rely on color alone to convey meaning.
- Respect reduced-motion preferences when adding animation.
- All meaningful images require useful alternative text; decorative images should use empty alt text.

## Quality

- Run `npm run build` before proposing changes.
- Keep copy in Brazilian Portuguese unless otherwise requested.
- Update the README when setup or deployment steps change.

