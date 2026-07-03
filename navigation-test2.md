navigation-test2

# ✅ DotMD-Safe Snippet Pack

**Purpose:** Every snippet here uses pure markdown — no HTML, no `<` characters. **Test method:** Keep master in backup library → open in DotMD → save → sync to GitHub → diff against master. Byte-identical after 2–3 cycles = confirmed safe.

## Quick Navigation

- [Text Styling](#text-styling)
- [Headings and Anchors](#headings-and-anchors)
- [Tables](#tables)
- [Lists and Tasks](#lists-and-tasks)
- [Code](#code)
- [Quotes and Callouts](#quotes-and-callouts)
- [Links and Images](#links-and-images)

---

## Text Styling

**Bold text** and *italic text* and ***bold italic***.

`Inline code` for filenames like `app.md` or commands like `git diff`.

~~Strikethrough~~ for corrections (test this — GFM feature, most editors support it).

==Highlighted text== (test this — works in Markor, not all editors).

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Headings and Anchors

Headings create their own anchors automatically — no HTML `a` tags needed.

Rule: lowercase the heading, replace spaces with hyphens, drop punctuation.

| Heading written | Link to it |
| --- | --- |
| `## Project Data` | `Go` |
| `## Important Note` | `Go` |
| `## Q3 Bug List!` | `Go` |

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Tables

Basic table:

| Feature | Status | Notes |
| --- | --- | --- |
| Sync | ✅ Pass | Clean round trip |
| Folders | ❌ Bug | Delete fails |
| Anchors | ⚠️ Test | Pending |

Aligned columns:

| Left | Center | Right |
| --- | --- | --- |
| a | b | c |

Visual emphasis inside cells — use bold, code, emoji instead of color:

| Priority | Item |
| --- | --- |
| 🔴 **High** | Folder deletion bug |
| 🟡 **Medium** | File count mismatch |
| 🟢 **Low** | Emoji rendering |

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Lists and Tasks

- Bullet item
- Another item

- Nested item - Deeper nest

1. Numbered step
2. Second step

1. Sub-step

Task list (great for bug trackers):

- \[x\] Documented sync bug
- \[x\] Backed up snippet library
- \[ \] Run isolation test
- \[ \] File consolidated report

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Code

Inline: run `git log --oneline` to see commits.

Fenced block with language:

```bash
git diff HEAD~1 -- SpanStyle-Nav-Demo.md
```

```markdown
# Example markdown inside a code block
**This renders as literal text — safe way to show syntax**
```

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Quotes and Callouts

> Simple blockquote for notes.

> **⚠️ Warning:** Bold plus emoji inside a blockquote replaces a styled div callout.

> **💡 Tip:** Nest formatting freely —
>
> - lists work inside quotes
>
> - so does `code`

Horizontal rule as a section divider:

---

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Links and Images

Plain link: [DotMD site](https://app.md)

Reference-style link: \[my repo\]\[repo\]

\[repo\]: https://github.com/example/example

Image from relative path (test with your Assets folders):



![Sample image](Assets/ImageAst/sample.png)

Image that is also a link:



![Alt text](Assets/ImageAst/sample.png)

[Back to Top](#-dotmd-safe-snippet-pack)

---

## Round-Trip Test Log

| Snippet section | Cycle 1 | Cycle 2 | Cycle 3 | Verdict |
| --- | --- | --- | --- | --- |
| Text styling | ? | ? | ? |  |
| Anchor links | ? | ? | ? |  |
| Tables | ? | ? | ? |  |
| Task lists | ? | ? | ? |  |
| Code blocks | ? | ? | ? |  |
| Blockquote callouts | ? | ? | ? |  |
| Images | ? | ? | ? |  |

