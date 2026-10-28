# Research Roadmap

## Mission

Build a source-linked library for creating and evaluating convincing AI-generated photographic imagery. Combine photographic fundamentals, computer-vision research, prompt design, and repeatable experiments. The goal is not to collect the longest prompts; it is to identify which choices improve which properties for which model and under what conditions.

## Workstream 0 — Evidence infrastructure
- [x] Create repository structure and evidence principles.
- [x] Add initial bibliography and research leads.
- [ ] Add stable source IDs, publication metadata, and review status.
- [ ] Add issue templates for source reviews, asset proposals, and experiment reports.
- [ ] Add a machine-readable source index if it becomes useful.

## Workstream 1 — Beauty, skin, and hair (highest priority)
- [ ] Define an observation vocabulary without assuming one ideal appearance.
- [ ] Document pore scale and visibility by region, framing, and resolution.
- [ ] Document sebum, specularity, redness, pigmentation, freckles, moles, fine hair, expression lines, and under-eye features.
- [ ] Study skin-tone rendering across illuminants and white-balance changes.
- [ ] Document hairline, individual strands, flyaways, curls, brows, lashes, lips, teeth, and makeup.
- [ ] Separate physical skin properties from lighting and post-processing.
- [ ] Build independent prompt modules and a failure catalog.
- [ ] Avoid treating blemishes or asymmetry as universal requirements for realism.

## Workstream 2 — Lighting
- [ ] Build profiles for window light, open shade, overcast sky, direct sun, flash, softbox, practical lights, and mixed lighting.
- [ ] Record source size, distance, direction, intensity, color, fill, bounce, shadow softness, and background relationship.
- [ ] Separate shadow-edge softness from shadow darkness.
- [ ] Study skin highlights and shadow shape together.
- [ ] Test flare and backlighting only under plausible source geometry.
- [ ] Distinguish prompt-only generation from explicit relighting tools.

## Workstream 3 — Camera and optics
- [ ] Create profiles for exact devices/lenses, not vague brand signatures.
- [ ] Record sensor format, physical focal length, equivalent focal length, aperture, focus distance, shutter, ISO, and processing when known.
- [ ] Explain focal length versus camera position and perspective.
- [ ] Build repeatable scenes for wide, normal, and portrait fields of view.
- [ ] Test focus, depth of field, bokeh, motion blur, and optical distortions.
- [ ] Label every profile as verified specification, visual target, or model-validated control.

## Workstream 4 — Computational photography and color
- [ ] Document smartphone HDR, multi-frame fusion, denoising, sharpening, tone mapping, local contrast, portrait segmentation, and JPEG/HEIF encoding.
- [ ] Separate sensor noise, chroma noise, film-like grain, sharpening halos, and compression.
- [ ] Document white balance, color response, highlight roll-off, shadow color, saturation, and skin-tone fidelity.
- [ ] Avoid adding noise, flare, or compression indiscriminately.

## Workstream 5 — Scene coherence
- [ ] Study anatomy, hand/object interactions, reflections, contact shadows, material response, perspective, background geometry, and composition.
- [ ] Build scenario recipes: casual selfie, friend-taken portrait, street candid, indoor lifestyle, beauty editorial, fashion, and product photo.
- [ ] Make defects conditional on plausible capture circumstances.

## Workstream 6 — Model-specific prompts
- [ ] Separate model-agnostic principles from provider-specific syntax.
- [ ] Record exact model/version, generation or editing mode, aspect ratio, quality, seed where available, and reference inputs.
- [ ] Keep a baseline for each task.
- [ ] Record failures, not only successful examples.

## Workstream 7 — Evaluation
- [ ] Use a fixed rubric.
- [ ] Compare normal display size and native resolution.
- [ ] Use blinded human evaluation when feasible.
- [ ] Keep provenance and rights for all benchmark images.
- [ ] Test repeatability across seeds and model versions.
- [ ] Report uncertainty; do not claim “indistinguishable” without a suitable controlled study.

## Milestone gates

**A — Reference library:** each priority asset has definitions, sources, confidence labels, and limitations.

**B — First benchmark:** baseline and at least three variants generated under controlled settings and evaluated with the same rubric.

**C — Reproducible assets:** another contributor can reproduce the setup and understand the supporting evidence.

**D — Public release:** links work, licenses are checked, unsupported claims are removed, and generated examples are labelled.

## Immediate next actions

1. Review the CHI 2025 photorealism paper, Generative Photography, LightLab, SynthLight, and skin/facial appearance papers in SOURCES.md.
2. Expand Skin Realism Pack into independent variables.
3. Define one portrait scenario and baseline.
4. Generate controlled variants using one selected model.
5. Record outputs before publishing “best prompt” claims.