# Smartphone Computational Photography

## Why a phone is not just a small camera

A smartphone photograph is often the output of a computational pipeline, not a single untouched sensor exposure. The exact pipeline varies by device, mode, app, and firmware. Manufacturer documentation describes HDR fusion and differences between processed and RAW/ProRAW capture.

## Core stages to investigate

### Multi-frame HDR and fusion
Multiple exposures or frames may be combined to retain highlight and shadow information. This can affect local contrast, ghosting, texture, and highlight roll-off.

### Denoising
Noise reduction may combine spatial and temporal information. Fine hair, skin texture, and fabric detail can be softened or reconstructed.

### Sharpening and local contrast
Edge enhancement can increase apparent crispness but may introduce halos or exaggerated texture.

### Tone mapping
The pipeline maps scene brightness into displayable output. Shadows may be lifted, highlights compressed, and local contrast adjusted.

### Color rendering
White balance and color matrices affect skin, neutrals, foliage, and indoor lighting. Mixed light may remain visible even after automatic white balance.

### Portrait mode
Background blur may be computationally segmented, optical, or a mixture. Hair, glasses, transparent objects, and complex edges can expose segmentation errors.

### Encoding and sharing
JPEG/HEIF encoding and social-platform recompression can alter fine detail, edges, chroma, and noise.

## Research links

- Apple HDR support: https://support.apple.com/en-lamr/guide/iphone/iph2cafe2ebc/ios
- Apple RAW and ProRAW documentation: https://developer.apple.com/documentation/avfoundation/capturing-photos-in-raw-and-apple-proraw-formats

These explain aspects of Apple's pipeline; they do not establish that all smartphone brands use the same implementation.

## Prompting implications

A smartphone look may be described through plausible framing, available-light behavior, restrained sharpening, HDR character, denoising, and color rendering. Do not automatically add noise, JPEG blocks, wide-angle distortion, or shallow depth of field. Those properties depend on the device, scene, selected camera module, exposure, and processing.

## Suggested experiment

Compare three prompt conditions with the same scenario:
1. Smartphone label only.
2. Smartphone label plus plausible distance and framing.
3. Scenario plus restrained computational-processing description.

Evaluate framing, face proportions, highlight handling, fine-detail retention, background blur, and overall plausibility. The result can show whether the model responds to these terms; it cannot prove the image was produced by an actual phone.
