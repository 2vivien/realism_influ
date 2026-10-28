# Color Science & Computational Photography Pack

**Status:** initial knowledge taxonomy.

## Color pipeline

When known, document: scene illumination → material reflectance → sensor response → white balance → demosaicing → denoising → color rendering → tone mapping → sharpening → encoding/compression → display.

Generated images may only approximate this chain. Separate verified settings from intended visual targets.

## White balance and skin tone

- Color temperature is a simplified source description; real sources may have green/magenta or spectral differences.
- Mixed lighting can produce different casts in different parts of the same scene.
- White balance cannot always neutralize several sources simultaneously.
- Surrounding surfaces reflect colored light onto skin.
- Avoid treating one fixed skin color value as invariant across lighting.
- Evaluate fidelity across multiple complexions and illumination conditions.

Prompt: “Natural color rendering under the stated mixed illumination, with believable local color shifts from the environment, controlled saturation, and skin tones coherent with the white balance and light sources.”

## Tone and contrast

Track exposure, highlight clipping, highlight roll-off, shadow detail, black level, global versus local contrast, shadow/highlight hue shifts, saturation, skin microcontrast, sharpening halos, and color grade. Avoid contradictory terms without explaining their relationship.

## Computational photography

**HDR / multi-frame fusion:** can preserve highlight and shadow detail, but aggressive tone mapping can flatten contrast or create halos.

**Denoising:** can reduce noise while erasing hair, pores, and fine fabric, causing waxy skin.

**Sharpening:** increases apparent detail but does not recover information never captured. Excess creates halos and brittle edges.

**Portrait segmentation:** computational blur can fail around hair, glasses, translucent objects, or complex boundaries.

**JPEG/HEIF:** compression depends on codec, quality, content, chroma subsampling, processing, and repeated saves. Artifacts are not universal signs of a phone photo.

## Noise versus grain

Distinguish photon shot noise, read/fixed-pattern noise, luminance noise, chroma noise, film-like grain, artificial digital grain, and JPEG/ringing artifacts. A prompt cannot faithfully simulate a specific sensor's noise pipeline merely by saying “sensor noise.”

## Prompt modules

**Restrained smartphone processing:** “Moderate local contrast, restrained computational sharpening, balanced HDR with natural highlight roll-off, and detail that remains coherent rather than uniformly crisp.”

**Neutral photographic color:** “Believable white balance for the stated light sources, restrained saturation, natural shadow color, smooth highlight transitions, and no excessive teal-orange grading.”

**Warm practical interior:** “Warm practical lights and cooler ambient fill remain distinct, with believable mixed color on nearby surfaces and skin; avoid one uniform orange filter across the entire frame.”

## Evaluation

Check skin, whites, neutral objects, highlights, shadows, saturated objects, and background under the same scene assumptions. Record display conditions and post-processing. Do not infer exact camera settings from appearance alone.