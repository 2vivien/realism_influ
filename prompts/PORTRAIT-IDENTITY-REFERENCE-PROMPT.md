# Portrait Identity Prompt — Reference-Based Close-Up

**Type:** image-to-image / identity-preserving portrait  
**Status:** user-supplied prompt; initial analysis, not yet experimentally validated  
**Purpose:** generate a close-up portrait that preserves the subject identity and hairstyle from a supplied reference image.

## Original prompt (verbatim)

> Ultra close-up front-facing portrait of the exact same woman from image 1. Straight head-on camera angle looking directly into the lens with a calm, beautiful, natural expression. Clear, highly detailed face with realistic skin microtexture, visible pores, and deep brown almond eyes. Keep her exact hairstyle: long dark Boho locs with loose curly tendrils framing her face. Clean, simple, minimalist off-white neutral studio backdrop. High-end editorial photography, perfectly lit face with soft natural lighting, true-to-life human details, no artificial smoothing.

## Usage

1. Supply the intended identity reference as **image 1**.
2. Use this prompt for a close-up identity portrait, not for a full-body image.
3. Keep the reference image and generation settings recorded.
4. Inspect whether facial structure, hairstyle, complexion and expression are actually preserved.
5. If the model supports reference strength, identity adapters or image guidance, record the chosen setting rather than assuming the text alone guarantees identity.

## Important limitation

The phrase “exact same woman” expresses the desired result; it does not guarantee identity preservation. The result depends on the image model, reference-image pathway, strength/settings, crop, and how well the reference depicts the relevant features.
