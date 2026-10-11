# Brief And Workflow

## Normalized Brief

The five morphological axes are the creative core, but they sit inside a small production brief:

1. Topic and communication goal.
2. Audience and reading context.
3. Source status: supplied content/data, research required, or conceptual illustration.
4. Reference intent, when a reference is supplied: close match, selected traits, or inspiration only.
5. Topic pattern: preferably one primary and optionally one secondary.
6. Composition: one primary and optionally one local secondary structure.
7. Format and size.
8. Visual style: one primary and optionally one supporting influence.
9. Volume: both item count and depth.
10. Palette or brand constraints, when any.
11. Language, deadline, and required deliverables.

Do not demand all eleven fields. Infer defaults when the consequence is reversible. Ask when audience, format, factual basis, confidentiality, or a major structural ambiguity blocks responsible production.

## Interaction Mode Router

Infer one of three modes from natural language; do not require the user to learn commands.

Use **quick infographic mode** when most of these are true:

- The visual contains roughly 2-8 short nodes.
- The content is supplied or non-factual.
- There is one reading path and one hierarchy level.
- The chosen composition obviously fits the information.
- No regulated, medical, legal, financial, or safety-critical claim is involved.
- The user requests a result without discussion.

Expected outcome: one finished, inspected direction without an approval pause. Persist the final artifact and a compact note of material inferred choices.

Use **concept-first mode** when any high-impact condition applies:

- A business or technical process has branches, roles, dependencies, exceptions, or feedback loops.
- The content requires research, reconciliation, or numerical validation.
- There are multiple levels, sections, audiences, or publication surfaces.
- The requested composition conflicts with the information shape.
- The infographic is dense enough that pagination or a carousel may be better than one canvas.
- The user asks for concepts, alternatives, or art direction.
- A promising direction intentionally departs from a familiar composition, metaphor, hierarchy, density, or visual language and therefore needs an explicit hypothesis and comparison with a safe baseline.

Expected outcome: an approved concept followed by the finished artifact. Persist the approved concept card as the decision record for production and revisions.

Use **user-directed concept mode** when the user supplies a structure, sketch, wireframe, layout, ordering, or explicit art direction. Preserve the user's sequence, hierarchy, and emphasis. Do not silently redesign it. Propose a deviation only when the concept creates a comprehension, factual, accessibility, or production problem; name the issue and the smallest viable correction before applying it.

Expected outcome: a faithful production of the user's concept with any approved deviations recorded alongside the artifact. The supplied concept remains the source of truth for later revisions.

Complexity is a routing signal rather than a separate mode. Dense, researched, high-stakes, or structurally ambiguous work normally uses concept-first mode; when the user has already provided the controlling concept, use user-directed concept mode and add only the validation needed to make it safe and workable.

## Concept-First Sequence

1. Restate the normalized brief and mark inferred values.
2. Build a content outline and identify unresolved factual gaps.
3. Present a compact concept card containing:
   - Main idea.
   - Information structure.
   - Reading path.
   - Key emphasis.
   - Composition.
   - Expected density.
   - Risks or unresolved constraints.
   - For a conscious experiment, the standard solution being departed from, communication hypothesis, expected benefit, risks, verification method, and rollback condition from [design-critique.md](design-critique.md).
4. When alternatives would materially improve the decision, propose 2-3 viable directions using:
   - **Рекомендую**
   - **Почему**
   - **Альтернативы**
   - **Риски**
   - **Когда выбрать**
5. For each direction, name the primary composition, reading path, style, palette character, and expected density.
6. Pause for approval.
7. Persist the approved concept card as the production decision record.
8. Produce the requested artifact and export.
9. Run visual and factual QA; when an experiment was approved, compare the rendered result with the baseline and pre-production hypothesis, then record `accept`, `revise`, or `reject` with evidence.

## Quick Infographic Sequence

1. Infer missing low-risk choices.
2. Build one concise information hierarchy.
3. Produce one visual direction without an approval pause.
4. Render and inspect.
5. Deliver the artifact and a compact note listing inferred choices.

## User-Directed Concept Sequence

1. Restate the supplied structure, sequence, and key emphasis briefly enough to catch misinterpretation.
2. Check the concept for factual, comprehension, accessibility, and production blockers.
3. If no blocker exists, produce directly. If one exists, propose the smallest correction and wait only when it materially changes the user's concept.
4. Record approved deviations; otherwise preserve the concept unchanged.
5. Render, inspect, and deliver the requested artifact.

## Semantic Economy And Two-Level Reading

- Every content block and decorative element must improve comprehension, orientation, emphasis, or recall. Do not add sections merely to fill the canvas.
- The first viewing level must reveal the title, central takeaway, and most important facts within a quick scan.
- The second level may use elegant illustration, environmental detail, or secondary annotations that reward close inspection.
- Reserve clear information zones so essential text cannot disappear into rich visual detail.
- Decorative detail must support the subject and reading path rather than compete with labels or create false data cues.

## Output Contract

Default deliverable:

- Verified `.png` export at the requested or inferred dimensions.
- For homework, coursework, and ordinary one-off infographics, deliver only PNG unless the user requests another format or the brief explicitly requires editability.
- Add a source list and structured long description for researched or complex factual work when needed; these may be sidecar documents rather than extra graphic formats.

Optional outputs:

- Editable `.pptx` source when the user requests slide-based editing or presentation delivery.
- Genuine layered `.psd` with logical groups and separately editable content when the user explicitly requests Photoshop editing.
- `.pdf` for print or fixed distribution.
- `.svg` for scalable diagrams.
- `.html` for responsive or interactive delivery.
- Production specification and image-generation prompts when rendering tools are unavailable.

Use descriptive filenames with topic, format, and revision. Avoid overwriting an approved version during palette or copy revisions.

If a requested genuine layered PSD cannot be created or verified in the current environment, do not substitute a flattened PSD. Deliver the verified formats that can be produced, explain the exact PSD limitation, and provide separated source assets or a reconstruction specification when useful.
