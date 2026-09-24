# Rusty's Workshop

A fixed-front robot conveyor game: grab scrap, tap to bend it, throw it, and let protected items pass.

## Play

**[Open Rusty's Workshop](https://benzo42069.github.io/rustys-workshop/)**

The live static browser release is **v0.3.2 with the play-screen header cleanup**, including the corrected shoulder, hand, and wrist rig. All 15 items, controller mappings, and tap requirements are unchanged from the delivered v0.3.2 HTML.

The top-left title, tagline, version label, and controller hint are removed. Sound, pause, and help remain in their original top-right positions. Controller connection status is available inside Help. Every inline script and bundled asset is byte-identical to the original v0.3.2 release.

## Deployment status

GitHub Pages is live with HTTPS enforced, publishing from `main` at `/`. The current live response was verified as HTTP 200 and byte-identical to the tested header-cleanup file on September 24, 2026.

Current hosted SHA-256: `20f95da1350136152a8e202614e392dc06864984c4654cc8ec2ff33d14dc1eef`

Original v0.3.2 SHA-256: `b631320a33e1ffe3ddbb8ab566c160c2e0c353613486f4f24c883d710f2bcdc1`

The original deployment passed seven hosted-browser checks using normal HTTPS navigation in isolated headless Chrome on macOS: startup/artwork, grab and repeated-press bending, throw/recovery, pause/resume, protected-item refusal/pass, portrait control bounds, and absence of uncaught JavaScript/audio-decoding errors.

For the header cleanup, nine additional Chromium checks passed against the exact patched HTML: absence of branding; unchanged desktop, landscape, and portrait settings positions; controller status inside Help; grab/bend/throw; pause/resume/mute; simulated Xbox prompts; and no uncaught JavaScript errors. Current desktop and portrait renders were inspected. A separate isolated Chrome session on macOS opened the actual HTTPS site, completed game loading, and produced a live screenshot and rendered DOM confirming that the header is gone and the settings remain. These are browser-automation checks, not a physical-controller or child playtest.

## Publishing boundary

The playable `index.html`, empty `.nojekyll` marker, and this public README are the only release-repository files. Do not upload the development archive, original source sheets, private verification logs, credentials, or unrelated projects.

No custom Actions workflow, backend, analytics, paid runner, or new hosting subscription was added. Existing Actions policy and protections were left unchanged.

## Controls

Xbox: A grabs, repeated X presses bend, LB/RB throw, B lets an item pass, Menu pauses, Y opens help, and View toggles sound. Keyboard and touch alternatives are available in the game.

The browser build is not a Godot export. Physical Xbox/USB/Bluetooth, real iPhone/iPad/Safari, subjective audio, and child playtesting remain separate acceptance checks. Turn the phone sideways for a larger workshop.
