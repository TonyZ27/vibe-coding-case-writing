# Proof Blocks

Proof blocks are colored editorial callouts that make a small number of key impacts or insights scannable. They should amplify evidence already present in the story, not compensate for weak evidence.

## Block types

| Type | Purpose | Suitable content |
| --- | --- | --- |
| **Impact** | Show a concrete change | `5 tools -> 1 workspace` |
| **Adoption** | Show verified use behavior | `10+ designers in facilitated trials` |
| **Influence** | Show how use changed the product | `Requests expanded the tool into design validation` |
| **Insight** | Surface an earned product or build principle | `Detect automatically; curate deliberately` |
| **Constraint** | Make a decisive boundary visible | `Browser decoding required a matching scrcpy stream` |

## Evidence rules

- Place the block next to the paragraph or visual that supports it.
- Use a number only when its basis is known.
- Attribute author-reported claims in prose or production notes.
- Do not label interest as adoption or output as impact.
- Keep each block to one statement and, if needed, one short qualifier.
- Avoid generic principles that could belong to any project.

## Quantity by length

- **Compact:** two or three blocks.
- **Standard:** three or four blocks.
- **Extended:** four to six blocks across the article.

Do not stack all blocks at the top if an insight only becomes meaningful later.

## Semantic Markdown/HTML format

Use semantic HTML when the publishing surface supports styling:

```html
<aside class="proof-block proof-block--impact">
  <p class="proof-block__label">Impact</p>
  <p class="proof-block__statement"><strong>5 tools -> 1 workspace</strong></p>
  <p class="proof-block__note">APK installation, mirroring, capture, file handling, and audit documentation became one flow.</p>
</aside>
```

Recommended visual tokens:

- Impact: warm accent.
- Adoption: cool accent.
- Influence: violet accent.
- Insight: neutral or brand accent.
- Constraint: muted warning accent.

Color is presentation, not meaning. Preserve the label and hierarchy for accessibility, maintain sufficient contrast, and never rely on color alone.

For Markdown-only publishing, use this fallback:

```markdown
> **Impact**
> **5 tools -> 1 workspace**
> APK installation, mirroring, capture, file handling, and audit documentation became one flow.
```

## Editorial test

Remove the block temporarily. If the surrounding article does not still substantiate the statement, the block is unsupported. If the block repeats the adjacent sentence word for word, tighten one of them.
