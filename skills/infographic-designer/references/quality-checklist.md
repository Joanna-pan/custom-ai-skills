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

- PNG dimensions match the brief.
- PPTX elements intended for editing are actually editable.
- PSD opens successfully and contains multiple meaningful, named layers or groups rather than one flattened composite.
- PSD groups separate `Text`, `Data-Charts`, `Illustrations`, `Decor`, `Background`, and `Sources` when those content classes exist.
- Text remains native and editable when the available workflow supports Photoshop text layers. Otherwise, each text block remains separate in `Text` and the rasterized-text limitation is disclosed.
- PNG, PPTX, and PSD contain the same approved content, geometry, and palette.
- PSD canvas dimensions, color mode, transparency, stacking order, and clipping match the approved output.
- Generated imagery contains no accidental text, malformed symbols, or misleading objects.
- Source links and credits are present when required.

## Visual Inspection Passes

1. Inspect at 100% scale for alignment, text rendering, and connector accuracy.
2. Inspect as a thumbnail for hierarchy and immediate comprehension.
3. Inspect at the target mobile/desktop/print context.
4. Open or render the PPTX independently; do not assume the export proves editability.
5. Open the PSD independently, inspect its layer panel, toggle each major group, and compare a composite render with the approved PNG.
6. After a palette-only revision, compare geometry to the approved version and confirm that only intended color changes occurred in every default format.

Do not deliver until blocking issues are fixed. If a limitation cannot be fixed with available tools, state it precisely and provide the best production-ready fallback.
