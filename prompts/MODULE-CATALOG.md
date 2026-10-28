# Reusable Prompt Module Catalog

These composable fragments are starting hypotheses, not universal magic tokens. Test them with a named model and scenario. Do not concatenate every module into one prompt.

## Human appearance

**HUM-001 Natural facial detail**  
“Preserve coherent facial geometry and natural variation in skin, lips, eyelids, brows, and fine facial hair; detail should match camera distance and focus.”

**HUM-002 Restrained expression**  
“A relaxed, believable expression with coordinated movement around the eyes, cheeks, and mouth; avoid a frozen smile or mechanically mirrored features.”

**HUM-003 Natural hair structure**  
“Hair contains coherent strand groups with varied direction, plausible roots and occlusion, and highlights that follow the light; include flyaways only where appropriate.”

## Skin

**SKN-001 Balanced microtexture**  
“Fine, regionally varied skin texture visible at this framing, subtle pores and natural tonal variation, with highlights shaped by the stated light source.”

**SKN-002 Restrained specularity**  
“Skin highlights are broad or small according to source size and surface; avoid a uniform oily sheen across the entire face.”

**SKN-003 Close-up detail**  
“Scale-appropriate pores, fine vellus hair, and small surface variations remain integrated with anatomy, focus, and directional light rather than appearing as an overlay.”

## Lighting

**LGT-001 Window light**  
“Large window light from camera-left, gradual shadow transitions, restrained room bounce from the opposite side, and catchlights consistent with the window.”

**LGT-002 Overcast outdoors**  
“Broad sky illumination with soft shadows and environmental color reflected naturally onto the subject.”

**LGT-003 Direct sun**  
“Directional sunlight with clear shadow geometry and contrast consistent with the sun's small apparent angular size.”

**LGT-004 Mixed practical lighting**  
“Distinct warm practical lights and cooler ambient fill remain visible, with local color shifts rather than a uniform filter.”

## Camera and focus

**CAM-001 Casual smartphone target**  
“Casual smartphone main-camera framing at a plausible subject distance, restrained computational sharpening and HDR, and detail consistent with available light.”

**CAM-002 Environmental portrait**  
“A natural perspective that includes the surroundings, with focus and background detail consistent with framing and capture distance.”

**CAM-003 Portrait-lens target**  
“Portrait-lens perspective from a realistic camera distance, with gradual optical defocus and background blur consistent with aperture and subject-background separation.”

## Color and processing

**COL-001 Natural color**  
“Believable white balance for the stated illumination, restrained saturation, natural shadow color, and smooth highlight transitions.”

**COL-002 Restrained phone processing**  
“Moderate local contrast, restrained computational sharpening, balanced HDR, and no excessive clarity halos or waxy denoising.”

**COL-003 Editorial color**  
“Intentional but restrained tonal shaping that preserves skin-tone coherence, material separation, and highlight detail.”

## Capture character

**CAP-001 Plausible candid framing**  
“An unforced, slightly imperfect composition that still follows a believable camera position and subject distance.”

**CAP-002 Motivated motion**  
“Motion blur follows the direction and speed of moving subjects or camera movement; static edges remain consistent with the capture.”

**CAP-003 Compression restraint**  
“Preserve intended image quality; introduce visible compression only when low-quality or repeatedly shared imagery is part of the scenario.”

## Scene coherence

**SCN-001 Physical consistency**  
“Perspective, light direction, shadow softness, reflections, focus, material response, and background geometry remain consistent across the frame.”

**SCN-002 Contact and interaction**  
“Hands, clothing, and objects make plausible contact with surfaces, with consistent occlusion, pressure, scale, and contact shadows.”

## Negative constraints

Use only where the model supports them. Prefer concise constraints over generic lists: avoid waxy skin, uniform pore patterns, painted freckles, inconsistent catchlights, contradictory shadow directions, artificial blur halos, random RGB fringes, anatomical distortions, and implausible object contact.

## Compatibility

Some models ignore camera numbers or do not support separate negative prompts. Text-to-image, image editing, and relighting are different tasks. Record which module was used and whether its effect was observed, not merely intended.