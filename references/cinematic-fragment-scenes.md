# Reference 9: Cinematic fragment scene transitions

**Status:** reference and proposed recipe only; no component, demo or deployment.

**Source:** [Web Fueled reel](https://www.facebook.com/reel/2141634959723541) · [User-submitted share](https://www.facebook.com/share/r/1F6W9TTunB/).

**Intake:** October 12, 2026. The parent researcher supplied observations from a research worker's inspection of approximately 13 seconds of actual playback in dot's cloud browser. This documentation task did not independently inspect the source. Facebook's AI-generated description is not used as independent evidence.

## Observed in the recording

- Saturated blue/cyan river and mountain imagery, oversized pink/yellow flowers and a brush-like sweep.
- A transition into a dark rain-lit street with cyan, amber, red and violet reflections.
- Rectangular strips and tiles smear and reassemble into dimensional scene reveals.
- Short, heavy uppercase headlines near the top center and a minimal menu at the top right.
- A hand on a trackpad and a highlighted pointer accompany scene changes.

## Unknowns and attribution limits

The exact interaction trigger is unverified: the hand/pointer recording does not establish scroll, drag, hover or time-based control. An overlay claims **GSAP + Three.js**, but no inspected source code or live-site URL establishes the actual stack. Apparent depth does not prove WebGL or real-time 3D. Exact durations, easing, fonts, assets, mobile behavior, keyboard access and menu behavior are unverified. Treat the hand and pointer as recording context, not required page decoration.

## Proposed original reusable pattern — not source reconstruction

Build a cinematic scene-transition sequence with configurable original imagery, semantic HTML headlines and a clear final project CTA. Let staggered rectangular fragments briefly bridge scenes, then settle into a readable composition. Keep depth restrained and copy stable rather than fragmenting text with the imagery.

Suggested original Glytched concept: a cobalt landscape, an expressive abstract studio scene and a rain-lit futuristic street. Give each a distinct approved headline and end with a project CTA. These three scenes and the CTA are our proposed narrative, not an assertion that all appear in the source.

Start with a lightweight 2D composition using a bounded number of clipped image regions and transform/opacity transitions. Reuse one responsive scene asset across fragments; do not download an image per tile. Use WebGL only if meaningful depth cannot be achieved efficiently in 2D and device testing justifies its cost. GSAP is not a requirement merely because an overlay names it.

A bounded pinned scroll timeline is one possible implementation, **not verified source behavior**. If selected, map native scroll position to scene progress with natural entry/exit and reversible transitions. Do not intercept wheel/touch gestures, trap navigation or introduce long empty scroll distances. Explicit scene controls are another possible approach; select and document one interaction model before building. If automatic playback is chosen, provide a visible keyboard-operable pause and no autoplay audio.

## Configuration and component contract

| Piece | Editable inputs / proposed behavior |
| --- | --- |
| SceneSequence | Ordered scenes, chosen interaction mode, transition timing/range, optional pinning, current scene state and cleanup lifecycle |
| SceneMedia | Original/licensed image, dimensions, responsive sources, desktop/mobile focal points, alt text or decorative status, provenance |
| FragmentTransition | Bounded fragment count, strip/tile layout, stagger, direction, displacement, easing and depth limits |
| SceneCopy | Approved headline/supporting copy in HTML, contrast backing and readable placement; not canvas-only text |
| Navigation | Semantic menu and optional scene controls with visible focus, meaningful names and logical order |
| ProjectCTA | Clear label and working approved destination, reachable with keyboard and without motion |

Expose palette, typography, spacing, overlay contrast, scene ordering, media URLs, crop/focal points, transition timing, fragment limits, depth intensity, interaction mode, scroll range where applicable and fallback scene. Avoid invented metrics, endorsements or product claims.

## Responsive, accessibility and performance requirements

- **Mobile:** use fewer fragments, less displacement/depth, a shorter unpinned sequence or a static stacked layout. Keep headlines and CTA clear of focal subjects, menus usable and touch targets comfortable. No horizontal overflow at 320px.
- **Semantic access:** keep text, navigation and CTA in HTML and logical reading order. Mark decorative fragments hidden from assistive technology; avoid repeated image descriptions. Give meaningful images appropriate alternatives. Do not duplicate interactive elements inside fragments.
- **Motion:** provide a readable static layout for reduced motion, JavaScript failure and unsupported effects. Preserve every essential message and CTA; a single fallback image must not hide scene-specific information. Avoid flashing and rapid high-contrast cuts. Retain native scrolling and keyboard operation.
- **Contrast:** verify text and focus indicators against all transition states, with stable backing where needed. Do not make the headline readable only after an animation finishes.
- **Loading:** compress responsive imagery, specify dimensions, prioritize the first scene and lazy-load later scenes near use. Hold the current image until the next is decoded; avoid blank transitions. Bound asset/layer count and measure memory, frame stability and layout shift.
- **Lifecycle:** suspend unnecessary work offscreen/when hidden, remove listeners on teardown and dispose GPU resources if an optional WebGL enhancement is used. Keep the 2D/static fallback usable when the renderer fails.

## Originality and future acceptance

Create new imagery and branding; do not copy the source's artwork, footage, lettering, identity or proprietary code. Record license provenance or exact generation prompts. A link to the reel grants no reuse rights.

Future acceptance: coherent original scene narrative, restrained fragment motion, readable HTML copy and a working final CTA on desktop and phones. Test the selected interaction trigger, keyboard/focus/menu behavior, native scrolling and optional pinning, reduced motion, no-JS and failed-media fallbacks, responsive focal points, contrast throughout transitions, loading/layout stability and cleanup. Compare 2D and any proposed WebGL cost before choosing dependencies. Report measured results and unrun checks separately. **No implementation QA has been run for this documentation-only concept.**

Related: [Forme architecture/materials](architecture-materials-forme.md) offers a separate owner-requested day-to-night scroll direction; do not transfer that verified owner preference into a claim about this reel's trigger.

[Reusable prompt](../prompts/cinematic-fragment-scenes.md) · [Reference index](README.md)
