# Motion routing rubric (KHOSAN Time)
Prioritize the **information function** of each shot.

| Narrative beat | Suggested visual grammar | Engine default | When to escalate |
|---|---|---|---|
| First 0–2 second hook | Kinetic typography / controlled reveal / contrast | GSAP DOM/SVG | 3D title only if dimensional context matters |
| Breaking news | Editorial split panel, timestamp and lower third | HTML/CSS/GSAP | Three.js for geographic or spatial demonstrations |
| Evidence / quote | Document zoom, callout, highlight | SVG/GSAP | Canvas for substantial drawn diagram |
| Historical event / timeline | Museum timeline / paper scroll | GSAP/SVG | Three.js only for 3D reconstruction with a disclaimer |
| Data / statistic | KPI count-up, bar chart, causal arrows | SVG/GSAP/Canvas | 3D only if it improves interpretation |
| People and social emotion | Character theater / editorial card | HTML/CSS/GSAP | Separate validated GLB character if actual 3D acting needed |
| How it works / science | Isometric systems, network nodes, nested diagrams | SVG/Canvas | Three.js for actual spatial geometry |
| Spiritual / fortune | restrained gold particles, depth layers, silhouettes | Canvas/GSAP | Three.js for true celestial scene |
| What-if scenario | future timeline and scene morphs | GSAP/Canvas | Three.js when location/camera is key |
| Closing CTA | minimalist logo lockup + readable question | CSS/GSAP | rarely needs 3D |

## Score candidates from 0 to 5
total = 0.35*semantic + 0.25*readability + 0.20*feasibility + 0.10*brand + 0.10*efficiency.
Disqualify if source unavailable for required copy, rights unclear for commercial reuse, or essential 9:16 typography fails. When no approved template fits: custom CSS/GSAP is a valid choice.

## Operating modes
- `reference`: catalog/preview only; describe concept, do not copy implementation.
- `inspect`: fetch package/repo, read instructions/license, classify stack, isolate reusable techniques.
- `implement`: create new original scene based on suitable patterns, or adapt licensed source with attribution.
- `render`: validate and export to user requested format.

## Scene motion-plan contract
```json
{
  "scene_id":"S01",
  "role":"hook",
  "duration_mode":"audio-driven",
  "engine":"gsap-dom",
  "template_reference":"motiongit:385712",
  "template_state":"reference-only",
  "visual_pattern":"kinetic-type-reveal",
  "camera":"2d-push",
  "assets":["hero_image"],
  "fallback":"css-fade-push",
  "reason":"readable 2-second reveal",
  "review_required":true
}
```

## Browser video QA
Type-check/lint JS; verify fonts including Thai line breaking; render sampled timestamps 0, 0.5, 2.0, every scene midpoint and last second. Confirm frame stepping/seek if offline export. Verify canvas origin clean over HTTP; 30fps default unless job requests 60fps; resync to measured audio, no hardcoded 180s timeline. Use TTS, music and visual timing consistently in preview/export.
