# Image Production And References

## Choose The Production Method

Use a hybrid workflow when the infographic combines expressive imagery with exact information design:

- Use a genuine image-generation model for illustrative scenes, dimensional objects, material appearance, depth, lighting, textures, paper cut, clay, collage, photorealism, and similar visual treatments.
- Use layout, vector, chart, and presentation tools for exact geometry, grids, data encodings, connectors, masks, editable labels, and final typography.
- A user request for a flat vector diagram, chart-led infographic, or deliberately simple geometric style may be produced programmatically when its appearance does not depend on generated illustration.

For generated visual layers, prefer `openai/gpt-image-2`. If it is unavailable, use the best available full image-generation model and state which model was used. Do not silently replace image generation with an SVG, Sharp, Canvas, gradients, primitive paths, or code-built pseudo-3D. If no genuine image model is available, explain the limitation and obtain approval before changing the requested production method.

Keep exact words, numbers, legends, and information-bearing labels out of generated imagery. Ask the image model to leave clean, compositionally intentional areas for separately typeset copy. Decorative text fragments are acceptable only when they do not carry meaning and cannot be mistaken for real labels.

## Clarify Reference Fidelity

When the user supplies a visual reference and has not already defined how to use it, ask one concise question before production:

`Как следовать референсу: максимально близко; взять только выбранные признаки; или использовать лишь как общее направление?`

Interpret the answer as:

1. **Close match** - preserve the approved composition, palette character, materials, depth, and visual rhythm as closely as practical while keeping the new content truthful and respecting rights and policy.
2. **Selected traits** - ask or infer which traits matter, such as palette, style, composition, typography character, icon language, lighting, or texture; do not copy unselected traits.
3. **Inspiration only** - use the reference to understand quality and mood, then create a distinct composition and visual system.

Do not ask this question when the user has already said what to copy, what to ignore, or how closely to follow the reference.

## Build The Image Prompt

Specify the approved fidelity mode, composition, subject, material, perspective, lighting, palette roles, background, aspect ratio, and clean text zones. Include negative constraints for generated words, malformed symbols, inconsistent perspective, clutter, and unwanted visual clichés. Generate the visual layer without critical copy, then add exact text and data during layout.

## Verify The Method

Before claiming the draft is ready:

1. Record the actual image model or production tool used for each major visual layer.
2. Confirm that a requested illustrative or dimensional style came from genuine image generation rather than a code-built imitation.
3. Inspect the rendered PNG at full size and thumbnail size.
4. Check that generated imagery has no accidental text, broken objects, misleading relationships, or insufficient space for labels.
5. State any fallback model or production-method deviation to the user.
