# Glytched particle study · 1.0.0

An original reusable Canvas 2D component and isolated demo. Particles assemble, hold, release and drift on an 11-second base cycle. Cyan/magenta palette follows the supplied Glytched identity. **The text is a typography study, not an official logo**: available approved assets included the metallic hero image but no standalone mark. No hero image is recreated or used as a substitute logo.

## Run and deployable scope

From repository root, run `python3 -m http.server 8790` and open `http://localhost:8790/components/glytched-particles/`. Runtime files are `index.html`, `demo.css`, `particles.js`, `demo.js`; all URLs are relative. No build, fonts, assets, frameworks or network requests are required beyond these four files. QA and documentation are not runtime requirements.

No live route for this library was verified or used. The separate `glytched-demos` repository's prior Veyra authorization does not establish a particle deployment route. Smallest hosting step: authorize an isolated destination for these four runtime files through the existing Glytched staging pipeline. No deployment, Plesk change or production-page change is included. GitHub source and screenshots are review artifacts, not a live interactive host.

## Reuse and configuration

Include a container with `data-particles`, a decorative `canvas` (`aria-hidden="true"`) and a static `.fallback` element. Add a `.phase` label optionally. Load `particles.js`, then instantiate:

```js
const effect = new GlytchedParticles(root, {
  colors: ['#37e5f5', '#f476d6'],
  density: 800,
  speed: 1,
  shape: 'type', // 'type' = GLYTCHED typography; 'orbit' = abstract form
  pointerStrength: 8
});
effect.configure({ shape: 'orbit', density: 450, speed: 0.65 });
effect.pause(); effect.play(); effect.replay();
// Before removing the component from a dynamically mounted page:
effect.destroy();
```

Density caps: 420 below 650 CSS pixels; 1,400 otherwise. Pixel ratio caps: 1 on smaller containers, 1.5 otherwise. Rendering targets about 30 fps; this is a scheduling limit, not a measured mobile performance claim. Speed clamps to 0.3–2; pointer displacement clamps to 0–12 pixels. Pointer response is disabled for touch/coarse input, with no gesture interception. Options should be supplied by trusted application configuration.

The component emits `particle-state` after control/preference changes with paused/reduced/count information. `demo.js` provides UI wiring; do not copy its global demo instance into a multi-instance integration. Namespace/scope `demo.css` before embedding into an existing WordPress/Elementor page: it is standalone page styling. Keep real headings, explanations, controls and CTA in HTML outside the decorative canvas. A real mark requires a separately approved source asset and sampler; do not silently replace the typography with an invented logo.

## Motion and fallbacks

Reduced-motion preference draws a fully assembled static form and disables play/replay in the demo. No-JS or unavailable Canvas retains the HTML typography fallback and explanatory content. User pause stops frame scheduling; offscreen and hidden-document states suspend it. Resize re-samples bounded targets. Destroy cancels frames, removes registered listeners, disconnects observers and restores the fallback. No pointer interaction is required to understand the content.

The CTA navigates within the demo. There are no transactions, lead collection or production links. Cyan/magenta motion stays moderate with no flashing effects. Typography/system fonts are not claimed as official Glytched font assets.

## Provenance and rights

Inspiration: [Code XR reel](https://www.facebook.com/reel/1611869037184551), [submitted share](https://www.facebook.com/share/r/19yq7r2iUZ/). Parent cloud-browser observations: bright particles form a heart and round cloud, then scatter on black. Pointer interaction and React/CSS stack claims were not verified. This component uses newly written Canvas 2D code and a different typography/orbit concept; no source code, source media or reel assets were copied. No generated visual assets were needed. Original component code is provided under [MIT](LICENSE.txt); this does not grant rights in the Glytched brand.

## QA

Run `node components/glytched-particles/qa/check.cjs` from repository root with the local server on port 8790. Requires Playwright, Chromium at `/usr/bin/chromium`, and axe-core at `/tmp/glytched-particle-qa/node_modules/axe-core/axe.min.js` (adjust the test path for another setup). [Results](qa/results.json), [desktop](qa/desktop.png), [mobile](qa/mobile.png), [reduced motion](qa/reduced-motion.png).

Checks cover four responsive widths, automated accessibility, phase progression, pause/replay, configuration, keyboard/CTA access, reduced motion, offscreen resumption, simulated hidden-document state, no-JS, touch handling and cleanup. Screenshots are reviewed separately from automated assertions. No physical-device performance, Safari/Firefox, screen-reader listening or hosted-route checks are claimed.
