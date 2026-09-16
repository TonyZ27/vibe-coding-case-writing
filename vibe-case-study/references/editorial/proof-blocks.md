# Evidence Callouts

An evidence callout is an evidence-backed claim, rendered as one large visual panel. It is not an `At a Glance`, metric strip, or stack of labeled cards. A case may use several callouts when each marks a different consequential turn in the story.

The reference treatment is a full-width tinted panel with generous padding, rounded corners, large sentence-scale typography, and one short phrase in bold. This skill defines the content and presentation intent; the portfolio implementation owns exact colors, spacing, and CSS.

## Narrative job

The statement should connect three things:

1. the surface result or expected interpretation;
2. the stronger behavior, decision, or change underneath it;
3. why that evidence changes how the project should be understood.

A useful pattern is:

> The meaningful result was not [surface output or initial signal]. It was **[stronger proof]**: [why that behavior changes the product, workflow, or ownership].

Do not force that exact sentence shape. Prefer language earned by the current project's causal story.

## Selection hierarchy

Choose the strongest supported statements available. Prefer distinct narrative jobs over repeated versions of the same result:

1. **Second-order adoption:** users teach, invite, contribute, or redistribute without the creator.
2. **Behavioral adoption:** independent or repeat use tied to real work.
3. **Product influence:** use or feedback materially changes product scope or direction.
4. **Outcome:** a task or workflow becomes more coherent, reliable, or possible.
5. **Design insight:** a consequential decision produces a bounded, transferable lesson.
6. **Constraint:** a real technical or product boundary changes the solution.

Higher-ranked evidence is not automatically available. Use only what the current project supports. A set often moves from an initial outcome, to real use, to the influence that use had on the product—but only when each step has its own evidence.

## Evidence eligibility

- **Observed:** eligible when the repository, product, artifact, or receipt directly supports it.
- **Author-reported:** eligible with careful wording and a requested receipt in production notes.
- **Hypothesis:** not eligible for proof styling. Keep it as an ordinary-prose next signal, success criterion, or production-note question.
- **Unsupported:** exclude it.

A source-library pattern can strengthen the interpretation or wording. It cannot supply the current project's facts.

## Public format

Use one unlabeled Markdown blockquote per callout. Do not display `Impact`, `Adoption`, `Insight`, or another category above it.

```markdown
> The strongest signal wasn't the first trial. It was that **designers returned with later builds**—and their next requests pushed the tool beyond fidelity checks.
```

Formatting rules:

- Write one to three sentences, usually 25–65 words.
- Bold one phrase of roughly two to eight words.
- Do not add a visible label, metric heading, or qualifier row.
- Do not split one statement into several cards or place several callouts back-to-back.
- Keep `At a Glance` as neutral prose or a compact list outside the blockquote.
- Place the callout after the reader has seen the evidence that earns it; do not default it to the hero.

## Production-note specification

```text
Role: Evidence callout
Statement:
Inline emphasis:
Evidence status: Observed | Author-reported
Evidence IDs:
Intended placement:
Originating source pattern: none | [pattern ID]
Visual intent: full-width tinted callout; large text; one inline bold phrase; no visible label
```

## Quantity by length

- **Compact:** one or two callouts. Use two only when a later use or change adds a genuinely different proof point.
- **Standard:** two or three callouts, usually distributed across the project's stages.
- **Expanded:** three or four callouts, each tied to a distinct decision, validation signal, or influence on the product.
- **Practice Note:** zero or one callout; omit it when the evidence supports only a provisional lesson.

These are editorial ranges, not quotas. Use fewer callouts when the evidence is thin; never use more merely to decorate the article.

## Editorial test

Remove the visual treatment and read the statement as ordinary prose. It should still be factual, specific, and consequential. If it merely repeats `At a Glance`, relies on color to feel important, or could belong to any project, rewrite it. If it describes what success might look like rather than what happened, remove proof styling.
