---
name: khosan-motion-director
description: "Automatically choose suitable MotionGit motion templates and a JavaScript animation engine (HTML/CSS/GSAP, Vite, Three.js) for KHOSAN Time content. Use for animated headlines, cinematic news, documentary explainers, data visuals, kinetic typography, 3D stages, and scripted videos. Inspect MotionGit catalog and source package before adaptation."
---
# KHOSAN Motion Director — Agent Skill v1.0
## Goal
Turn a verified KHOSAN Time brief into a purposeful, reusable motion plan and working browser-based animation. Select techniques **by scene**, not one flashy effect for an entire video. The catalog is a *reference/index*, not a runtime SDK or proof that source has been downloaded.

## Activate on
"animate", "motion", "video explainer", "kinetic type", "three.js", "Vite", "JS animation", "storyboard to HTML", "KHOSAN video", "animated dashboard", "Walter NPC stage".

## Mandatory workflow
1. Read project Brand Context, AGENT.md, storyboard and user constraints. Source validation precedes motion for news.
2. Read `references/motion-router.md`, `references/template-shortlist.md`, and `references/editorial-video-qa.md`; check the up-to-date source catalog `CATALOG.en.md` and `catalog.json` in this repository.
3. For each scene identify: semantic intent (hook/evidence/timeline/data/emotion/CTA), portrait or landscape, visual assets, Thai text length, 2D/3D demands, delivery and render environment.
4. Rank candidate motion families by: semantic fit 35%, legibility 25%, feasibility 20%, brand match 10%, cost/performance 10%. Prefer simple animation when a complex engine adds no explanatory value.
5. Mark all chosen templates `reference-only` until the actual template code/package and license have been checked. For the selected source, inspect its linked GitHub repo, exact commit, asset requirements, license, and .motion instructions before using code. Never assume catalog listing contains source.
6. Output `motion-plan.json`, `storyboard.json`, `layers.json`, design tokens, source attribution/rights manifest, a scene-specific implementation plan, and preview-ready code. Do not treat a design proposal as tested code.
7. Use review gate: storyboard/motion plan first; then implement; then preview/inspect sampled frames and timing; render only when requested/approved.
8. Log source URL, commit/ref, license status, integration decisions and missing assets. Do not declare finished solely after successful FFmpeg render: inspect actual frames, scene motion, Thai subtitle safe zones, and editorial source-image relevance; produce contact-sheet QA.\n9. If a template listing says 'coming soon' or is demo-only (notably MotionGit 3D Book #3), say so and use an original, clearly differentiated implementation only if requested. No fabricated rights or download capabilities.

## Renderer/engine selection
- **CSS/WAAPI**: simple fades, slides, lower thirds, Ken Burns; no build required.
- **GSAP + DOM/SVG**: kinetic headlines, precise scene timelines, infographic transitions, choreography.
- **Canvas 2D**: composited diagrams/particles where native graphics simplify output; verify origin-clean.
- **Vite + vanilla TypeScript/JavaScript**: multi-scene modular project or shared components. Vite is a **build tool**, not an animation engine.
- **Three.js (often via Vite)**: genuine 3D camera, depth, objects and mapped scenes. Use for select beats, not ordinary statistics or Thai subtitles.
- **Existing KHOSAN HyperFrames**: only if requested or already embedded; follow its own composition rules. Do not confuse it with the user's preferred standalone studio.
- **Blender character rigs**: keep facial/body rigging upstream. Three.js can consume validated GLB/GLTF and animation clips but cannot repair poor weight painting or facial shape keys.

## KHOSAN implementation defaults
- User's current delivery preference: **standalone Edge browser app via local Python server**, with export workflow to WebM then FFmpeg MP4; no required `npm run dev` or HyperFrames Studio. Vite is allowed at **authoring/build time**, but ship built static dist + local server launcher for delivery.
- 9:16 1080x1920 and 16:9 1920x1080. Mobile-first text. Respect KHOSAN established per-project wireframe: portrait hero object ~Y520–880, headline ~Y850–1120, subtitles ~Y1180–1380, CTA ~Y1480–1630, avoid essential text below Y1650. Make these configurable (other scene styles may need different layouts).
- Logo: use supplied `logoKST.png` if present; don't hardcode a missing image, don't cover faces or text.
- Audio narration default when requested: `th-TH-PremwadeeNeural` via edge-tts, never silently replace voice. Use ffprobe-measured timing and resync scene start/duration; never trim narration to old estimates.
- Use `layers.json` for replaceable assets and placeholder images that render visibly if missing. Background motion must serve the narrative.
- Guard canvas export via local HTTP origin, not file://. Check console syntax, missing images, font loading, overlap, captions, safe zone, SFX/BGM levels, seek/replay determinism and frame timing.

## Minimum agent output (per task)
1. Concept + hook + headline + short CTA anchored to verified content.
2. Scene router table: chosen pattern, reason, source template reference ID/link, engine, complexity and fallback.
3. JSON files and implementation. When only asked to plan, stop at plan.
4. Test report including what was actually executed vs not executed.

## Hard constraints
No one-click copying of unreviewed third-party projects. No assumption that the source templates use Vite, GSAP or Three.js. No unverified factual visuals, misleading reconstructions, or claim of verified license without inspecting it. No arbitrary looping or frame-time randomness in exported scenes.
