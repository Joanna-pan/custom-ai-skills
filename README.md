# Infographic Designer Skill

**Infographic Designer** is a reusable skill for OpenClaw, Codex, and compatible AI agents. It helps turn a topic, source material, data, or a visual reference into a truthful, readable, compositionally coherent static infographic.

The skill covers the full workflow: brief normalization, information structure, composition choice, visual production, typography checks, design critique, and verified delivery formats.

## Who It Is For

- Designers and art directors
- Editors and content teams
- Educators and students
- Researchers and analysts
- Presentation, poster, and learning-material authors
- Agent users who need a repeatable infographic workflow rather than one-off image generation

## What The Skill Does

### Structures The Brief

The workflow identifies:

- topic and communication goal;
- audience and reading context;
- main takeaway;
- facts, arguments, stages, and explanations;
- composition and reading path;
- format, density, visual style, and delivery requirements.

It uses a five-axis morphological model:

1. content pattern;
2. composition;
3. format and size;
4. visual style;
5. volume and depth.

### Chooses The Right Interaction Mode

The skill supports three modes:

- **Quick infographic** - one inspected version for a simple, low-risk request.
- **Concept first** - concept card, alternatives, risks, and approval before production for complex or uncertain material.
- **User-directed concept** - faithful execution of a user-supplied structure, sketch, layout, or art direction.

### Selects Composition By Meaning

The workflow distinguishes comparisons, processes, timelines, hierarchies, cycles, causal chains, systems, maps, ratings, anatomy views, and other information patterns.

Composition is selected from the relationships in the content, not from decorative appeal alone.

### Handles Visual References

When a visual reference is supplied, the skill clarifies how closely to follow it:

- close match;
- selected traits only;
- inspiration only.

This separates palette, materials, lighting, typography character, and composition from literal image copying.

### Supports Hybrid Production

Precise information design is handled with layout, vector, chart, and presentation tools:

- grids;
- typography;
- diagrams;
- labels;
- connectors;
- numeric values.

Expressive visual layers may use genuine image-generation models for:

- illustrative scenes;
- dimensional objects;
- collage;
- paper cut;
- material textures;
- photorealism;
- lighting and depth.

Critical text, numbers, legends, and labels should not be baked into generated imagery. They are added separately and remain exact.

## Design Critique And Conscious Experiments

For unusual or experimental directions, the skill uses a testable design-critique procedure.

Before production it records:

- safe baseline;
- baseline problem;
- proposed departure;
- hypothesis;
- expected benefit;
- risks and tradeoffs;
- verification method;
- rollback condition.

After rendering, the experiment receives one of three outcomes:

- **Accept** - the hypothesis is supported and all invariants pass.
- **Revise** - the idea remains plausible but needs a bounded correction.
- **Reject** - the hypothesis is unsupported or an invariant failed.

Experimental design cannot justify factual errors, poor readability, weak contrast, or an unclear reading path.

## Quality Checks

The skill checks the rendered artifact, not only the prompt or source file.

Core checks include:

- factual accuracy and source consistency;
- clear main takeaway;
- reading path;
- composition-content fit;
- no clipped or overlapping text;
- text bounds inside containers on both axes with padding;
- consistent type size, weight, and line-height for blocks with the same semantic role;
- readability at target size;
- thumbnail hierarchy;
- contrast and accessibility;
- no generation artifacts;
- clean edges and transparency when assets are composited;
- parity across requested formats.

## Supported Outputs

Default:

- verified `PNG` at the requested or inferred dimensions.

When requested and supported by the runtime workflow:

- editable `PPTX`;
- genuine layered `PSD`;
- `PDF`;
- `SVG`;
- `HTML`;
- image series and carousels;
- production specifications and prompts for visual layers.

## Important PSD And PPTX Limits

Supported output names do not guarantee that every runtime can create them.

`PPTX` should be produced only when the environment can create and independently verify an editable presentation.

`PSD` should be produced only when the environment can create a genuine layered Photoshop document. A valid PSD deliverable should:

- open as a PSD;
- contain multiple meaningful named layers or groups;
- preserve editable text when the workflow supports it;
- match the approved PNG;
- pass a separate layer-structure inspection.

A flattened image saved with a `.psd` extension is not a layered PSD and should never be presented as one.

If a requested workflow is unavailable, the agent should state the limitation and provide a verified alternative such as PNG, separated assets, PPTX, SVG, or a reconstruction specification.

## Limitations

- This skill is not a replacement for a dedicated chart workflow for ordinary single charts.
- Output quality depends on available image models, renderers, fonts, and export tools.
- Expressive styles such as 3D, paper cut, collage, or material rendering require a genuine image-generation model. Programmatic pseudo-3D or SVG imitation is not an equivalent substitute.
- Generated imagery must be inspected: models can create malformed objects, accidental text, or misleading details.
- Facts, statistics, dates, and quotes must be grounded in sources.
- Confidential data should not be sent to external models without permission.
- The skill does not imitate a living artist's distinctive style; requests should be translated into broader visual-language traits.
- Complex compositions may still require human design judgment.

## Installation

This repository stores skills under `skills/<skill-name>/`. Install the `infographic-designer` folder into your agent's skill directory.

### OpenClaw workspace

From a cloned copy of this repository:

```bash
mkdir -p ~/.openclaw/workspace/skills
cp -R skills/infographic-designer ~/.openclaw/workspace/skills/infographic-designer
```

Then start a new session so the agent reloads skills.

### Codex / local skill directory

```bash
mkdir -p ~/.codex/skills
cp -R skills/infographic-designer ~/.codex/skills/infographic-designer
```

The installed skill folder must contain `SKILL.md` at its root.

## Example Requests

```text
Create a vertical 4:5 infographic about the principles of accessible interface design.
Use an editorial style and five concise content blocks.
```

```text
Create an infographic from the attached reference.
Use its palette, materials, and lighting character, but build a different composition.
```

```text
Create a process infographic. First show me the concept card and risks before production.
```

## Project Principles

- Content is more important than decoration.
- Composition should match the structure of the information.
- Visual expressiveness does not justify distorted data.
- Critical text should not be embedded inside generated imagery.
- Experiments need a testable hypothesis and rollback condition.
- A deliverable format should not be promised unless it can be created and verified.
- The final artifact should be checked at full size, thumbnail size, and in its intended publication context.

## GitHub About

**English:** OpenClaw/Codex skill for designing, producing, and auditing truthful, readable infographics from topics, data, source material, and visual references.

**Русский:** Skill для создания и проверки инфографики: от брифа и композиции до визуального производства, дизайн-критики и QA.
