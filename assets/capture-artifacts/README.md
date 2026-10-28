# Capture Artifact Catalog

Artifacts should arise from plausible camera, lens, exposure, environment, or processing conditions. A checklist of imperfections is not a recipe for realism.

## Motion blur
Cause: relative movement during exposure. Record shutter duration, subject/camera movement, stabilization, and direction. Blur direction and magnitude should fit the scene. Uniform blur on static and moving objects is suspicious unless camera movement explains it.

## Defocus
Caused by focus plane and depth of field. Depends on aperture, focal length, focus distance, sensor format, and scene depth. Watch for cutout-like background blur, hair halos, and inconsistent focus within one plane.

## Sensor noise
Depends on illumination, exposure, sensor, gain/ISO, and processing. Do not paste identical noise across all regions or add heavy noise to a bright clean exposure without explanation.

## JPEG and compression
Possible signs include blocking, ringing, chroma smearing, and detail loss. These depend on codec, quality, content, and repeated saves. Heavy blocks are not a universal “real photo” signature.

## Lens flare and veiling glare
Require plausible bright-source geometry and depend on lens design, coatings, aperture, source angle, and contamination. Avoid arbitrary colored circles or glow without a motivating source.

## Chromatic aberration
Lateral fringing may increase toward image edges; longitudinal fringing behaves differently around focus. Keep it lens-dependent. Uniform RGB outlines on every edge are usually artificial.

## Vignetting and distortion
Depend on optics, focal length, aperture, correction, and image pipeline. Modern processing may correct them. Avoid exaggerated corners or warped edges that contradict the target device.

## Dust and smudges
Lens contamination may affect flare/haze; sensor dust behaves differently and may appear as soft marks under certain conditions. Do not sprinkle random dust onto every image.

## Rolling shutter
Fast motion or panning can skew geometry on some electronic readout systems. Do not add arbitrary warping to a static scene.

## Decision rule

Before adding an artifact, ask: what mechanism causes it; what conditions make it plausible; which region should be affected; what would contradict it; can the target model represent it; and does it improve the intended style in a controlled comparison?

## Status labels

- **Catalogued:** described, not tested.
- **Prompt-tested:** included in a prompt experiment.
- **Post-process-tested:** applied through an explicit editing step.
- **Validated in scenario:** repeated under documented conditions.
- **Not recommended:** tested and found to create implausible results.