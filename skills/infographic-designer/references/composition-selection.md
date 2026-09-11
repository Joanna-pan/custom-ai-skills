# Composition Selection

Choose the composition from the information relationship first, then apply visual style.

## Semantic Fit

| Information job | Strong primary choices | Use carefully |
|---|---|---|
| Compare two alternatives | Two columns, split screen, balancing scales, Venn | Radar only for comparable multivariate scales |
| Compare many categories or rank | Ordered bars, table, modular grid, podium | Pie/donut for many categories |
| Sequence or instructions | Vertical/horizontal chain, staircase, zigzag, flowchart | Spiral when exact order must be obvious |
| Time | Chronological strip, Gantt, calendar grid | Decorative paths that obscure dates |
| Cycle or recurrence | Circular cycle, orbital system | Circle when the process actually has a start/end |
| Hierarchy | Tree, pyramid, concentric circles, nested frames | Treemap unless area encodes a real quantity |
| Decision logic | Decision tree, flowchart, 2x2 matrix | Network graph without directional labels |
| Causes and effects | Ishikawa, branching tree, domino chain | Sankey unless flow magnitude is measured |
| Flow of quantities/resources | Sankey, funnel, river with tributaries | Equal-width arrows for unequal amounts |
| Parts of an object/system | Cutaway, anatomy, layered section, object with callouts | Card grid when spatial relationships matter |
| Equal-weight facts | Modular grid, bento, cards, honeycomb | Hierarchical forms that imply rank |
| Relationships/network | Network graph, constellation, metro map | Dense graph without clustering or labels |
| Narrative/case study | Storyboard, route map, chapters, before/after | Dashboard when chronology is the main story |
| KPIs/status | Indicator panel, compact dashboard | Decorative gauges without actionable thresholds |

## Primary And Secondary Structure

When two compositions are selected, name one **primary reading structure** and one **local supporting structure**. The secondary structure must occupy a bounded region and must not create a competing reading path.

Good example: a route map with one compact KPI panel.

Bad example: a Sankey, radial cycle, timeline, and card grid all competing at the same level.

## Quantitative Integrity

- Use position and length for precise comparison before angle, area, volume, or decorative color intensity.
- Preserve zero baselines where omission would exaggerate differences.
- Label units, denominators, time periods, and data scope.
- Do not use 3D perspective for measured bars, pies, areas, or bubbles.
- Distinguish measured data from conceptual or schematic relationships.
- Make uncertainty, missing values, and estimates visible.

## Process Integrity

For a working process, identify start and end states, actors or owners, inputs and outputs, decisions and branch conditions, parallel steps, exceptions, feedback loops, handoffs, and dependencies.

Use consistent arrow semantics. Avoid crossed connectors when regrouping or swimlanes would make the route clearer.

## Density Controls

- If text must be reduced below comfortable reading size, split the canvas or use a carousel.
- Prefer direct labels to distant legends.
- Keep one dominant title, one primary takeaway, and a visible reading order.
- Do not solve excess content by shrinking everything uniformly.
