# Camera & Optics Profile Library

**Status:** profiles are templates and visual targets unless the exact device/lens is verified and the model behavior experimentally validated.

## Three separate records

1. **Physical specification:** verified from manufacturer documentation or EXIF.
2. **Intended visual target:** the look requested in a prompt.
3. **Observed behavior:** what the model actually produced.

A prompt's camera metadata is not proof that a generator simulated that camera.

## Profile schema

Record exact device and lens, sensor format/resolution, physical focal length, 35 mm-equivalent focal length where relevant, aperture, subject distance, focus distance, shutter, ISO, stabilization, capture format, processing, source URL, verification date, and status.

## Starter visual profiles

### CAM-001 — Main smartphone camera, casual portrait
Use a plausible camera distance and main-camera perspective. Avoid extreme facial enlargement from very close wide-angle placement unless intended. Mention restrained computational sharpening or HDR only as a target, not a universal device signature. Do not automatically add JPEG artifacts or noise.

Prompt: “Casual main-camera smartphone photograph, natural perspective for the stated camera distance, restrained computational HDR and sharpening, realistic highlight handling, and detail consistent with available light.”

### CAM-002 — Wide-angle documentary scene
Wide field of view and strong foreground/background relationships. Perspective depends on camera position; wide lenses do not independently force all perspective distortion. Keep edges and geometry plausible.

### CAM-003 — Normal-lens environmental portrait
A 35–50 mm-equivalent target can be useful depending on format and framing. Specify camera distance and background detail.

### CAM-004 — Full-frame portrait lens
Example target: 85 mm lens at f/2 on a compatible full-frame camera. Specify subject and background distance. Use gradual optical defocus, not a uniform blur mask. Record the actual lens model and settings if known.

### CAM-005 — Compact camera / point-and-shoot
Casual snapshot look, restrained processing, direct flash if appropriate. Do not add film borders or heavy grain unless requested.

## Focal length, perspective, and depth of field

- Focal length affects angle of view for a given sensor format.
- Camera position determines perspective relationships. Moving closer or farther changes relative size and facial proportions.
- Depth of field depends on aperture, focal length, focus distance, sensor format, and acceptable circle of confusion.
- Background blur is not determined by aperture alone.
- Bokeh depends on lens design, aperture, aberrations, focus, and scene highlights.
- Equivalent focal length communicates angle of view relative to a reference format; it is not the physical focal length of every camera.
- Smartphone portrait blur may be computationally simulated rather than purely optical.

## Optical behavior

Only include when the scenario supports it: barrel/pincushion distortion, vignetting, chromatic aberration, veiling glare, flare, diffraction, focus breathing, edge rendering, motion blur, and sensor noise.

## Example: iPhone main camera

Do not publish one generic signature for all iPhones. A target such as “26 mm equivalent, f/1.8” must be tied to a particular model and camera module before it is treated as a specification. Device generations, camera modules, and processing pipelines differ.

## Example: Sony A7 IV + 85 mm lens

The α7 IV is a full-frame interchangeable-lens camera. “85 mm f/2” describes a compatible lens and aperture, not the camera body. Record the lens model, focus distance, shutter, ISO, lighting, file format, and processing if known.

## Research links

- Generative Photography: https://generative-photography.github.io/project/
- PreciseCam: https://research.adobe.com/publication/precisecam-precise-camera-control-for-text-to-image-generation/
- CamEdit: https://papers.nips.cc/paper_files/paper/2025/hash/a60567166d738f4c43e563fdf8a2afe4-Abstract-Conference.html