# Photographic Scenario Cards

Each card is a starting prompt skeleton. Fill in the subject and context, then test it against a baseline. Camera settings are visual targets unless the model provides and demonstrates explicit camera control.

## SCN-PORTRAIT-001 — Natural window-light portrait

**Goal:** believable portrait with restrained retouching.

**Prompt skeleton:**  
“Natural portrait of [adult subject], [expression and pose], photographed indoors near a large window to camera-left. Broad daylight creates gradual facial shadow transitions, with subtle room bounce from the opposite side. Preserve coherent facial geometry, natural skin texture appropriate to the framing, believable hair strands, and skin highlights consistent with the source. Neutral photographic color, restrained sharpening, and a background whose focus and illumination fit the camera distance.”

**Variables to test:** source size, direction, texture wording, camera distance, background distance.

**Failure checks:** contradictory catchlights, flat shadowless face, oily sheen, repeated pore pattern, blurred hair halo.

## SCN-PHONE-001 — Casual smartphone snapshot

**Goal:** ordinary everyday capture rather than polished campaign imagery.

**Prompt skeleton:**  
“Casual smartphone photograph of [adult subject] [doing an ordinary activity] in [specific environment]. Main-camera framing from a plausible everyday distance, natural ambient light from [source/direction], spontaneous but anatomically plausible posture, realistic clothing folds, and detail consistent with available light. Restrained computational sharpening and HDR, natural color, and no artificial studio glow.”

**Optional only if scenario supports it:** slight framing imperfection, motion blur in moving background, compression consistent with sharing.

**Failure checks:** extreme wide-angle face distortion without close camera placement, fake grain everywhere, impossible background blur.

## SCN-CANDID-001 — Friend-taken outdoor photograph

**Goal:** spontaneous outdoor image with coherent daylight.

**Prompt skeleton:**  
“Unposed documentary-style photograph of [adult subject] [action] in [location type]. Camera at [height and distance], [wide/normal field-of-view target], [overcast/open-shade/direct-sun] illumination from [direction]. Natural expression and movement, coherent perspective, believable shadow direction, realistic skin and hair detail at this viewing distance, and ordinary color processing.”

**Failure checks:** shadow direction conflicts, subject looks staged, motion blur without movement, background perspective errors.

## SCN-INDOOR-001 — Warm restaurant / evening interior

**Goal:** believable mixed light and background.

**Prompt skeleton:**  
“Photograph of [adult subject] in a real-feeling restaurant interior at evening. Warm practical lamps illuminate nearby surfaces while cooler ambient light enters from [source]. Preserve mixed-light color shifts, plausible reflections on glass and metal, background exposure consistent with the room, and natural skin highlights. Framing is [shot type] from [camera distance], with focus and blur appropriate to the scene.”

**Failure checks:** uniform orange filter, reflections without sources, background brightness inconsistent with light, blur mask around hair.

## SCN-EDITORIAL-001 — Professional beauty portrait

**Goal:** controlled, polished photography that still respects physical coherence.

**Prompt skeleton:**  
“Professional beauty portrait of [adult subject], [styling and expression], with a large diffused key source at [direction] and restrained fill from [direction]. Catchlights and facial shadows correspond to the source setup. Skin texture is preserved but not exaggerated; makeup has realistic coverage; hair highlights follow the light. Controlled color rendering and smooth highlight transitions, with no waxy smoothing or artificial glow.”

**Failure checks:** flat lighting despite directional source, uniform oily skin, excessive retouching, impossible hair highlights.

## SCN-LOWLIGHT-001 — Dim indoor phone capture

**Goal:** plausible low-light computational photography.

**Prompt skeleton:**  
“Casual low-light smartphone photograph of [adult subject] in [dim environment], illuminated by [motivated practical source]. Exposure and detail reflect the limited available light. Fine details remain plausible after restrained denoising; any motion blur follows subject or camera movement. Preserve mixed color from the actual sources and avoid adding uniform grain as a shortcut.”

**Failure checks:** clean daylight-level detail in deep darkness, heavy noise without cause, blur on static objects only, unnatural skin tone.

## SCN-PRODUCT-001 — Product in a real environment

**Goal:** believable material and contact behavior.

**Prompt skeleton:**  
“Photograph of [product] resting on [surface] in [environment], illuminated by [source and direction]. Preserve the product's geometry, material roughness, reflections, contact shadow, scale, and perspective. Camera position and focus suit the intended product shot; color rendering is restrained and consistent with the light.”

**Failure checks:** floating object, reflection mismatch, incorrect contact shadow, inconsistent perspective, plastic-like materials.

## Usage notes

- Do not combine multiple scenario cards unless the scene genuinely combines them.
- Keep the baseline prompt concise and internally consistent.
- Record the model/version and exact settings.
- Use the evaluation rubric and preserve failures as well as successes.
