# Experiment Protocol

## Required record

- Experiment ID and date.
- Operator.
- Research question and hypothesis.
- Source IDs.
- Image scenario and target use.
- Model/provider, exact version, and task mode.
- Exact baseline prompt and all variants.
- Negative prompt if supported.
- Seed and exposed generation settings.
- Aspect ratio, resolution, quality mode, reference inputs, and masks if used.
- Number of attempts per condition.
- Output filenames/links and provenance.
- Evaluation rubric and conditions.
- Results for every trial.
- Failures, regressions, confounders, limitations, and next step.
- Status: planned / running / analyzed / replicated / inconclusive.

## Procedure

1. Define one measurable question.
2. Choose a baseline and one primary variable.
3. Freeze other controllable settings.
4. Generate multiple samples when the system is stochastic.
5. Record all outputs, not only the best.
6. Evaluate at intended viewing size and native resolution.
7. Blind evaluators to condition labels where possible.
8. Report failures and uncertainty.
9. Repeat before describing an effect as reproducible.
10. Publish a concise summary with source and output links.

## Example: skin texture wording

Question: does restrained texture wording improve perceived naturalness without creating stippling?

- A: baseline, no explicit skin-texture module.
- B: same prompt plus “fine, regionally varied skin texture appropriate to this framing.”
- C: same prompt plus explicit pores, fine hair, and highlight description.

Keep scene, model/version, settings, reference input, and seed constant where supported. If seeds are unavailable, use repeated samples and report that limitation.

Metrics: naturalness at normal display size (1–5), skin texture plausibility (1–5), artificial stippling (0–3), skin-tone consistency (1–5), and overall image quality (1–5, separate from realism).

Do not assume C wins because it contains more detail.

## Example: camera target

Question: does a coherent capture description improve framing and focus behavior compared with focal length alone?

- A: focal length only.
- B: focal length plus camera-to-subject distance and framing.
- C: B plus aperture, focus, and depth-of-field target.

Record whether the model maintains the scene and whether changes match requested camera behavior. A different-looking output is not proof of accurate camera control.

## Example: lighting

Question: does source size and direction improve facial shadow coherence?

- A: generic “soft light.”
- B: large window source from camera-left.
- C: B plus room bounce and shadow transitions.

Rate shadow direction, edge softness, catchlights, skin highlights, and overall plausibility separately.

## Interpretation

Do not compare different model versions as a controlled prompt test. Do not select only the best sample. Do not infer causality from one image. Report variation where possible. A prompt can improve aesthetics while reducing realism; record both separately.