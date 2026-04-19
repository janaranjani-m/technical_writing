# Markdown Syntax Guide (Basic to Advanced)

This guide covers practical Markdown syntax for writing high-quality documentation.

## 1. Basics

### Headings

Use # symbols for headings.

```md
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

### Paragraphs

Write normal text separated by a blank line.

```md
This is paragraph one.

This is paragraph two.
```

### Line Breaks

Use two spaces at end of line, or use <br>.

```md
Line one.  
Line two.

Line one.<br>
Line two.
```

### Emphasis

```md
*Italic* or _Italic_
**Bold** or __Bold__
***Bold Italic***
~~Strikethrough~~
```

### Horizontal Rule

```md
---
```

---

## 2. Lists

### Unordered List

```md
- Item A
- Item B
  - Sub-item B1
  - Sub-item B2
```

### Ordered List

```md
1. First
2. Second
3. Third
```

### Task List (GitHub Flavored Markdown)

```md
- [x] Completed task
- [ ] Pending task
```

---

## 3. Links and Images

### Inline Link

```md
[OpenAI](https://openai.com)
```

### Link with Title

```md
[OpenAI](https://openai.com "OpenAI Home")
```

### Reference Link

```md
[Project Docs][docs]

[docs]: https://example.com/docs
```

### Automatic URL

```md
<https://example.com>
```

### Image

```md
![Alt text](images/diagram.png)
```

### Image with Title

```md
![Architecture](images/arch.png "System Architecture")
```

---

## 4. Code

### Inline Code

```md
Use the `npm run build` command.
```

### Fenced Code Block

Use triple backticks and language hint.

```md
```python
print("Hello, world")
```
```

### Indented Code Block

```md
    This is an indented code block.
```

---

## 5. Quotes and Callouts

### Blockquote

```md
> This is a quote.
```

### Nested Blockquote

```md
> Outer quote
>> Inner quote
```

### Note-style Callout (common docs style)

```md
> Note: Save your work before running migrations.
```

---

## 6. Tables

```md
| Feature | Status | Notes |
|---------|--------|-------|
| Login   | Done   | Stable |
| Billing | WIP    | In QA |
```

Alignment:

```md
| Left | Center | Right |
|:-----|:------:|------:|
| A    | B      | C     |
```

---

## 7. Escaping and Special Characters

### Escape Markdown Characters

Use backslash.

```md
\*Not italic\*
\# Not a heading
```

### HTML Entities

```md
&copy; 2026
&lt;div&gt;
```

---

## 8. Advanced GitHub Flavored Markdown

### Footnotes

```md
This has a footnote.[^1]

[^1]: Footnote text.
```

### Collapsible Section

```md
<details>
  <summary>Click to expand</summary>

  Hidden details go here.
</details>
```

### Highlighted Diff

```md
```diff
- old line
+ new line
```
```

### Mention and Issue References (platform-specific)

```md
@username
#123
owner/repo#456
```

### Emoji (platform-specific)

```md
:rocket: :white_check_mark:
```

---

## 9. Mixed Markdown + HTML

Markdown allows inline HTML in many renderers.

```md
<p align="center"><b>Centered bold text</b></p>
```

Useful tags in docs:

- `<br>` for line breaks
- `<kbd>` for keyboard keys
- `<sub>` and `<sup>` for scientific/technical docs

Example:

```md
Press <kbd>Ctrl</kbd> + <kbd>S</kbd>.
H<sub>2</sub>O and x<sup>2</sup>
```

---

## 10. Documentation Writing Patterns

### Section Template

```md
## Feature Name

### Overview
Short explanation.

### Prerequisites
- Item

### Steps
1. Step one
2. Step two

### Expected Result
What should happen.

### Troubleshooting
- Problem: ...
- Solution: ...
```

### API Endpoint Template

```md
## GET /users/{id}

### Description
Returns one user.

### Request
| Field | Type | Required | Description |
|-------|------|----------|-------------|
| id    | path | Yes      | User ID |

### Response
```json
{
  "id": 1,
  "name": "Alice"
}
```
```

---

## 11. Best Practices

- Use heading hierarchy correctly (do not skip levels unnecessarily).
- Keep lines readable and sections short.
- Use lists for steps and scanning.
- Always include alt text for images.
- Add language hints for code blocks.
- Keep table columns concise.
- Use consistent terminology.
- Add examples near each concept.
- Validate links periodically.

---

## 12. Common Mistakes to Avoid

- Missing blank line before or after lists and code blocks.
- Inconsistent heading levels.
- Very large paragraphs without structure.
- Broken relative links.
- Using screenshots without explanatory text.

---

## 13. Quick Cheat Sheet

```md
# Heading 1
## Heading 2
**bold** *italic* ~~strike~~
- bullet
1. numbered
[link](https://example.com)
![img](path/image.png)
`inline code`
```js
console.log("code block")
```
> quote
| a | b |
|---|---|
| 1 | 2 |
- [ ] task
```

---

## 14. Practice Exercises

1. Create a README with title, intro, install steps, and usage.
2. Add a table of features with status.
3. Add one image with alt text.
4. Add one code block with syntax highlight.
5. Add one troubleshooting section with bullet points.

---

## 15. Useful References

- CommonMark Spec: https://spec.commonmark.org/
- GitHub Flavored Markdown: https://github.github.com/gfm/
- Markdown Guide: https://www.markdownguide.org/
