# Literature Notes: What the Research Suggests

This is an initial reading map based on available abstracts, project pages, and publication records. It is not a substitute for a full paper review. Mark each note as provisional until methods, experiments, and limitations have been inspected.

## 1. Characterizing Photorealism and Artifacts in Diffusion Model-Generated Images — CHI 2025

**Source:** https://mucollective.co/files/2025-photorealism.pdf

### Why it matters
The work studies how people judge whether images are AI-generated or real, and catalogs artifacts. Its methodology includes curated real photographs, thousands of generated candidates, and a large crowdsourced evaluation. The authors discuss scene complexity, artifact categories, and the selection of images that are not immediately identified as generated.

### What we should take from it
- Perceived realism is an evaluation problem, not just a prompt-writing problem.
- Image selection matters: showing only the best outputs can overstate performance.
- Artifact taxonomy is useful for a structured failure catalog.
- Scene complexity and context can affect detection.

### What not to conclude
Do not assume one set of artifacts applies to every model or that a detector/human judgment score is a universal measure of realism. Review the full methods, image sampling, participants, and limitations before making quantitative claims.

### Repository actions
- Use a fixed rubric.
- Save failed outputs as well as successful ones.
- Evaluate at intended display size and native resolution.
- Separate perceived realism from attractiveness and technical quality.

## 2. Generative Photography — CVPR 2025

**Source:** https://generative-photography.github.io/project/

### Why it matters
The project targets scene-consistent control over camera parameters. The paper page describes limitations in current text-to-image systems when users request different camera settings, and proposes a framework to improve consistency.

### What we should take from it
- A textual camera specification is not equivalent to physically grounded camera control.
- Lens, field of view, blur, shutter, and color temperature can interact with the scene.
- A good benchmark should test whether the scene remains consistent as a parameter changes.

### Repository actions
Compare focal-length-only prompts with a fuller camera scenario. Rate framing, perspective, and focus behavior independently. Do not claim the model used a real camera merely because the prompt names one.

## 3. PreciseCam — CVPR 2025

**Source:** https://research.adobe.com/publication/precisecam-precise-camera-control-for-text-to-image-generation/

### Why it matters
The work investigates camera control using a parameterized method and a dataset with camera parameters, rather than relying exclusively on natural-language descriptions.

### Repository actions
Use this as evidence that prompt engineering has limits. If exact camera behavior is a hard requirement, consider reference images, camera-conditioned models, or editing pipelines in addition to text prompts.

## 4. LightLab — SIGGRAPH 2025

**Source:** https://research.google/pubs/lightlab-controlling-light-sources-in-images-with-diffusion-models/

### Why it matters
LightLab explores fine-grained control of light sources and ambient illumination, including training with real RAW photograph pairs and synthetic data.

### What we should take from it
- Lighting is a structured physical variable.
- Source intensity and color can be treated as separate controls.
- Prompt-only descriptions and explicit relighting systems are different capability classes.

### Repository actions
Build a light-profile schema that records source size, direction, intensity, color, fill, shadow behavior, and background relation. Keep the actual model/task mode in every experiment.

## 5. SynthLight — CVPR 2025

**Source:** https://vrroom.github.io/synthlight/

### Why it matters
The project treats portrait relighting as re-rendering and shows how face illumination changes affect cast shadows and specular highlights.

### Repository actions
Evaluate light direction, shadow shape, neck shadows, and skin highlights together. A face with detailed pores but inconsistent lighting should not receive a high realism score.

## 6. Controllable Biophysical Human Faces — 2025

**Source:** https://doi.org/10.1111/cgf.70170

### Why it matters
The work links facial appearance with biophysical attributes such as melanin and blood content and emphasizes relationships between facial geometry and appearance.

### Repository actions
Treat skin as a material whose appearance depends on anatomy, illumination, and optical behavior. Avoid treating pores, redness, and specular highlights as independent stickers.

## 7. Physically Based Facial Texture Generation in the Wild — 2025

**Source:** https://pubmed.ncbi.nlm.nih.gov/40531629/

### Why it matters
The title and publication record indicate a physically based approach to facial texture generation. Full paper review is required before extracting more specific claims.

### Repository actions
Read the full text when available and record method, dataset, and limitations before using it to justify a prompt recipe.

## 8. TrueSkin — 2025 preprint

**Source:** https://arxiv.org/abs/2509.10980

### Why it matters
The preprint reports challenges in skin-tone recognition and generation across lighting and camera conditions.

### Repository actions
Test skin-tone fidelity across diverse complexions and illumination conditions. Do not use one skin-tone reference as the sole benchmark.

## 9. Midjourney official prompting guidance

**Source:** https://docs.midjourney.com/hc/en-us/articles/32023408776205-Prompt-Basics

The official guide recommends clear, specific descriptions and warns that overly long lists can confuse results. This is an important counterweight to community advice that longer prompts always improve realism.

### Repository actions
Test concise, coherent prompts against longer prompts. Measure outcome quality rather than assuming prompt length is a proxy for control.

## 10. Apple computational photography documentation

**Sources:**
- https://support.apple.com/en-lamr/guide/iphone/iph2cafe2ebc/ios
- https://developer.apple.com/documentation/avfoundation/capturing-photos-in-raw-and-apple-proraw-formats

Apple documents HDR multi-exposure blending and computational processing in standard capture pipelines, with differences between processed formats and RAW/ProRAW workflows.

### Repository actions
A smartphone signature should include computational processing, not only lens and aperture. Do not infer an exact phone model from an image's visual appearance alone.

## Cross-cutting conclusions

1. Prompting is only one control surface; reference images and dedicated tools may be more effective for some parameters.
2. Physical coherence across the whole image matters more than isolated “realism” adjectives.
3. The same prompt can behave differently across models and versions.
4. Source provenance and reproducibility are essential.
5. Every recommendation should carry a status and limitations.
