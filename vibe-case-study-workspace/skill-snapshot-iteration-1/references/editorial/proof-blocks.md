# Proof Blocks

Proof blocks are editorial callouts that make a small number of key impacts or insights scannable. This skill specifies their content and meaning in platform-neutral Markdown; the publishing system may map block types to colors later.

## Block types

| Type | Purpose | Suitable content |
| --- | --- | --- |
| **Impact** | Show a concrete change | `5 tools -> 1 workspace` |
| **Adoption** | Show verified use behavior | `10+ designers in facilitated trials` |
| **Influence** | Show how use changed the product | `Requests expanded the tool into design validation` |
| **Insight** | Surface an earned product or build principle | `Detect automatically; curate deliberately` |
| **Constraint** | Make a decisive boundary visible | `Browser decoding required a matching scrcpy stream` |
| **Next signal** | Name a hypothetical success criterion without claiming it happened | `The next test is whether returning users bring others into the workflow` |

## Content specification

Record every block in production notes with:

```text
Type:
Statement:
Optional qualifier:
Evidence status: Observed | Author-reported | Hypothesis
Evidence ID:
Intended placement:
Originating source pattern: none | [pattern ID]
```

Unsupported candidates do not become proof blocks.

## Evidence rules

- Place the block next to the paragraph or visual that supports it.
- Use a number only when its basis is known.
- Attribute author-reported claims in prose or production notes.
- Use Hypothesis only with **Next signal**, or with an Insight that does not imply the outcome occurred.
- Do not label interest as adoption or output as impact.
- Keep each block to one statement and, if needed, one short qualifier.
- Avoid generic principles that could belong to any project.

## Quantity by length

- **Compact:** one or two blocks.
- **Standard:** two or three blocks.
- **Expanded:** three or four blocks across the article.

Do not stack all blocks at the top if an insight only becomes meaningful later.

## Public Markdown format

```markdown
> **Impact**
> **5 tools -> 1 workspace**
> APK installation, mirroring, capture, file handling, and audit documentation became one flow.
```

Keep the type label even when the publishing system later adds color, so meaning never depends on color alone.

## Editorial test

Remove the block temporarily. If the surrounding article does not still substantiate an Impact, Adoption, Influence, or Constraint statement, the block is unsupported. If a Next signal reads like a completed result, rewrite it. If the block repeats the adjacent sentence word for word, tighten one of them.
