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
- The parent browser review observed hero lighting shifts from dusk to blue hour, with changing firelight. That review did not independently establish the input trigger or animation mechanism.

## Owner observation and requested direction

On October 10, 2026, Dex said: “I appreciate the fact that as you scroll, the hero shifts from daytime to night. I thought that was a pretty neat touch”. This is an owner-observed interaction and the specifically requested design direction: **scroll-driven day-to-night progression**. The browser review independently observed lighting change, but did not establish that scrolling triggered it. Retain both accounts without presenting the original trigger, rendering technique or implementation as technically verified.

## Source uncertainty and exclusions

Exact fonts and implementation stack are unknown. Mobile layout, hover, drag, keyboard operation and the destinations/behavior of the CTAs and play link were not demonstrated. The caption says **“3D Helix Image Carousel”**, but no helix was observed; neither a helix carousel nor real-time 3D is verified. Do not infer either from the caption. The reel’s neon promotional heading and laptop frame are presentation overlays, not website elements to reproduce.

## Proposed original recipe — not observed implementation

Create an original responsive architecture/materials landing page. Combine cinematic photography with quiet editorial spacing and a clear content hierarchy. Use a new identity, approved original copy and licensed or generated imagery; do not reproduce the source composition pixel for pixel.

| Proposed component | Editable inputs and behavior |
| --- | --- |
| Header | Brand/wordmark, navigation labels/targets, outlined PillButton. Overlay only where contrast remains reliable; provide a usable compact mobile layout. |
| CinematicHero | Eyebrow, heading, supporting copy, responsive media, focal points, filled PillButton and optional StoryLink. Keep copy stable and readable over a scroll-driven day/dusk/night scene progression. |
| PillButton | Label, verified destination or actual action, fill/outline variant and focus treatment. Use links for navigation and buttons for actions. |
| StoryLink | Approved story destination or playable media with accessible controls. Omit the play affordance if no working media/story exists. |
| MaterialCard | Original image, alt text, material name, approved description and optional real destination. Do not invent performance/sustainability claims. |
| MaterialsSection | Editorial introduction, three editable cards, grid gaps and reading order. Stack cards on phones. |
| ImageCTA | Panoramic image/focal point, contrast layer, short heading and working CTA. |
| Footer | Approved identity, navigation and appropriate legal/context text. |

The proposed reusable hero maps normalized scroll position over a bounded section to a smooth, reversible **day → dusk → night** progression. Scrolling back restores earlier lighting states; leaving scroll position unchanged holds the scene state. Use matched original daytime/dusk/night imagery with consistent camera, geometry and focal points, or an appropriate original scene whose lighting can be controlled efficiently. A crossfade between matched scenes is one possible implementation, not a verified source technique. Timed ambient playback alone does not satisfy this requested interaction.

Keep hero text and CTAs stable and readable throughout the transition. Use restrained pinning only when it improves the composition, with a short bounded range and natural entry/exit; do not trap scroll or delay access to later content. On phones, prefer a shorter unpinned range, responsive media and carefully matched focal points. The effect must work with native touch, wheel and keyboard scrolling without intercepting those inputs.

Start with a good still and use it under reduced motion, disabled JavaScript, media failure or unsupported effects, retaining all essential content. Provide an optional static-view control; if any sustained automatic firelight or other ambient motion is added, give it a visible keyboard-operable pause. Avoid autoplay audio. Do not add helix behavior on the strength of an unverified caption. All of these are proposed original implementation requirements, not claims about the source code.

## Tokens and content contract

Expose `font_display`, `font_body`, type sizes/line heights, `color_background`, `color_surface`, `color_text`, `color_muted`, `color_accent`, overlay strength, spacing, container widths, card aspect ratios, pill radius, focus style, breakpoints, desktop/mobile image focal points, motion mode, scroll start/end range, day/dusk/night stops, interpolation, optional pinning range, mobile range, static fallback scene and static-view/pause labels. Content inputs: identity, nav items, hero copy/CTAs, story destination/media, material cards, CTA copy/destination, footer and each asset’s alt text/license/provenance.

## Accessibility, mobile and performance requirements

Use semantic landmarks, one primary heading, logical heading/focus order, visible focus and keyboard-operable controls. Meet WCAG AA text contrast; check copy against the brightest and darkest media states. Use comfortable touch targets (aim for 44px) and avoid hover-only content. On phones, preserve subject focal points without covering text, stack material cards and keep navigation reachable. At 320px, no unintended horizontal scrolling.

Use responsive, compressed images with explicit dimensions; prioritize the hero still and lazy-load secondary imagery. A still should remain useful before additional scene states load. Load matched scene states before blending to avoid flashes; avoid a large image sequence or renderer without a measured need. Budget and measure media bytes; justify animation dependencies rather than assuming a rendering library is required. Pause unnecessary motion offscreen/when hidden and clean up listeners if integrated into a dynamic page.

## Rights and acceptance

Linked footage grants no asset, font, brand or code reuse rights. Maintain an asset register for licensed or generated media, including exact generation prompts where relevant. Use approved facts only; do not invent testimonials, certifications or technical claims.

Future acceptance: cinematic imagery and quiet editorial hierarchy at desktop and phone sizes; efficient loading with minimal layout shift; working navigation/CTAs; readable copy in every lighting state; smooth reversible day/dusk/night changes tied to scroll position; no autonomous lighting progression while scroll is stationary; usable without motion. Test forward/reverse and restored scroll positions, mobile/native scrolling, optional pinning entry/exit, keyboard/focus, contrast, touch layout, reduced-motion, no-JS, media failure, static-view and pause controls, loading/layout stability and the chosen CMS integration. Record actual results and unrun checks separately. **No component, responsive or animation QA has been run: this deliverable is documentation only.**

Related direction: architectural scene storytelling and cinematic product-showcase recipes. Reuse suitable existing layout/card/fallback patterns when a build is separately authorized; do not duplicate a framework or modify the original six templates.

[Reusable implementation prompt](../prompts/architecture-materials-forme.md)
