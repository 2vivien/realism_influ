# Research Source Registry

This is a curated starting bibliography, not a claim that every available source has already been read. Entries are discovery and review targets. Verify the current version, methods, license, and publication status before relying on a claim. Accessed 2026-10-28.

## Peer-reviewed research and research projects

### Camera control and image formation

1. **Generative Photography: Scene-Consistent Camera Control for Realistic Text-to-Image Synthesis — CVPR 2025.**
   - Paper: https://openaccess.thecvf.com/content/CVPR2025/html/Yuan_Generative_Photography_Scene-Consistent_Camera_Control_for_Realistic_Text-to-Image_Synthesis_CVPR_2025_paper.html
   - Project: https://generative-photography.github.io/project/
   - Why it matters: tests whether image generators maintain scene consistency when camera parameters such as focal length, bokeh, shutter speed, and color temperature are changed.
   - Implication: camera words in a prompt are not guaranteed to act as physically accurate controls.

2. **PreciseCam: Precise Camera Control for Text-to-Image Generation — CVPR 2025.**
   - Research page: https://research.adobe.com/publication/precisecam-precise-camera-control-for-text-to-image-generation/
   - Why it matters: investigates camera control beyond prompt-only instructions and introduces a dataset with camera parameters.

3. **CamEdit: Continuous Camera Parameter Control for Photorealistic Image Editing — NeurIPS 2025.**
   - Paper: https://papers.nips.cc/paper_files/paper/2025/hash/a60567166d738f4c43e563fdf8a2afe4-Abstract-Conference.html
   - Why it matters: studies continuous control over camera-like parameters such as aperture and shutter speed in image editing.

### Lighting and relighting

4. **LightLab: Controlling Light Sources in Images with Diffusion Models — SIGGRAPH 2025.**
   - Research page: https://research.google/pubs/lightlab-controlling-light-sources-in-images-with-diffusion-models/
   - Why it matters: studies parameterized control over light sources and ambient illumination, using real RAW photograph pairs and synthetic data.

5. **SynthLight: Portrait Relighting with Diffusion Model by Learning to Re-render Synthetic Faces — CVPR 2025.**
   - Project: https://vrroom.github.io/synthlight/
   - Why it matters: portrait relighting, cast shadows, and natural specular highlights on skin.

6. **Training-free diffusion for controlling illumination conditions in images — Computer Vision and Image Understanding, 2025.**
   - Article: https://www.sciencedirect.com/science/article/pii/S1077314225001730
   - DOI: https://doi.org/10.1016/j.cviu.2025.104450
   - Why it matters: physically guided lighting changes, cast shadows, soft shadows, and inter-reflections.

### Skin, faces, and tone fidelity

7. **Controllable Biophysical Human Faces — Computer Graphics Forum, 2025.**
   - DOI and publisher: https://doi.org/10.1111/cgf.70170
   - Why it matters: models relationships between facial geometry and biophysical attributes, including melanin and blood content.

8. **Physically Based Facial Texture Generation in the Wild — IEEE TPAMI, 2025.**
   - Publication record: https://pubmed.ncbi.nlm.nih.gov/40531629/
   - DOI: https://doi.org/10.1109/TPAMI.2025.3580953
   - Why it matters: physically based facial texture generation.

9. **TrueSkin: Towards Fair and Accurate Skin Tone Recognition and Generation — 2025 preprint.**
   - arXiv: https://arxiv.org/abs/2509.10980
   - Why it matters: skin-tone fidelity under different lighting and capture conditions, including reported limitations for intermediate skin tones.
   - Caution: preprint evidence should be treated as preliminary until independently assessed.

### Human perception and artifacts

10. **Characterizing Photorealism and Artifacts in Diffusion Model-Generated Images — CHI 2025.**
    - Paper: https://mucollective.co/files/2025-photorealism.pdf
    - Why it matters: human judgments of generated versus real images, artifact categories, scene complexity, and controlled image selection.

11. **RealGen: Photorealistic Text-to-Image Generation via Detector-Guided Rewards — 2025 preprint.**
    - arXiv: https://arxiv.org/abs/2512.00473
    - Why it matters: artifact-aware optimization and evaluation.
    - Caution: results depend on the benchmark, detector, and model; do not treat the method as universal proof of realism.

## Official documentation and practitioner education

12. **OpenAI image prompting guide:** https://developers.openai.com/api/docs/guides/image-prompting
13. **Nikon focal length guide:** https://www.nikon.co.uk/en_GB/learn-and-explore/magazine/tips-and-tricks/what-is-focal-length-in-photography-a-guide-for-beginners
14. **Sony Alpha Universe, window-light portraits:** https://www.sony.co.uk/alphauniverse/alpha-academy/articles/top-tips-window-light-portraits

Official specifications are preferred for device details. Practitioner tutorials are useful for vocabulary and workflows, but they are not controlled evidence.

## Community and visual discovery

Community prompts, Pinterest boards, Reddit threads, model galleries, and creator tutorials are hypothesis sources, not proof that a prompt works.

- Pinterest photorealistic portrait prompts: https://www.pinterest.com/search/pins/?q=photorealistic%20portrait%20prompt
- Pinterest natural skin texture: https://www.pinterest.com/search/pins/?q=natural%20skin%20texture%20portrait%20photography
- Pinterest window-light portraits: https://www.pinterest.com/search/pins/?q=natural%20window%20light%20portrait
- Reddit search: https://www.reddit.com/search/?q=photorealistic%20image%20prompt
- Stable Diffusion community search: https://www.reddit.com/r/StableDiffusion/search/?q=photorealistic%20portrait%20prompt&restrict_sr=1
- GitHub repositories: https://github.com/search?q=photorealistic+prompt&type=repositories
- Hugging Face models: https://huggingface.co/models?search=photorealistic
- arXiv research: https://arxiv.org/search/?query=photorealistic+image+generation&searchtype=all
- CVF Open Access: https://openaccess.thecvf.com/

For each useful community item, capture the original URL, author, date, model/version, exact prompt and settings if supplied, provenance, license, and whether it was independently reproduced. Search-result snippets are leads; follow them to the primary source.

## Evidence labels

- **Peer-reviewed:** published in a reviewed journal or conference; methods still need scrutiny.
- **Preprint:** not necessarily peer-reviewed.
- **Official specification:** manufacturer or software documentation.
- **Practitioner guidance:** useful workflow or professional advice.
- **Community observation:** prompt post, thread, or anecdote.
- **Internal experiment:** a documented test performed for this repository.
- **Hypothesis:** plausible but not yet tested.

## Research queue

- Skin microtexture and subsurface scattering under different illuminants.
- Skin-tone fidelity across a range of complexions and mixed lighting.
- Sensor noise versus artificial grain and JPEG artifacts.
- Smartphone multi-frame HDR, sharpening, denoising, tone mapping, and portrait segmentation.
- Focal length, camera distance, perspective, and facial proportions.
- Depth of field and bokeh across generation models.
- Flare, veiling glare, chromatic aberration, vignetting, and dust.
- Human perception of authenticity and limits of AI-image detectors.
- Prompting versus reference-image conditioning, relighting, ControlNet, LoRA, and model-specific tools.

## Rights and reuse

Link to sources and write original summaries. Do not mirror full papers, paid prompt packs, or scraped image collections without permission. See docs/research/DATA-AND-RIGHTS.md.