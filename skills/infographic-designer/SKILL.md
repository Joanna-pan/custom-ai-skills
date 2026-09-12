---
name: infographic-designer
description: Design, create, revise, and audit static infographics from a topic, source material, data, or a five-axis morphological brief. Use for visual explainers, process maps, timelines, comparisons, posters, carousels, and PNG/PPTX/layered PSD deliverables. For a single ordinary chart without an infographic narrative, prefer a dedicated chart workflow.
---

# Infographic Designer

Turn information into a truthful, readable, compositionally coherent infographic. Treat the user's morphological choices as art direction, not as permission to force an unsuitable composition onto the content.

## Defaults

- Work adaptively: infer low-risk missing choices and ask only when a missing answer materially changes meaning, audience, format, or publication constraints.
- Use a modern editorial + data-journalism visual language when no style is specified.
- Deliver `PNG + PPTX + layered PSD` by default unless the user explicitly opts out of a format. Add PDF, SVG, or HTML when the requested medium benefits from it.
- Keep information-bearing text, numbers, labels, arrows, and charts editable. Use image generation for illustration, texture, objects, scenes, or backgrounds rather than for final body text.
- A flattened image saved with a `.psd` extension is not a layered PSD. Never present it as one.
- Never invent facts, statistics, dates, quotes, sources, or causal claims.

## Route The Work

1. Read [brief-and-workflow.md](references/brief-and-workflow.md) to normalize the request and choose simple or complex mode.
2. Read [morphological-matrix.md](references/morphological-matrix.md) when the user wants options, has supplied matrix values, or important axes are missing.
3. Read [composition-selection.md](references/composition-selection.md) before choosing or validating the spatial structure.
4. Read [style-recipes.md](references/style-recipes.md) when building an art direction, production prompt, or one of the user's recurring styles.
5. Read [content-and-sources.md](references/content-and-sources.md) whenever facts, research, statistics, quotations, or supplied source material are involved.
6. Read [color-system.md](references/color-system.md) when choosing, presenting, or revising a palette.
7. Read [psd-delivery.md](references/psd-delivery.md) whenever producing or revising the default PSD deliverable.
8. Read [openclaw-delivery.md](references/openclaw-delivery.md) when the current runtime or destination is OpenClaw WebChat or Control UI.
9. Always use [quality-checklist.md](references/quality-checklist.md) before delivery.

## Core Workflow

### 1. Normalize The Brief

Capture topic and goal, audience, source status, and one or two choices from each axis when useful: topic pattern, composition, format/size, visual style, and volume. Do not make the user complete a form if the request already implies the answer.

### 2. Protect Meaning

Build the information architecture before styling. Separate title, core takeaway, evidence, explanatory nodes, labels, caveats, and sources. For quantitative content, choose encodings that preserve scale and comparison. For a process, make direction, branching, ownership, inputs, and outputs unambiguous.

### 3. Choose The Interaction Mode

- **Simple / direct:** For a small, low-risk visual or an explicit request such as "без обсуждения", infer the remaining brief, make one concept, render, inspect, and deliver.
- **Complex / collaborative:** For processes, dense or factual material, multiple hierarchy levels, uncertain data, or conflicting choices, propose 2-3 concepts and pause for approval before production. Present them as `Рекомендую -> Почему -> Альтернативы -> Риски -> Когда выбрать`.

### 4. Produce Deliberately

Use one approved content model for every output. Build the editable layout first or in parallel with generated assets. Do not bake critical copy into generated imagery. Keep the PSD organized into meaningful groups and retain editable text layers when the available workflow supports them. When a required renderer is unavailable, return the deliverables that can be verified plus a precise limitation and production-ready fallback; never claim that a missing or flattened artifact is a layered PSD.

### 5. Inspect The Artifact

Render the real output and inspect it at target size and thumbnail size. Check content, reading path, clipping, overlap, typography, contrast, source consistency, layer structure, and parity across PNG, PPTX, and PSD. Iterate until it passes the checklist.

## Palette Revisions

Treat color as an independent system. If the user asks to change only the palette, preserve approved content, geometry, hierarchy, and style unless contrast or meaning requires a small correction. Show swatches for complex work and explain any accessibility adjustment.

## Boundaries

- Do not select a visually impressive structure that misrepresents the information.
- Do not use decorative 3D effects on quantitative charts when depth can distort comparison.
- Do not rely on color alone to carry meaning.
- Do not imitate a living artist's distinctive style; translate the request into broader visual characteristics.
- Do not expose confidential source data to external generation or research services without permission.
