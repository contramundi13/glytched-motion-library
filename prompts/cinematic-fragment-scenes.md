# Reusable prompt: Cinematic fragment scene sequence

**Status:** prompt only; build and deployment require separate authorization.

[Reference brief and evidence limits](../references/cinematic-fragment-scenes.md).

## Fill in the project contract

```yaml
brand: "Glytched" # adapt only with the intended brand's brief
purpose_and_audience: ""
scenes: [] # ordered image, dimensions, responsive sources, focal points, alt, approved headline/copy
asset_provenance: [] # license/usage rights or exact generation prompts
palette_and_type_tokens: {}
spacing_and_contrast_tokens: {}
interaction_mode: "" # select explicitly; source trigger is unverified
transition_timing_or_scroll_range: {}
fragment_layout_count_and_stagger: {}
depth_and_displacement_limits: {}
optional_pinning: false
mobile_treatment: "lightweight 2D or static stacked scenes"
reduced_motion_layout: "static scenes with all essential copy and CTA"
project_cta: {} # approved label and working URL
stack_and_integration_target: ""
asset_layer_and_runtime_budget: {}
```

## Implementation prompt, for a separately authorized build

> Create an original cinematic scene-transition experience for the supplied brand, audience and purpose. A suggested Glytched narrative is a cobalt landscape, an expressive abstract studio scene and a rain-lit futuristic street, ending in a clear project CTA. Use newly generated or licensed imagery and approved original copy; do not reproduce the reference's assets, branding or proprietary code. Record asset provenance and generation prompts. Do not invent business claims.
>
> Transition between scenes through a restrained stagger of rectangular strips or tiles that briefly smear, shift and reassemble, then settle into a coherent scene. Keep the approved headlines and supporting copy readable in semantic HTML, with stable contrast and logical reading order. Expose scene content/order, imagery, responsive focal points, palette, typography, timing, stagger, fragment count, displacement, depth and CTA as configuration. Do not add the recorded hand or highlighted pointer as page decoration.
>
> Begin with a lightweight 2D baseline: bounded clipped regions sharing responsive source images, with transform/opacity motion. Use WebGL only when meaningful depth and measured performance justify it; preserve the 2D/static fallback. Do not assume GSAP or Three.js is required or verified. The reel overlay names those tools, but actual stack and interaction trigger are unknown.
>
> Select and document the interaction model before implementation. A bounded pinned scroll timeline is a possible design, not observed source behavior. If chosen, preserve native wheel, touch and keyboard scrolling, support reversible progression and natural pin entry/exit, and avoid long scroll traps. On phones prefer a shorter unpinned treatment or static stacked scenes. If explicit scene controls are chosen, make them native keyboard-operable buttons with clear names and current-state feedback. If automatic playback is chosen, include a visible pause control and no autoplay audio.
>
> Keep menu, copy and the final project CTA reachable with keyboard and without animation. Use visible focus, adequate contrast through every transition state, comfortable touch targets and meaningful image alternatives. Hide decorative tile duplicates from assistive technology and never clone focusable controls into fragments. Avoid flashing or rapid high-contrast cuts. With reduced motion, no JavaScript, failed media or renderer failure, provide a static readable layout preserving every essential message and CTA.
>
> Use compressed responsive imagery with explicit dimensions. Prioritize the first scene and lazy-load later scenes near use; hold the current image until the next has decoded. Bound asset bytes, fragments and layers; measure loading, layout stability, memory and motion smoothness on representative desktop and phone sizes. Reduce mobile depth/displacement and preserve image focal points. Suspend unnecessary work offscreen/when hidden, remove listeners and dispose renderer resources on teardown.
>
> Inspect the existing reusable library before adding code and reuse appropriate navigation, CTA, layout and fallback patterns. Return editable source, parameter documentation, provenance, dependency rationale and integration instructions for the selected stack. Test the chosen trigger, native scroll behavior, keyboard/focus, menu/CTA destinations, mobile overflow/focal points, transition contrast, reduced motion, no-JS, media failure, loading and lifecycle cleanup. Report actual results and unrun checks distinctly. Do not publish, deploy, purchase services or change active sites without separate authorization.

## Evidence boundary

The parent research worker inspected approximately 13 seconds of actual playback. The [reference brief](../references/cinematic-fragment-scenes.md) records those attributed visual observations. The trackpad/pointer does not establish the trigger, the stack overlay does not establish implementation, and Facebook's AI-generated description is not independent evidence. The proposed three-scene Glytched narrative and its CTA are original design suggestions. This prompt has not been implemented or tested.

[Prompt index](README.md)
