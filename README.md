# Wireform Jig

Procedural wireframe forms + generative analogue music, in one self-contained HTML file.

## What it makes
- Parametric 3D wireframe surfaces (sphere, torus, torus knot, hourglass/hyperboloid, Möbius, wavy tube, spiky star, saddle, blob, diamond, wave sheet, Lissajous ribbon) drawn as pure lines on black — the family in your reference images.
- Morphing between two forms, twist / pinch / bumps / wave / spikes deformation, 5 line styles (wireframe, parallel, rings, dots, fan), palettes, warped grid background.
- Full motion: turntable spin, tumble, roll, wobble, breathing, line-march dashes, morph oscillation. Drag the canvas to orbit manually.
- Generative analogue music: the form *is* the score. Each sequencer step samples a vertex of the current shape — X → scale degree, depth → octave, twist → filter, spin → swing/LFO, breathing → echo. Synthesised live with WebAudio (saw/square plucks, bass, kick/hat/snare, pad, resonant low-pass, tape saturation + hiss + wow/flutter, feedback delay, generated reverb). No samples.

## Reference
Your 5 screenshots: white line-forms on black — parallel-line fans ("Show Comparisons / Causality / Multivariate Data…"), warped grid with rings/spheres, wireframe hourglasses & tori, and lat/long spheres. Presets are named after the first image's captions plus the shapes in the others.

## How to open
Double-click `index.html` — no server, no install, no internet needed. (Sound needs a user gesture: press ▶ Start sound.)

## How to use
1. Press **Shuffle** (Space) ~20 times.
2. **★ Keep** (F) the ones you like — they collect in a strip under the preview (saved in your browser). Click one to restore it.
3. **Lock** groups you want to protect, then tweak by hand. **Off** hides a group without losing its settings. Each group has its own Shuffle.
4. Press **▶ Start sound** (P) and change the shape while it plays — the music follows the form. Turn "Form → music strength" up for a tighter link.
5. Export: **PNG** (2×), **Copy link** (encodes all settings in the URL), **Record audio** (.webm), **Record 6s video** (.webm). Format picker: 1:1, 16:9, 9:16, 4:5.

## Limitations
- Canvas 2D custom projection (no WebGL/Three.js) so it works offline from disk — resolution is capped for smooth 60fps; very high line counts may slow older machines.
- Audio recording is WebM via MediaRecorder (browser-dependent); video export is a 6-second WebM clip, not MP4.
- I couldn't run a browser in the build environment to click-test it — JS syntax was checked with Node. If anything looks off, tell me what you see and I'll fix it in the same file.
