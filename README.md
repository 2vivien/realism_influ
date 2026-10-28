# Realism Influ — Photographic Reality Research Library

> A research-driven, evidence-tracked library for building more convincing AI-generated photographic images.

**Realism Influ** investigates how human appearance, skin and hair, lighting, camera geometry, optics, color science, image processing, composition, and scene coherence contribute to perceived photographic realism.

This repository is a curated knowledge base and experimental notebook—not a promise that any prompt can make synthetic imagery indistinguishable from a real photograph.

## Start here

- [Research roadmap](docs/ROADMAP.md)
- [Research methodology](docs/research/METHODOLOGY.md)
- [Literature notes](docs/research/LITERATURE-NOTES.md)
- [Community prompt analysis](docs/research/COMMUNITY-PROMPT-ANALYSIS.md)
- [Source review template](docs/research/SOURCE-REVIEW-TEMPLATE.md)
- [Source registry](SOURCES.md)
- [Skin Realism Pack](assets/skin-realism/README.md)
- [Hair & Facial Beauty Pack](assets/hair-beauty/README.md)
- [Lighting library](assets/lighting/README.md)
- [Camera profiles](assets/camera-profiles/README.md)
- [Smartphone computational photography](assets/camera-profiles/SMARTPHONE-COMPUTATIONAL-PHOTOGRAPHY.md)
- [Color science and computational photography](assets/color-processing/README.md)
- [Capture artifact catalog](assets/capture-artifacts/README.md)
- [Scene coherence and composition](assets/scene-coherence/README.md)
- [Master prompt](prompts/MASTER-PROMPT.md)
- [Reusable prompt modules](prompts/MODULE-CATALOG.md)
- [Photographic scenario cards](prompts/SCENARIO-CARDS.md)
- [Experiment protocol](experiments/EXPERIMENT-PROTOCOL.md)
- [Planned experiment log](experiments/EXPERIMENT-LOG.md)
- [Realism evaluation rubric](evaluation/REALISM-RUBRIC.md)
- [Data and image rights](docs/research/DATA-AND-RIGHTS.md)
- [Contribution guide](CONTRIBUTING.md)

## Principles

1. **Evidence before claims.** Separate peer-reviewed findings, manufacturer specifications, practitioner guidance, and hypotheses.
2. **Record provenance.** Every source should have a URL, publication metadata when available, access date, relevance, and confidence.
3. **Test prompt components.** Change one major variable at a time when possible; record model, version, settings, seed, reference inputs, and outcomes.
4. **Physical coherence beats adjective stacking.** Skin, lighting, lens behavior, perspective, and processing must agree with the same capture scenario.
5. **No fake camera certainty.** A prompt saying “85 mm f/2” does not guarantee that a model simulates a real lens. Camera metadata is a target description unless independently verified.
6. **No universal realism recipe.** Model behavior varies. Results must be reported per model and version.
7. **Respect people and image rights.** Use licensed, consented, public-domain, or otherwise authorized reference material. Do not use the library to impersonate a real person or misrepresent synthetic imagery as documentary evidence.

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

This repository starts as a structured research program. Assets marked **hypothesis** or **untested** are not validated recipes. **Tested** means an experiment was run and documented; **replicated** means the finding was repeated under specified conditions. Neither label implies universal effectiveness.

## Citation and reuse

Read each source's license and terms before redistributing images, datasets, code, or full text. Link to sources and summarize findings in original wording rather than mirroring copyrighted content. See [Sources](SOURCES.md) and [Data and image rights](docs/research/DATA-AND-RIGHTS.md).

## Language

Main documentation is in English for international accessibility. French notes and translations are welcome when they add value.
