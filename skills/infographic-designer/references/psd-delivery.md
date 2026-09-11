# Layered PSD Delivery

Use this contract whenever creating or revising the default Photoshop deliverable.

## Required Structure

Create a genuine layered PSD. Use meaningful names and group only content classes that exist:

1. `Text` - title, headings, labels, body copy, numbers, and source copy.
2. `Data-Charts` - editable chart marks, scales, legends, connectors, and data labels.
3. `Illustrations` - generated or drawn objects and scene elements.
4. `Decor` - textures, shadows, ornaments, and non-informational accents.
5. `Background` - background color, image, or texture.
6. `Sources` - source notes, credits, and related marks when they are better managed separately from primary text.

Preserve sensible subgroups for repeated stages, cards, panels, or carousel pages. Avoid generic names such as `Layer 1`. Keep masks and transparency when they are needed for non-destructive editing.

## Editability

- Prefer native Photoshop text layers for all information-bearing text.
- Keep charts and diagram components independently selectable when the production path supports it.
- Generated raster illustrations may remain raster layers, but separate major objects when later repositioning or palette work is reasonably expected.
- Do not merge unrelated content merely to reduce the layer count.
- Use 8-bit RGB with an embedded sRGB profile for ordinary screen work unless the brief requires a print profile or another color mode.

If native text-layer creation is unavailable, keep every text block on its own named layer inside `Text` and disclose that those layers are rasterized. The editable PPTX remains the source for changing copy. If the environment cannot create a genuine multi-layer PSD at all, do not rename or wrap a flattened PNG as PSD.

## Parity And Verification

1. Build PSD layers from the same approved content model and geometry as the PPTX and PNG.
2. Open or parse the completed PSD independently; successful file creation alone is insufficient.
3. Confirm that the document has multiple named layers/groups and the expected canvas dimensions.
4. Toggle each major group to verify that it contains the intended content and no required content is trapped in the wrong group.
5. Render a composite preview and compare it with the approved PNG for content, palette, alignment, clipping, transparency, and stacking order.
6. Report whether text layers are native or rasterized when delivering the files.

Never call a single-layer composite, a renamed image, or an unverified file a layered PSD.
