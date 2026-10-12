# Reusable prompt: Object Explorer

**Status:** documentation only; no build or deployment authorized by this prompt.

[Source brief](../references/object-explorer.md)

## Inputs

```yaml
brand_and_audience: ""
approved_brand_statement: ""
object_assets_and_provenance: []
approved_views_and_focal_points: []
approved_material_or_color_options: []
annotations: [] # approved text and optional visual anchors
palette_and_typography: {}
interaction_mode: "" # choose explicitly; source behavior is unverified
motion_and_performance_budget: {}
static_fallback_image: ""
cta_label_and_destination: {}
stack_and_integration_target: ""
```

## Prompt for a separately authorized implementation

> Create an original Object Explorer for the supplied brand: transition from a strong brand statement into clear annotated object details. An optional direction is an Inspired Creations shirt/hoodie customization study using approved assets and real supported options, or a Glytched digital sculpture with restrained cyan/magenta light. Choose one coherent direction. Do not copy Raymond branding, source copy, garment imagery, footage or creator code; do not invent fit/fabric claims or imply a commercial partnership.
>
> Start with a licensed/generated still and accessible HTML details. Add bounded view changes with a lightweight image sequence or optional renderer only when justified by assets and measured cost. Source claims about scroll rotation, colors and WebGL/Three.js are not verified requirements. Select and document the interaction model. Keep native scrolling intact and give users explicit touch/keyboard controls; do not require hover or dragging.
>
> Expose imagery, views, focal points, approved options, annotation anchors/text, type/palette, motion limits, fallback image and CTA. Keep brand headings, labels, details, navigation and CTA in semantic HTML. Associate annotations with a readable detail list; decorative leader lines must not carry information alone. Move details below the object on phones, use comfortable touch targets, visible focus and adequate contrast, and avoid copying the source's tiny indicators. Represent color/material previews honestly without claiming unsupported availability or exact physical accuracy.
>
> Reduced motion, no-JS and failed media/rendering must show a static object with all essential details and a working CTA. Compress responsive images, set dimensions, defer secondary views, suspend unnecessary offscreen work and clean up listeners/GPU resources. No live transactions or lead collection unless separately authorized.
>
> Return editable source/configuration, asset provenance and generation prompts where applicable, integration instructions and actual QA. Test keyboard, touch, pointer, responsive annotations, contrast, reduced motion, media failure, no-JS, loading and lifecycle cleanup. Distinguish unrun checks and physical-device performance from emulation. Do not publish, deploy or modify active pages without separate authorization.

[Prompt index](README.md)
