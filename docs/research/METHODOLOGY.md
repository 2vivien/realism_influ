# Research Methodology

## Research questions

1. Which visual properties make a generated image read as a photograph rather than a polished render?
2. Which properties respond to prompts, reference inputs, or explicit tools, and which remain model-dependent?
3. How do skin, hair, lighting, lens behavior, color, compression, and scene geometry interact?
4. Which prompt modules produce repeatable improvements rather than one-off attractive outputs?
5. How can claims be documented without overstating realism or ignoring skin-tone and capture-condition differences?

## Evidence hierarchy

1. **Peer-reviewed primary research:** inspect methods, dataset, baselines, metrics, selection effects, and limitations.
2. **Official technical documentation:** use for device specifications, API controls, and model behavior.
3. **Established imaging reference:** use for physical principles.
4. **Practitioner tutorial:** useful for vocabulary and workflow, not proof of causality.
5. **Community prompt or anecdote:** hypothesis generator only.
6. **Internal experiment:** evidence for the tested scenario and model, not automatically generalizable.

A search snippet, Pinterest caption, or viral prompt is not a factual source until traced to the primary source.

## Source-review procedure

For each source, record a stable ID, title, author, date, venue/domain, URL, access date, evidence class, review status, relevant findings, methods, limitations, related assets, and reuse restrictions. Summarize in original wording. Relevance and reliability are separate fields.

## Hypothesis-driven prompt design

Good questions include:
- Does restrained skin-texture wording improve naturalness under a large soft source?
- Does camera distance plus framing improve facial proportions more reliably than focal length alone?
- Does moderate local contrast preserve skin texture better than global sharpening?
- Does added grain help at intended viewing size or merely conceal defects at a crop?

Avoid “Is this prompt better?” unless better is defined.

## Controlled experiments

- Establish a baseline.
- Change one primary variable at a time where feasible.
- Keep model/version, aspect ratio, quality, reference inputs, seed, and other settings constant where supported.
- If deterministic seeds are unavailable, state that limitation and use repeated samples.
- Save exact prompts, settings, outputs, and evaluation notes.
- Compare native resolution and intended display size.
- Record negative outcomes and regressions.
- After single-variable tests, test interactions such as source size × skin specularity or focal length × camera distance.

## Human evaluation

When feasible, randomize image order and hide prompt/model metadata. Ask separately about photographic plausibility, technical quality, aesthetics, and perceived authenticity. Record evaluator count, display conditions, viewing size, time limits, and selection effects. Do not claim population-level conclusions from informal votes.

## Artifact analysis

Inspect at three scales:
- **Normal display size:** composition and photographic plausibility.
- **Native resolution:** texture, hair, eye detail, edge transitions, noise, and compression.
- **Crops:** anatomy, skin consistency, reflections, geometry, and material boundaries.

Describe and prioritize defects. Do not add every possible defect to a prompt.

## Claim language

Prefer “observed in these trials,” “the paper reports,” “this appears model-specific,” and “untested hypothesis.” Avoid “guaranteed photorealism,” “works with every model,” or “scientifically proven” without a suitable study.

## Reproducibility checklist

Record experiment ID/date, question, hypothesis, source IDs, model/provider/version, task mode, exact prompts, all exposed settings, seed if available, reference provenance, number of trials, output links, evaluation method, results, failures, confounders, limitations, and next step.