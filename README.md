# Rusty's Workshop

A fixed-front robot conveyor game: grab scrap, tap to bend it, throw it, and let protected items pass.

This repository is reserved for the static browser release. The current upload target is **v0.3.2**, including the corrected shoulder, hand, and wrist rig.

## Deployment status

The repository is initialized. The game upload and GitHub Pages activation are pending; this README is not a playable deployment.

## Publishing boundary

Only the self-contained playable `index.html` and an empty `.nojekyll` marker belong in the publishing root. Do not upload the development archive, original source sheets, verification logs, credentials, or unrelated projects.

GitHub Pages should publish from `main` at `/`. No custom Actions workflow, backend, analytics, or paid runner is required.

## Controls

Xbox: A grabs, repeated X presses bend, LB/RB throw, B lets an item pass, Menu pauses, Y shows controls, and View toggles sound. Keyboard and touch alternatives are available in the game.

The browser build is not a Godot export. Physical-controller and actual-device qualification remain separate from automated browser tests.
