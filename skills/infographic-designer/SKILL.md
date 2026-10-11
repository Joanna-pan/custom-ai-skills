---
name: infographic-designer
description: Design, create, revise, and audit static infographics from a topic, source material, data, or a five-axis morphological brief. Use for visual explainers, process maps, timelines, comparisons, posters, carousels, and PNG/PPTX/layered PSD deliverables. For a single ordinary chart without an infographic narrative, prefer a dedicated chart workflow.
---

# Infographic Designer

Turn information into a truthful, readable, compositionally coherent infographic. Treat the user's morphological choices as art direction, not as permission to force an unsuitable composition onto the content.

## Defaults

- Work adaptively: infer low-risk missing choices and ask only when a missing answer materially changes meaning, audience, format, or publication constraints.
- Use a modern editorial + data-journalism visual language when no style is specified.
- Deliver a verified `PNG` at the requested or inferred dimensions by default. For homework, coursework, and ordinary one-off infographics, do not create PPTX or PSD unless the user asks for them or the brief explicitly requires an editable source. Add PPTX, genuine layered PSD, PDF, SVG, or HTML only when requested or when the delivery medium requires it.
- Keep information-bearing text, numbers, labels, arrows, and charts editable. Use image generation for illustration, texture, objects, scenes, or backgrounds rather than for final body text.
- For styles that depend on rendered materials, depth, illustration, paper cut, collage, 3D, photorealism, or similar generated visuals, use `openai/gpt-image-2` when available; otherwise use the best available genuine image-generation model and disclose it. Do not imitate these styles with programmatic SVG, gradients, primitive paths, Sharp, Canvas, or pseudo-3D.
- A flattened image saved with a `.psd` extension is not a layered PSD. Never present it as one.
- Never invent facts, statistics, dates, quotes, sources, or causal claims.

## Route The Work

1. Read [brief-and-workflow.md](references/brief-and-workflow.md) to normalize the request and choose quick, concept-first, or user-directed mode.
2. Read [morphological-matrix.md](references/morphological-matrix.md) when the user wants options, has supplied matrix values, or important axes are missing.
3. Read [composition-selection.md](references/composition-selection.md) before choosing or validating the spatial structure.
4. Read [design-critique.md](references/design-critique.md) when concept-first work includes a material design choice, when a standard structure appears insufficient, or when the user asks for an unusual, exploratory, or experimental direction.
5. Read [production-method.md](references/production-method.md) whenever creating visual assets, working from a reference image, choosing a generation method, or using a rendered, illustrative, material, dimensional, paper cut, collage, 3D, or photoreal style.
6. Read [style-recipes.md](references/style-recipes.md) when building an art direction, production prompt, or one of the user's recurring styles.
7. Read [content-and-sources.md](references/content-and-sources.md) whenever facts, research, statistics, quotations, or supplied source material are involved.
8. Read [color-system.md](references/color-system.md) when choosing, presenting, or revising a palette.
9. Read [psd-delivery.md](references/psd-delivery.md) whenever a layered PSD is requested or required.
10. Read [openclaw-delivery.md](references/openclaw-delivery.md) when the current runtime or destination is OpenClaw WebChat or Control UI.
11. Always use [quality-checklist.md](references/quality-checklist.md) before delivery.

## Core Workflow

### 1. Normalize The Brief

Capture topic and goal, audience, source status, and one or two choices from each axis when useful: topic pattern, composition, format/size, visual style, and volume. Do not make the user complete a form if the request already implies the answer.

### 2. Protect Meaning

Build the information architecture before styling. Separate title, core takeaway, evidence, explanatory nodes, labels, caveats, and sources. For quantitative content, choose encodings that preserve scale and comparison. For a process, make direction, branching, ownership, inputs, and outputs unambiguous. Apply semantic economy: every block, label, illustration, and ornament must improve comprehension, orientation, emphasis, or recall; do not add content merely to fill space.

### 3. Choose The Interaction Mode

- **Quick infographic:** When the request is low-risk, the structure is evident, or the user asks for an immediate result, infer reversible choices, produce one direction, inspect it, and deliver without an approval pause.
- **Concept first:** When the user asks to approve an idea, the content is dense or structurally uncertain, or factual/design risks are material, present a compact concept card before production: main idea, information structure, reading path, key emphasis, composition, expected density, and risks. When alternatives are useful, present them as `Рекомендую -> Почему -> Альтернативы -> Риски -> Когда выбрать`, then pause for approval. If a material departure from the safest conventional solution may improve communication, use the conscious-experiment procedure in [design-critique.md](references/design-critique.md) before production and retain a safe baseline.
- **User-directed concept:** When the user supplies a structure, sketch, layout, or explicit art direction, treat it as the controlling concept. Preserve its sequence, hierarchy, and emphasis; propose deviations only when needed for comprehension, factual integrity, accessibility, or production feasibility, and identify each deviation before applying it.

Infer the mode from the request; never require special command syntax. Complexity is a risk signal, not a fourth mode: it normally routes work to concept-first unless the user has already supplied the controlling concept.

### 4. Produce Deliberately

Use one approved content model for every output. Follow `production-method.md` before creating or accepting generated visual layers, and keep critical copy out of generated imagery. Create two levels of perception: the title, takeaway, and key facts must scan immediately, while supporting illustration and detail may reward closer viewing without competing with the information zones. Build an editable layout when an editable deliverable is requested. Do not bake critical copy into generated imagery. Keep a requested PSD organized into meaningful groups and retain editable text layers when the available workflow supports them. When a required renderer is unavailable, return the deliverables that can be verified plus a precise limitation and production-ready fallback; never claim that a missing or flattened artifact is a layered PSD.

When a request requires multiple generated images or visual directions, run image-generation jobs strictly in sequence. Start the next generation only after the previous job has completed, its output file is readable, and the result has been visually inspected. Do not submit concurrent image-generation jobs for a multi-image request, even when the provider supports batching or parallel calls.

### 5. Inspect The Artifact

Render the real output and inspect it at target size and thumbnail size. Check content, immediate comprehension, deeper detail, reading path, clipping, overlap, typography, contrast, source consistency, and any requested editable structure. For every text-bearing field, compare the rendered text bounds with the container bounds on both axes and include the intended internal padding; resize the container, rewrap the copy, or adjust typography until the complete text fits comfortably. For a conscious experiment, compare the result with its pre-production hypothesis and baseline, then accept, revise, or reject it; never invent the rationale after seeing the output. Check parity only across formats actually requested. Iterate until it passes the checklist.

## Palette Revisions

Treat color as an independent system. If the user asks to change only the palette, preserve approved content, geometry, hierarchy, and style unless contrast or meaning requires a small correction. Show swatches in concept-first work and explain any accessibility adjustment.

## Boundaries

- Do not select a visually impressive structure that misrepresents the information.
- Do not use decorative 3D effects on quantitative charts when depth can distort comparison.
- Do not rely on color alone to carry meaning.
- Do not imitate a living artist's distinctive style; translate the request into broader visual characteristics.
- Do not expose confidential source data to external generation or research services without permission.
