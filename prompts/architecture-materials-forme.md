# Reusable prompt: Cinematic architecture and materials

**Status:** prompt only. No demo, component or deployment is authorized by this catalog entry.

[Source observations and uncertainty](../references/architecture-materials-forme.md)

## Requested interaction and provenance

Dex specifically values the hero shifting from daytime to night **as the user scrolls** (owner observation, October 10, 2026). The parent browser review saw the lighting change but did not independently establish its trigger. Implement the requested scroll-driven direction as an original design; do not claim the source trigger or technical method is verified.

## Supply project inputs

```yaml
brand_name: ""
audience_and_project_purpose: ""
approved_navigation: [] # label and actual destination
hero_eyebrow: ""
hero_heading: ""
hero_supporting_copy: ""
primary_cta: {} # approved label and actual destination/action
story: {} # real URL or playable media; omit if unavailable
editorial_intro: ""
material_cards: [] # three: name, approved copy, image, alt, optional URL
image_cta: {} # image, heading, copy, actual destination
footer: {}
assets_and_provenance: [] # licensed/generated media and usage rights
image_focal_points: {} # desktop and phone
font_display_and_license: ""
font_body_and_license: ""
color_tokens: {} # charcoal/brown/ivory/stone/taupe only if brand-appropriate
spacing_type_and_layout_tokens: {}
stack_and_integration_target: ""
motion_mode: "scroll-day-to-night"
matched_scene_assets: {} # original day/dusk/night, same geometry/camera, or appropriate original scene
scroll_range_and_stops: {} # bounded start/end, day/dusk/night stops and interpolation
optional_pinning: false # only if useful; short bounded range, natural entry/exit
mobile_scroll_range: {} # prefer shorter, unpinned progression
static_fallback_scene: "" # readable still for reduced motion/no-JS/media failure
static_view_and_ambient_pause_labels: {}
media_and_dependency_budget: {}
```

## Prompt to use when implementation is separately authorized

> Build an original responsive architecture/materials landing page for the supplied brand and audience. Use approved original copy and licensed or newly generated imagery. Aim for cinematic architectural photography and quiet editorial layout, with restrained warm/cool light and generous spacing. Adapt the palette and type to this brand; do not copy Forme branding, source imagery, exact layout, promotional reel overlays or proprietary code. Source technology and fonts are unverified.
>
> Compose Header, CinematicHero, PillButton, StoryLink, MaterialCard, MaterialsSection, ImageCTA and Footer as reusable pieces. Use a slim overlay header where contrast permits; a left-aligned hero eyebrow, prominent serif heading and short supporting text; a primary filled pill action and optional story/play link; an editorial introduction on a light surface; three tall material-image cards; a panoramic image CTA; and a compact footer. Preserve coherent hierarchy rather than treating these as fixed pixel positions. Only show a play affordance when working media or a genuine story destination is supplied. All CTAs must perform their stated action; if this is a fictional demo, label it clearly and use transparent demo-only behavior rather than collecting orders or enquiries.
>
> Expose typography, color, spacing, container, card ratio, pill shape, focus, responsive focal-point and motion tokens, plus all content and asset inputs. Use semantic landmarks/headings, native links/buttons, logical focus order, visible focus, sufficient contrast and comfortable touch targets. Keep all important content available without hover, dragging or motion. On phones, stack the material cards, preserve the image subject and prevent text/media collisions or horizontal overflow.
>
> Make the hero’s day-to-night change explicitly scroll-driven: map a bounded scroll range to matched original daytime, dusk and night imagery, or an appropriate original scene with controllable lighting. Preserve camera, geometry and focal points between states. Progress smoothly toward night when scrolling forward and reverse toward day when scrolling back; hold the state when scrolling stops. Timed ambient playback alone does not meet this requirement. Keep hero text and CTAs stable and readable at every intermediate state. These are proposed techniques, not verified source implementation.
>
> Use restrained pinning only if it helps, with a short bounded scroll range and natural entry/exit. Do not hijack native scrolling or make later content difficult to reach. On phones, prefer a shorter unpinned progression and responsive focal points; support touch, wheel and keyboard scrolling. Start with a strong compressed still and retain a static reduced-motion/no-JS/media-failure fallback with all content visible. Offer a static-view control where useful. If sustained automatic firelight or other ambient motion is added, provide a visible keyboard-operable pause. No autoplay audio. Do not add or describe a verified helix carousel: the caption mentions one but none was observed.
>
> Use responsive image sizes and explicit dimensions, prioritize the hero still, lazy-load secondary media and measure loading/layout stability. Do not add a large renderer without a concrete need and budget. Pause offscreen/hidden-page motion and clean up listeners when applicable. Inspect existing reusable components and adapt suitable layout/card/fallback patterns; preserve existing assets and avoid building a duplicate framework.
>
> Return editable source, configuration instructions, asset/license provenance and generation prompts where used, plus integration guidance for the selected stack. Test forward/reverse progression, unchanged lighting while scroll is stationary, restored scroll positions, optional pinning entry/exit, native mobile/keyboard scrolling, desktop and phone layouts, keyboard/focus, contrast across media states, touch targets, all destinations, media failure, no-JS, reduced motion, pause and loading performance. Acceptance requires cinematic photography with quiet editorial hierarchy, a smooth reversible scroll-driven day-to-night hero, efficient loading and full usability without motion. Report actual QA and unrun checks separately; do not claim verified behavior based on this reference. Do not publish, deploy, buy services or change production without separate authorization.

## Evidence boundary

The [brief](../references/architecture-materials-forme.md) records parent-attributed playback observations from October 10, 2026. Dex’s owner observation supplies the requested scroll trigger; the browser review did not independently establish it. Mobile, hover, drag and keyboard behavior, exact fonts, original trigger/animation mechanism and real-time 3D remain technically unverified. This prompt is an original implementation proposal, not a reconstruction or proof of the source’s implementation.
