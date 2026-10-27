# KHOSAN Production Quality Gate — Motion-Based News Video

## Origin: user production feedback (Oct 2026)
A six-video first render failed editorial quality despite technically valid MP4 output. Causes: arbitrary source-image rotation, apparent still-frame freezes, full-script captions that overflowed portrait safe zones, B-roll inserted by timestamp rather than narrative relevance, and treating a template catalog as a ready-to-run renderer.

## Catalog caveat: "3D Book · A Personal Story" (#3)
In the MotionGit `CATALOG.en.md` it is **16:9 only (1920x1080, 60 FPS), with demo video and download "coming soon"**. Its source template was not obtained. Never claim to have installed or rendered from this proprietary/third-party template. If user requests portrait 9:16, deliver an original 3D photobook-inspired scene, or wait until a legally reusable actual package exists. Preserve attribution and asset/license status.

## Non-negotiable checks before declaring "done"
1. **Editorial matching** — Index every available image/video; create contact sheets; inspect content; hand-pick image order per narrative angle. Reject unrelated imagery and graphics that depict allegations as proven facts. Never shuffle 18 images arbitrarily for all six edits.
2. **Motion** — Video must visibly change within each shot: slow parallax / dolly on photographs, actual source footage cutaways, and intentional transitions. Test frame differences in each chapter to detect frozen loops.
3. **Mobile layout** — Canvas 1080x1920; lock safe zones. Caption box inside approximately Y=1250–1450; no more than two lines and no clipping. Keep headline off faces/documentary images.
4. **Thai captions** — Divide by Thai grapheme clusters, aim <=28–30 clusters per line; preserve combining marks; do not put complete long paragraphs in a single caption. Caption intervals must be accurate to spoken WAV; proportional text-length timing is only *approximate* and **requires audible spot checks** or ASR/forced alignment before final publication.
5. **Audio** — Do not stretch/trim source voice to match arbitrary storyboard. Suppress original B-roll audio unless specifically requested. Verify no clipped endings or gaps.
6. **QA artifacts** — Write contact-sheet JPG for each finished video, FFprobe metadata report, motion-difference samples, source asset manifest, and a list of editorial uncertainties. A successful FFmpeg exit does NOT constitute visual QA.
7. **Legal and truthfulness** — Separate public allegations, statements, and independent facts, especially in family or financial disputes. Avoid images of children or sensational third-party quote posters when not verified; review rights before social publication.
8. **Keep local outputs local** — Don't upload identifiable/copyrighted assets, videos, or private source WAVs to GitHub just to store build instructions.

## Preferred production loop
Assets -> contact sheet -> editorial shortlist -> scene-to-image mapping -> 3D book/storyboard concept -> motion-preview of 10–20 seconds -> QA visually and audibly -> produce requested variants -> contact sheets + technical QC -> approval -> publish.

## Example local source reference
Original (non-MotionGit) book-style renderer created for a 9:16 test uses 3.5s animated paper-card holds, 0.5s original perspective page flips, video inset B-roll, safe-zone Thai ASS captions, six separate story angles, and FFprobe/contact-sheet checks. Do not equate original homage with use of unavailable MotionGit template #3.
