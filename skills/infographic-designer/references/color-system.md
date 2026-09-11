# Color System

Treat palette as a replaceable design subsystem rather than an inseparable part of composition.

## Palette Roles

Define colors by role: background, primary text, secondary text and rules, one or two base colors, one to three accents, and semantic states such as positive, warning, negative, unknown, or inactive.

Avoid using many unrelated accent colors merely to decorate sections.

## Concept Presentation

For complex mode, offer up to three swatch sets when color direction is unresolved:

1. Recommended palette: best fit for topic, medium, and readability.
2. Restrained alternative: lower visual intensity and broader professional use.
3. Expressive alternative: stronger character with stated risks.

Show swatches with role names and hex values when the production format supports exact color.

## Accessibility

- Target at least 4.5:1 contrast for ordinary text and 3:1 for large text.
- Keep essential graphical boundaries and states distinguishable; do not rely on hue alone.
- Reinforce status with labels, symbols, line styles, patterns, or position.
- Test palettes in grayscale or with a color-vision simulation when color encodes categories.

Reference: https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast

## Palette-Only Revision

When the user rejects the palette:

1. Preserve approved content, geometry, hierarchy, and composition.
2. Clarify the desired direction only if terms such as "better" or "nicer" are too ambiguous.
3. Replace role colors, not isolated objects at random.
4. Recheck contrast and category distinguishability.
5. Re-export PNG, PPTX, and layered PSD as a new revision.

If requested colors fail readability, retain their character while adjusting lightness, saturation, or usage, and explain the smallest necessary change.
