# Reference 8: Cinematic architecture and materials

**Status:** reference recipe only; no implementation or deployment.

**Source:** [Web Fueled — Forme concept](https://www.facebook.com/reel/1446200427463376) · [Dex’s submitted share](https://www.facebook.com/share/r/1BDWZSoXTr/)

**Submitted:** October 10, 2026. **Observation provenance:** the parent researcher reviewed actual public playback in dot’s cloud Chrome without login. This documentation task did not independently inspect playback. Forme identifies the reference, not a brand to reuse.

## Observed website composition

- A dark, full-width architectural interior hero: stone fireplace, mountain/water outlook and warm firelight.
- A slim overlaid header with a small wordmark, compact navigation and an outlined pill CTA.
- Left-aligned hero copy: uppercase eyebrow, oversized ivory high-contrast serif heading, short supporting text, pale filled pill CTA and secondary play link.
- An ivory editorial introduction followed by three prominent tall photographic material cards.
- A dark panoramic image-backed CTA and a narrow footer.
- Charcoal, deep brown, ivory, stone and taupe, accented by amber firelight and muted blue scenery. These are descriptive observations, not sampled production color values.
- Hero lighting shifts from dusk to blue hour, with changing firelight. The mechanism is unknown.

## Source uncertainty and exclusions

Exact fonts and implementation stack are unknown. Mobile layout, hover, drag, keyboard operation and the destinations/behavior of the CTAs and play link were not demonstrated. The caption says **“3D Helix Image Carousel”**, but no helix was observed; neither a helix carousel nor real-time 3D is verified. Do not infer either from the caption. The reel’s neon promotional heading and laptop frame are presentation overlays, not website elements to reproduce.

## Proposed original recipe — not observed implementation

Create an original responsive architecture/materials landing page. Combine cinematic photography with quiet editorial spacing and a clear content hierarchy. Use a new identity, approved original copy and licensed or generated imagery; do not reproduce the source composition pixel for pixel.

| Proposed component | Editable inputs and behavior |
| --- | --- |
| Header | Brand/wordmark, navigation labels/targets, outlined PillButton. Overlay only where contrast remains reliable; provide a usable compact mobile layout. |
| CinematicHero | Eyebrow, heading, supporting copy, responsive media, focal points, filled PillButton and optional StoryLink. Keep copy stable and readable. |
| PillButton | Label, verified destination or actual action, fill/outline variant and focus treatment. Use links for navigation and buttons for actions. |
| StoryLink | Approved story destination or playable media with accessible controls. Omit the play affordance if no working media/story exists. |
| MaterialCard | Original image, alt text, material name, approved description and optional real destination. Do not invent performance/sustainability claims. |
| MaterialsSection | Editorial introduction, three editable cards, grid gaps and reading order. Stack cards on phones. |
| ImageCTA | Panoramic image/focal point, contrast layer, short heading and working CTA. |
| Footer | Approved identity, navigation and appropriate legal/context text. |

Suggested motion options, subject to assets and budget: a compressed ambient video with a poster, or a dusk/blue-hour image crossfade. These are proposed techniques, not claims about the reel. Start with a good still. Provide a visible, keyboard-operable pause for sustained automatic motion. Avoid autoplay audio and scroll hijacking. Under reduced motion, disabled JavaScript, media failure or unsupported effects, retain a readable static scene and all essential content. Do not add helix behavior on the strength of an unverified caption.

## Tokens and content contract

Expose `font_display`, `font_body`, type sizes/line heights, `color_background`, `color_surface`, `color_text`, `color_muted`, `color_accent`, overlay strength, spacing, container widths, card aspect ratios, pill radius, focus style, breakpoints, desktop/mobile image focal points, motion mode/duration and pause label. Content inputs: identity, nav items, hero copy/CTAs, story destination/media, material cards, CTA copy/destination, footer and each asset’s alt text/license/provenance.

## Accessibility, mobile and performance requirements

Use semantic landmarks, one primary heading, logical heading/focus order, visible focus and keyboard-operable controls. Meet WCAG AA text contrast; check copy against the brightest and darkest media states. Use comfortable touch targets (aim for 44px) and avoid hover-only content. On phones, preserve subject focal points without covering text, stack material cards and keep navigation reachable. At 320px, no unintended horizontal scrolling.

Use responsive, compressed images with explicit dimensions; prioritize the hero still and lazy-load secondary imagery. A still should remain useful before any video loads. Budget and measure media bytes; justify animation dependencies rather than assuming a rendering library is required. Pause unnecessary motion offscreen/when hidden and clean up listeners if integrated into a dynamic page.

## Rights and acceptance

Linked footage grants no asset, font, brand or code reuse rights. Maintain an asset register for licensed or generated media, including exact generation prompts where relevant. Use approved facts only; do not invent testimonials, certifications or technical claims.

Future acceptance: cinematic imagery and quiet editorial hierarchy at desktop and phone sizes; efficient loading with minimal layout shift; working navigation/CTAs; readable copy in every lighting state; usable without motion. Test keyboard/focus, contrast, touch layout, reduced-motion, no-JS, media failure, pause controls, loading/layout stability and the chosen CMS integration. Record actual results and unrun checks separately. **No component, responsive or animation QA has been run: this deliverable is documentation only.**

Related direction: architectural scene storytelling and cinematic product-showcase recipes. Reuse suitable existing layout/card/fallback patterns when a build is separately authorized; do not duplicate a framework or modify the original six templates.

[Reusable implementation prompt](../prompts/architecture-materials-forme.md)
