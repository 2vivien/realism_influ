# Community Prompt Analysis

**Status:** initial qualitative synthesis of selected public examples. This is not a systematic review and does not establish causality.

## Sources sampled

- Reddit: “How I Fixed Bad AI Faces (After ~1,000 Generations)”  
  https://www.reddit.com/r/comfyui/comments/1sxz97s/how_i_fixed_bad_ai_faces_after_1000_generations/
- Reddit: “How to Generate Realistic AI Portraits Without the AI Look”  
  https://www.reddit.com/r/Aiarty/comments/1vse4iz/how_to_generate_realistic_ai_portraits_without/
- Reddit: “The prompt I use to generate extremely realistic skin texture”  
  https://www.reddit.com/r/midjourney/comments/1oa7jsj/the_prompt_i_use_to_generate_extremely_realistic/
- Reddit: “How I Create Realistic Photography in MidJourney”  
  https://www.reddit.com/r/Aiarty/comments/1p08kn5/how_i_create_realistic_photography_in_midjourney/
- GitHub: Raw Camera Casting prompt system  
  https://github.com/0aicoder0/raw-camera-casting-prompt
- Prompt gallery: PicGens realistic-photo prompts  
  https://www.picgens.com/prompts/chatgpt-realistic-photo-prompts
- Official Midjourney Prompt Basics  
  https://docs.midjourney.com/hc/en-us/articles/32023408776205-Prompt-Basics

## Repeating patterns

### 1. Describe a photograph, not just “realism”
Community examples often specify the shot type, subject, environment, and photographic intent rather than relying only on phrases such as “ultra realistic” or “8K.” This is a useful hypothesis, not a universal rule.

### 2. Name one coherent light setup
Common examples include side window light, overcast daylight, softbox light, and mixed warm/cool indoor sources. A single motivated setup is easier to evaluate than contradictory lighting adjectives.

### 3. Make the subject behavior specific
Expression, gaze, posture, camera distance, and framing are frequently more actionable than a generic “beautiful person” description.

### 4. Treat skin texture as conditional
Pores, peach fuzz, freckles, under-eye texture, and small tonal variation appear frequently. The risk is overcorrection: repeated stippling, exaggerated pores, artificial grime, or skin that looks older/rougher than intended.

### 5. Camera language is popular but may be decorative
“85 mm,” “f/1.4,” “shot on a named camera,” and “shallow depth of field” appear often. Research on camera-conditioned generation indicates that natural-language camera labels do not guarantee physically consistent camera control. Treat them as visual targets unless measured.

### 6. Small imperfections are scenario-dependent
Flyaway hair, slight motion blur, imperfect framing, and compression can support a casual snapshot. They may harm a clean studio portrait or product photograph if added indiscriminately.

### 7. Long prompts are not automatically better
Some community guides promote long, detailed recipes; official Midjourney guidance explicitly recommends clear, specific prompts and warns against excessive lists. The correct approach is to test prompt length and structure for each model.

## Confounders in community claims

- The author may show only the best output.
- Model/version and generation settings may be missing.
- Reference images or post-processing may contribute more than the text.
- The prompt may have been optimized for a single face, style, or scenario.
- “Looks real” may mean “looks attractive” or “looks like stock photography.”
- A highly upvoted post is not a controlled experiment.
- Prompt fragments can interact and change the result unpredictably.

## Prompt pattern worth testing

Subject and behavior → shot type and framing → environment → one motivated lighting setup → skin/hair/material detail appropriate to scale → camera/processing target → concise constraints.

Use this as an experimental baseline, not a proven formula.

## Recommended experiment matrix

Compare:
- Short coherent prompt vs. long adjective-heavy prompt.
- General realism terms vs. concrete photographic scenario.
- Camera label only vs. camera label plus distance and framing.
- Generic soft light vs. explicit source direction and size.
- Skin texture omitted vs. restrained vs. highly explicit.
- No artifacts vs. one scenario-motivated artifact.
- Text-only prompt vs. authorized reference-image conditioning.

## Conclusion

The strongest common principle is to reason like a photographer and describe a coherent capture scenario. The repository must now test which details actually help, for which models, and in which contexts. Community examples should remain attributed source leads rather than being copied wholesale or promoted as guaranteed prompts.
