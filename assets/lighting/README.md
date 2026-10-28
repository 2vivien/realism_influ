# Lighting Profile Library

**Status:** profile templates and prompt fragments; not validated universal presets.

A lighting description should specify the scene's sources and their relationship to the subject. “Soft light” alone is underspecified: softness primarily depends on the source's apparent angular size and geometry, while exposure and fill determine brightness and contrast.

## Profile schema

Record profile ID, scenario, source type, apparent size, distance if known, direction/elevation, intensity relationship, color, fill/bounce, shadow direction and softness, specular behavior, background illumination, camera assumptions, source URL, status, and limitations.

## Starter profiles

### LGT-001 — Large window, overcast daylight
Intent: natural portrait with broad, gentle transitions.
- Large window or bright sky off-axis.
- Room bounce weaker than the key.
- Visible but soft shadows with gradual transitions.
- Broad controlled skin highlights.
- Background falloff consistent with room geometry.

Prompt: “Soft daylight from a large window camera-left, broad source reflections in the eyes, gentle shadow falloff across the face, subtle room bounce from the opposite side, and background brightness consistent with the window direction.”

### LGT-002 — Open shade / bright overcast
Broad sky illumination and soft shadows. Environmental color may reflect onto the subject. Avoid hard direct-sun shadows unless another source explains them.

### LGT-003 — Direct sunlight
Directional light, clear shadow structure, stronger contrast, and highlights that may clip depending on exposure. Avoid softbox-like highlights without diffusion or fill.

### LGT-004 — Warm practical interior plus cool window
Distinct sources may have different colors. White balance cannot necessarily neutralize both simultaneously. Skin and surfaces should show plausible local color shifts rather than one uniform filter.

### LGT-005 — Softbox beauty portrait
Large diffuse source near or off camera axis. Catchlights, nose shadow, and fill must agree. “Beauty light” should not automatically mean flat frontal light.

### LGT-006 — Backlight / rim light
Source behind or behind-side of subject. Hair highlights align with the source. Flare appears only when source geometry and lens conditions support it. Avoid a uniform glowing outline without a motivated source.

### LGT-007 — On-camera phone flash
Near-axis light, potentially hard shadows and specular highlights, with background exposure dependent on ambient light and settings. Avoid mixing studio catchlights and direct-flash shadows without multiple sources.

### LGT-008 — Dim indoor ambient
Low photon levels can lead to longer exposure, higher gain, multi-frame processing, or blur. Denoising may soften detail. Motion blur should relate to actual movement.

## Lighting prompt composition

Source + apparent size + direction + color + intensity relationship + fill/bounce + shadow behavior + background relationship + surface response.

## Research note

Prompting cannot guarantee physically accurate relighting. Compare prompt-only generation with explicit relighting methods such as LightLab and SynthLight. Record whether the result came from text-to-image, editing, relighting, or compositing.