# Realism Influ — Photographic Reality Research Library

> A research-driven, evidence-tracked library for building more convincing AI-generated photographic images.

**Realism Influ** investigates how human appearance, skin and hair, lighting, camera geometry, optics, color science, image processing, composition, and scene coherence contribute to perceived photographic realism.

This repository is a curated knowledge base and experimental notebook—not a promise that any prompt can make synthetic imagery indistinguishable from a real photograph.

## Start here

- [Research roadmap](docs/ROADMAP.md)
- [Research methodology](docs/research/METHODOLOGY.md)
- [Source registry](SOURCES.md)
- [Skin Realism Pack](assets/skin-realism/README.md)
- [Lighting library](assets/lighting/README.md)
- [Camera profiles](assets/camera-profiles/README.md)
- [Color science and image processing](assets/color-processing/README.md)
- [Prompt engineering framework](prompts/MASTER-PROMPT.md)
- [Experiment protocol](experiments/EXPERIMENT-PROTOCOL.md)
- [Evaluation rubric](evaluation/REALISM-RUBRIC.md)
- [Contribution guide](CONTRIBUTING.md)

## Principles

1. **Evidence before claims.** Separate peer-reviewed findings, manufacturer specifications, practitioner guidance, and hypotheses.
2. **Record provenance.** Every source has a URL, publication metadata when available, access date, relevance, and confidence.
3. **Test prompt components.** Change one major variable at a time when possible; record model, version, settings, seed, reference inputs, and outcomes.
4. **Physical coherence beats adjective stacking.** Skin, lighting, lens behavior, perspective, and processing must agree with the same capture scenario.
5. **No fake camera certainty.** A prompt saying “85 mm f/2” does not guarantee that a model simulates a real lens. Camera metadata is a target description unless independently verified.
6. **No universal “realism recipe.”** Model behavior varies. Results must be reported per model and version.
7. **Respect people and image rights.** Use licensed, consented, public-domain, or otherwise authorized reference material. Do not use the library to impersonate a real person or misrepresent synthetic images as documentary evidence.

## Knowledge architecture

| Area | What it covers |
|---|---|
| Skin and facial appearance | Pore scale, sebum, redness, freckles, moles, fine hair, expression lines, subsurface scattering |
| Hair and beauty | Hairline, flyaways, strands, curls, brows, lashes, lips, makeup and facial expression |
| Lighting | Source size, direction, softness, intensity, color, bounce, shadows, specular response, mixed lighting |
| Camera and optics | Sensor format, equivalent focal length, subject distance, aperture, shutter, focus, depth of field, bokeh, distortion |
| Computational photography | HDR, denoising, sharpening, multi-frame fusion, portrait segmentation and tone mapping |
| Color and rendering | White balance, color response, skin-tone fidelity, tone curves, highlight roll-off, saturation and local contrast |
| Capture artifacts | Noise, motion blur, JPEG compression, chromatic aberration, flare, vignetting and dust when contextually plausible |
| Scene coherence | Anatomy, reflections, contact shadows, geometry, materials, environment and composition |
| Evaluation | Human preference, artifact taxonomy, repeatability, uncertainty and model-specific limitations |

## Status

This repository starts as a structured research program. Assets marked **hypothesis** or **untested** are not validated recipes. A status of **tested** means an experiment was run and documented; **replicated** means the finding was repeated under specified conditions. These labels do not imply universal effectiveness.

## Citation and reuse

Read each source's license and terms before redistributing images, datasets, code, or full text. The repository should link to sources and summarize findings in original wording rather than mirror copyrighted material. See [Sources](SOURCES.md) and [Data and image rights](docs/research/DATA-AND-RIGHTS.md).

## Language

The main documentation is in English to make the research accessible internationally. French notes and translations are welcome when they add value.
