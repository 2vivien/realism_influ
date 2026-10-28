# Skin Realism Pack

**Status:** design specification; prompt modules remain hypotheses until tested.

Skin is a spatially varying biological material photographed under a specific light source and camera pipeline. Do not reduce it to “pores plus blemishes.” Tone, texture, reflectance, age-related features, makeup, lighting, distance, and processing interact.

## Variables

### Microtexture
- Pore visibility: subtle, visible at close range, or macro.
- Distribution: region-dependent; avoid uniform stippling.
- Fine skin lines: depend on expression, age, region, and light.
- Vellus hair: visible only when scale, focus, and illumination support it.
- Surface irregularity: natural variation, not random noise pasted onto the face.

### Surface reflectance
- Matte, balanced, naturally reflective, or oily highlights.
- T-zone variation: forehead, nose, and chin can reflect differently from cheeks.
- Highlight size and intensity depend on source size, angle, surface, exposure, and processing.
- Avoid uniform wet, plastic, or mirror-like skin unless the scene calls for it.

### Color variation
- Local redness and pigmentation.
- Freckles, moles, sun spots, or blemishes only when requested or appropriate.
- Under-eye color and shadow should not become painted-on dark patches.
- Preserve intended skin tone under the stated illumination and white balance.
- Do not imply one texture or color is the default for all people.

### Shape and expression
- Expression lines follow facial movement.
- Folds and creases follow anatomy and expression.
- Asymmetry should remain plausible rather than distort geometry.
- Texture follows shape and lighting instead of floating as a flat overlay.

### Makeup and grooming
- Foundation may smooth or alter texture.
- Lip texture, eyeliner, lashes, brows, and concealer respond to light and focus.
- Avoid overdrawn lips, identical eyelashes, uniform brows, and excessively crisp facial boundaries unless stylistically intended.

## Prompt fragments to test

**Natural close portrait:**  
“Natural skin surface with regionally varied fine texture, subtle pores visible at this distance, delicate vellus hair where the light catches it, realistic tonal variation, and highlights consistent with the soft key light. Preserve natural facial geometry; avoid waxy smoothing and uniformly sharpened texture.”

**Soft beauty light:**  
“Healthy-looking skin with controlled broad highlights and gentle tonal transitions; retain fine texture without exaggerating pores or blemishes. Makeup, if present, has realistic coverage and follows the skin.”

**Low-light smartphone target:**  
“Skin rendered under the stated low-light environment, with restrained computational denoising and realistic fine-detail retention. Do not use heavy grain as a substitute for skin texture.”

**Editorial macro detail:**  
“Close-range skin detail with scale-appropriate pores, fine hairs, and small tonal variations; depth of field and focus falloff remain consistent with the intended lens and working distance.”

## Controlled variables

| Variable | Levels | Question |
|---|---|---|
| Texture wording | absent / restrained / explicit | Does detail help or create stippling? |
| Specularity | matte / balanced / oily | Do highlights remain coherent? |
| Pore scale | subtle / close-up / macro | Does texture match framing? |
| Color variation | minimal / subtle regional | Does it look natural or blotchy? |
| Fine hair | omitted / selectively visible | Does it follow light and focus? |
| Retouching | documentary / restrained beauty / editorial | Does it match the genre? |
| Light size | large soft / small hard | How do pores and highlights change? |
| Processing | neutral / denoised / sharpened | Does processing preserve texture? |

## Failure catalog

- **Waxy skin:** over-smoothing, uniform specularity, lost low-frequency detail, or model priors.
- **Pore overlay:** repeated dots without relation to anatomy or light.
- **Oily face:** highlights too intense or uniform across regions.
- **Painted freckles:** overly regular or sharp spots not integrated with shading.
- **Artificial dirt:** random marks added without a coherent scenario.
- **Over-sharpened texture:** cutout-like pores and halos.
- **Skin-tone drift:** illumination, white balance, surrounding colors, or model bias changes the intended complexion.
- **Texture mismatch:** hyper-detailed face with smooth neck, ears, hands, clothing, or background.

## Evaluation checklist

- Does texture scale match crop and viewing distance?
- Are pores spatially plausible rather than uniform?
- Do highlights match source size and direction?
- Does texture continue plausibly across face, ears, neck, and hands?
- Are marks integrated with shading?
- Is skin tone preserved under the scene lighting?
- Does the image remain plausible at normal viewing size?
- Is detail consistent with hair, eyes, clothing, and background?

## Asset schema

Recommended fields: asset ID, name, description, variables, prompt fragment, intended scenario, model/version, source IDs, status, known failures, test date, output references, and notes.

Do not assign numeric pore sizes or reflectance values unless a measurable physical scale is defined and sourced. Prompt descriptors are not calibrated biological measurements.