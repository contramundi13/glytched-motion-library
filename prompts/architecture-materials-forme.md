# Reusable prompt: Cinematic architecture and materials

**Status:** prompt only. No demo, component or deployment is authorized by this catalog entry.  
[Source observations and uncertainty](../references/architecture-materials-forme.md)

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
motion_mode: "static" # optional ambient video or dusk/blue-hour crossfade
motion_duration_and_pause_label: {}
media_and_dependency_budget: {}
```

## Prompt to use when implementation is separately authorized

> Build an original responsive architecture/materials landing page for the supplied brand and audience. Use approved original copy and licensed or newly generated imagery. Aim for cinematic architectural photography and quiet editorial layout, with restrained warm/cool light and generous spacing. Adapt the palette and type to this brand; do not copy Forme branding, source imagery, exact layout, promotional reel overlays or proprietary code. Source technology and fonts are unverified.
>
> Compose Header, CinematicHero, PillButton, StoryLink, MaterialCard, MaterialsSection, ImageCTA and Footer as reusable pieces. Use a slim overlay header where contrast permits; a left-aligned hero eyebrow, prominent serif heading and short supporting text; a primary filled pill action and optional story/play link; an editorial introduction on a light surface; three tall material-image cards; a panoramic image CTA; and a compact footer. Preserve coherent hierarchy rather than treating these as fixed pixel positions. Only show a play affordance when working media or a genuine story destination is supplied. All CTAs must perform their stated action; if this is a fictional demo, label it clearly and use transparent demo-only behavior rather than collecting orders or enquiries.
>
> Expose typography, color, spacing, container, card ratio, pill shape, focus, responsive focal-point and motion tokens, plus all content and asset inputs. Use semantic landmarks/headings, native links/buttons, logical focus order, visible focus, sufficient contrast and comfortable touch targets. Keep all important content available without hover, dragging or motion. On phones, stack the material cards, preserve the image subject and prevent text/media collisions or horizontal overflow.
>
> Start with a strong compressed still and stable readable copy. Only when assets and budget justify it, use a compressed ambient video with poster or a dusk/blue-hour image crossfade. Those are proposed implementations, not verified source techniques. Supply visible keyboard-operable pause for sustained automatic motion, no autoplay audio, and a static reduced-motion fallback. Maintain semantic content if JavaScript or media fails. Avoid scroll hijacking. Do not add or describe a verified helix carousel: the caption mentions one but none was observed.
>
> Use responsive image sizes and explicit dimensions, prioritize the hero still, lazy-load secondary media and measure loading/layout stability. Do not add a large renderer without a concrete need and budget. Pause offscreen/hidden-page motion and clean up listeners when applicable. Inspect existing reusable components and adapt suitable layout/card/fallback patterns; preserve existing assets and avoid building a duplicate framework.
>
> Return editable source, configuration instructions, asset/license provenance and generation prompts where used, plus integration guidance for the selected stack. Test desktop and phone layouts, keyboard/focus, contrast across media states, touch targets, all destinations, media failure, no-JS, reduced motion, pause and loading performance. Acceptance requires cinematic photography with quiet editorial hierarchy, efficient loading and full usability without motion. Report actual QA and unrun checks separately; do not claim verified behavior based on this reference. Do not publish, deploy, buy services or change production without separate authorization.

## Evidence boundary

The [brief](../references/architecture-materials-forme.md) records parent-attributed playback observations from October 10, 2026. Mobile, hover, drag and keyboard behavior, exact fonts, animation mechanism and real-time 3D remain unverified. This prompt is an original implementation proposal, not a reconstruction or proof of the source’s implementation.
