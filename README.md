# Rusty's Workshop

A fixed-front robot conveyor game: grab scrap, tap to bend it, throw it, and let protected items pass.

## Play

**[Open Rusty's Workshop](https://benzo42069.github.io/rustys-workshop/)**

The live static browser release is **v0.3.2**, including the corrected shoulder, hand, and wrist rig. All 15 items, controller mappings, and tap requirements are unchanged from the delivered v0.3.2 HTML.

## Deployment status

GitHub Pages is live with HTTPS enforced, publishing from `main` at `/`. The live response was verified as HTTP 200 and byte-identical to the original release on September 24, 2026.

Release SHA-256: `b631320a33e1ffe3ddbb8ab566c160c2e0c353613486f4f24c883d710f2bcdc1`

Seven hosted-browser checks passed using normal HTTPS navigation in isolated headless Chrome on macOS: startup/artwork, grab and repeated-press bending, throw/recovery, pause/resume, protected-item refusal/pass, portrait control bounds, and absence of uncaught JavaScript/audio-decoding errors. The rendered ready, bent, and portrait views were inspected. This was browser automation, not a physical-controller or child playtest.

## Publishing boundary

The playable `index.html`, empty `.nojekyll` marker, and this public README are the only release-repository files. Do not upload the development archive, original source sheets, private verification logs, credentials, or unrelated projects.

No custom Actions workflow, backend, analytics, paid runner, or new hosting subscription was added. Existing Actions policy and protections were left unchanged.

## Controls

Xbox: A grabs, repeated X presses bend, LB/RB throw, B lets an item pass, Menu pauses, Y shows controls, and View toggles sound. Keyboard and touch alternatives are available in the game.

The browser build is not a Godot export. Physical Xbox/USB/Bluetooth, real iPhone/iPad/Safari, subjective audio, and child playtesting remain separate acceptance checks. Turn the phone sideways for a larger workshop.
