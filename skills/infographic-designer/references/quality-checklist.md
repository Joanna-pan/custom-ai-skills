# Quality Checklist

Run this checklist against the rendered artifact, not only against source code or a prompt.

## Meaning

- The title, takeaway, and reading path are understandable without narration.
- The composition matches the relationship in the content.
- Visual prominence corresponds to informational importance.
- Measured values are not distorted by area, perspective, truncated scales, or inconsistent units.
- Schematic relationships are not presented as measured data.

## Content

- No invented facts, numbers, dates, quotations, or sources.
- Claims match their cited sources.
- Terminology, capitalization, units, and date formats are consistent.
- Copy is concise without removing necessary conditions or caveats.
- Spelling and punctuation are checked in the output language.

## Layout And Typography

- No clipping, overlap, orphaned labels, crossed text, or off-canvas elements.
- The longest word and longest label fit their containers.
- Body text remains readable at the actual publication size.
- Heading levels are visually distinct and limited.
- Connectors clearly attach to their intended nodes.
- The layout remains stable after final copy is inserted.

## Color And Accessibility

- Text and meaningful marks have sufficient contrast.
- Color is not the only carrier of category, state, or direction.
- Adjacent categories remain distinguishable in grayscale where relevant.
- A short description and structured long description exist for complex factual graphics.

## Production

- The PNG review draft was rendered and inspected before editable formats were produced, unless the user explicitly skipped review.
- When the requested style depends on generated imagery, the actual full image-generation model was used and recorded; `openai/gpt-image-2` was preferred when available.
- Rendered, illustrative, material, or dimensional styling was not silently replaced by programmatic SVG, primitive icons, gradients, or pseudo-3D.
- When a reference was supplied, its fidelity mode was confirmed or already explicit, and the result follows only the approved traits.
- PNG dimensions match the brief.
- When PPTX is requested, elements intended for editing are actually editable.
- When PSD is requested, it opens successfully and contains multiple meaningful, named layers or groups rather than one flattened composite.
- When PSD is requested, groups separate `Text`, `Data-Charts`, `Illustrations`, `Decor`, `Background`, and `Sources` when those content classes exist.
- When PSD is requested, text remains native and editable when the available workflow supports Photoshop text layers. Otherwise, each text block remains separate in `Text` and the rasterized-text limitation is disclosed.
- Every produced format contains the same approved content, geometry, and palette.
- When PSD is requested, canvas dimensions, color mode, transparency, stacking order, and clipping match the approved output.
- Generated imagery contains no accidental text, malformed symbols, or misleading objects.
- Source links and credits are present when required.
- In OpenClaw WebChat, each promised file is delivered as a real reply attachment rather than only a tool-result preview or local-only link.
- Temporary preview servers and background render processes are stopped before the final answer unless the user explicitly asked to keep them running.

## Visual Inspection Passes

1. Inspect at 100% scale for alignment, text rendering, and connector accuracy.
2. Inspect as a thumbnail for hierarchy and immediate comprehension.
3. Inspect at the target mobile/desktop/print context.
4. When PPTX is produced, open or render it independently; do not assume the export proves editability.
5. When PSD is produced, open it independently, inspect its layer panel, toggle each major group, and compare a composite render with the approved PNG.
6. After a palette-only revision, compare geometry to the approved version and confirm that only intended color changes occurred in every produced format.
7. In OpenClaw, confirm that deliverable paths exist before emitting attachment directives and that no temporary background process remains after delivery.

Do not deliver until blocking issues are fixed. If a limitation cannot be fixed with available tools, state it precisely and provide the best production-ready fallback.
