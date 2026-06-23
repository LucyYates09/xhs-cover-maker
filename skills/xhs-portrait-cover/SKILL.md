---
name: xhs-portrait-cover
description: Create and refine 3:4 Xiaohongshu portrait covers from a selfie, style reference, exact Chinese headline, and optional brand logos. Use when Codex needs to analyze a reference cover, propose concise cover copy, preserve a real person's identity and original background, build bold layered typography, add logo cards, or correct portrait lighting to look like a frontal soft beauty panel instead of rim light or a glowing cutout.
---

# Xiaohongshu Portrait Cover

Create high-impact portrait covers while preserving the real person and keeping revisions controlled.

## Workflow

1. Inspect every supplied image and label its role:
   - portrait/edit target;
   - composition or style reference;
   - logo or supporting graphic.
2. Separate the cover artwork from any Xiaohongshu interface shown in a screenshot. Reproduce only the artwork unless the user explicitly requests UI.
3. Extract the exact title, subtitle, label, palette, background preference, and logo requirements. Keep user-approved text verbatim.
4. If the title is unsettled, propose short two-line options before generating:
   - line 1: context, urgency, or audience;
   - line 2: action, tool, or outcome;
   - prefer 6–10 Chinese characters per line;
   - keep English product names correctly spelled.
5. Generate or edit with the image-generation capability. Use the portrait as an identity reference and preserve facial structure, glasses, moles, hairstyle, expression, pose, clothing, and body proportions.
6. Default to the person's real background when it is usable. Treat brand colors as accents in typography, brush strokes, labels, and logo cards—not as permission to replace the whole background.
7. Validate the result before presenting it:
   - 3:4 cover ratio and safe margins;
   - exact Chinese text and English spelling;
   - recognizable identity;
   - readable title at thumbnail size;
   - no unwanted app UI, watermark, duplicate logos, or added copy;
   - physically plausible portrait lighting.
8. Make revisions one variable at a time. Repeat all invariants in every edit prompt.

## Layout Recipe

Use this hierarchy unless the reference indicates otherwise:

- Top 35–40%: two-line oversized headline with white fill, navy/black extrusion, and restrained brand-color accents.
- Lower 55–65%: large half-body or waist-up portrait.
- One small rounded pill: category label such as `AI求职工具`.
- One or two tilted rounded-square logo cards: secondary to the face and title.
- Original background: slightly softened only when needed for legibility.

Do not copy a reference literally. Reuse its hierarchy, contrast, depth, and energy while producing an original arrangement.

## Portrait Lighting

Distinguish frontal face light from rim light:

- **Frontal face light**: broad soft source centered just above the camera; evenly lifts forehead, both cheeks, eyes under glasses, nose, mouth, chin, neck, and upper chest.
- **Rim light**: bright edge around hair, shoulders, or clothing. Do not use it when the user asks to brighten the face.

For a stronger face light, raise the face about 0.8–1 stop, open shadows behind glasses, and add subtle broad catchlights. Preserve pores, skin tone, moles, and facial contours. Avoid clipped highlights, oily shine, plastic smoothing, face reshaping, halos, neon outlines, or globally brightening the background.

When correcting a mistaken rim-light edit, explicitly remove the white/blue outline before requesting stronger frontal illumination.

## Editing Discipline

For each revision:

1. State the single requested change.
2. List everything that must remain unchanged.
3. Describe the light source or visual change physically, not only with adjectives.
4. Prohibit the most likely failure mode.
5. Re-check identity, text, background, and layout after generation.

Read [references/prompt-recipes.md](references/prompt-recipes.md) for reusable prompts and [references/qa-checklist.md](references/qa-checklist.md) for final inspection.
