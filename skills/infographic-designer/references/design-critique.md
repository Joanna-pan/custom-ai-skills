# Design Critique And Conscious Experiments

Use this procedure to make material design reasoning explicit without turning every visual choice into a debate. A conscious experiment is a testable departure from a safe conventional solution, not permission to excuse novelty or defects.

## When To Use It

Use design critique when at least one condition applies:

- Concept-first work contains a material choice in composition, metaphor, hierarchy, reading path, density, or visual language.
- The standard structure communicates the content poorly or leaves an important goal unmet.
- The user requests an unusual, exploratory, expressive, or comparative direction.
- A proposed deviation could materially improve comprehension, orientation, recall, or engagement but also introduces a real tradeoff.

Keep quick, low-risk work on the normal workflow unless the user explicitly requests exploration. For a user-directed concept, critique only a material risk or proposed deviation; do not use critique to silently replace the user's controlling concept.

## Invariants

Never treat these as experimental variables:

- factual accuracy, source fidelity, units, scales, and caveats;
- legibility, sufficient contrast, and essential accessibility;
- an unambiguous reading path when sequence matters;
- the distinction between measured data, schematic relationships, and decoration;
- required output dimensions, editable structure, and delivery constraints.

If a direction violates an invariant, correct or reject it. Do not defend a production defect as creative intent.

## Pre-Production Critique

1. Define the safe baseline: the clearest conventional solution that satisfies the brief.
2. State why the baseline may be insufficient for this communication goal.
3. Complete the experiment card before production:
   - **Departure:** the familiar solution or rule being changed.
   - **Problem:** what the baseline does not solve well enough.
   - **Hypothesis:** the observable communication improvement expected.
   - **Expected benefit:** comprehension, orientation, recall, engagement, or another named outcome.
   - **Risks and tradeoffs:** what may become worse.
   - **Verification:** the artifact inspection, comparison, usability check, or other evidence that will test the hypothesis.
   - **Rollback condition:** the result that sends production back to the baseline.
4. Present the baseline and experimental direction at concept level; full production of both is unnecessary unless comparison requires it.
5. Obtain approval before producing a material experimental departure. Approval confirms permission to test, not proof that the experiment works.

The experiment card is complete when the hypothesis can fail and the rollback condition is observable.

## Post-Render Critique

Inspect the real artifact at target size, thumbnail size, and its intended publication context. Answer briefly:

1. What communication task does the result solve?
2. What is perceived in the first few seconds?
3. What reading path follows?
4. Which material choices follow established practice?
5. Which choice was experimental?
6. Did the declared verification support the hypothesis relative to the baseline?
7. What remains a subjective judgment requiring human review?

Choose exactly one outcome:

- **Accept:** evidence supports the hypothesis and all invariants pass.
- **Revise:** the hypothesis remains plausible, but a bounded correction and another check are required.
- **Reject:** evidence does not support the hypothesis, a rollback condition occurred, or an invariant failed; use the baseline or a new approved concept.

Do not create a justification after production for an undeclared deviation. Treat it as an ordinary design choice or a defect, then assess it honestly.

## Persistence And Learning

- Store the approved experiment card and its outcome beside the artifact or in the task's production record.
- Add a `decisions.md` entry only when accepting or rejecting the direction materially affects the result, establishes a reusable criterion, changes the workflow, or is likely to guide future work. Record the baseline, alternative, rationale, evidence, consequences, and review trigger.
- Add a `failures.md` entry only for an acknowledged defect or failed process with meaningful impact and a concrete prevention measure. A rejected concept is not automatically a failure.
- Link related `DEC-*` and `FAIL-*` records when a defect changes the design rule or an accepted decision addresses a failure.
- Promote a pattern to best practice only after evidence from the current result or repeated results supports it. Keep unresolved taste disagreements marked as subjective rather than converting them into rules.

The critique is complete when the outcome, evidence, persistence target, and any human-review question are explicit.
