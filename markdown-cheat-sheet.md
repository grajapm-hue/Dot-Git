# Edited On : 02-07-26: 9.00pm
# Markdown Syntax → Pronunciation → HTML Cheatsheet
*Built for slide decks + HTML adaptation (marC workflow)*

> **Key idea:** Markdown has **symbols**, not tags. Each symbol compiles into an **HTML tag**. Learn the mapping once → you write `.md`, get HTML for free.

---

## 1. Text Structure

| Markdown | Say it as | Purpose | Becomes (HTML) |
|---|---|---|---|
| `#` | "hash" / "pound" | Heading 1 (title) | `<h1>` |
| `##` | "double hash" | Heading 2 (section) | `<h2>` |
| `### … ######` | "triple hash"… | Heading 3 to 6 | `<h3>`–`<h6>` |
| `paragraph` | — | Body text | `<p>` |
| blank line | "blank line" | Splits paragraphs | new `<p>` |

---

## 2. Inline Styling

| Markdown | Say it as | Purpose | Becomes |
|---|---|---|---|
| `**bold**` | "double asterisk / double star" | Bold | `<strong>` |
| `*italic*` or `_italic_` | "asterisk" / "underscore" | Italic | `<em>` |
| `***both***` | "triple asterisk" | Bold + italic | `<strong><em>` |
| `~~strike~~` | "double tilde" | Strikethrough | `<del>` |
| `` `code` `` | "backtick" | Inline code | `<code>` |
| `==highlight==` | "double equals" | Highlight (some flavors) | `<mark>` |

---

## 3. Lists

| Markdown | Say it as | Purpose | Becomes |
|---|---|---|---|
| `- item` / `* item` | "dash" / "star / bullet" | Bullet list | `<ul><li>` |
| `1. item` | "number dot" | Numbered list | `<ol><li>` |
| `- [ ]` / `- [x]` | "dash bracket" | Checkbox / task | `<input type="checkbox">` |
| `  - nested` | "indent dash" | Sub-item | nested `<ul>` |

---

## 4. Blocks

| Markdown | Say it as | Purpose | Becomes |
|---|---|---|---|
| `> quote` | "greater-than" / "angle bracket" | Blockquote / callout | `<blockquote>` |
| ` ```lang ` … ` ``` ` | "triple backtick / fence" | Code block | `<pre><code>` |
| `---` | "triple dash / three dashes" | Divider **or slide break** | `<hr>` |
| `\| col \| col \|` | "pipe" | Table | `<table>` |

---

## 5. Links & Media

| Markdown | Say it as | Purpose | Becomes |
|---|---|---|---|
| `[text](url)` | "bracket paren" | Hyperlink | `<a href>` |
| `![alt](url)` | "bang bracket paren" | Image | `<img>` |
| `<https://url>` | "auto-link" | Bare clickable link | `<a href>` |

---

## 6. Slide-Presentation Specific
*(for Marp, Slidev, reveal.js)*

| Markdown | Say it as | Purpose |
|---|---|---|
| `---` | "three dashes" | **New slide** (the #1 one to know) |
| `---` *(at very top)* | "front matter" | YAML config block (theme, etc.) |
| `<!-- comment -->` | "comment tag" | Speaker notes / hidden comment |
| `<!-- _class: lead -->` | "directive" | Per-slide styling (Marp) |

**Front matter example (Marp):**
```
---
marp: true
theme: default
paginate: true
---
```

---

## 7. The HTML Bridge

Markdown lets you drop **raw HTML tags directly** into a `.md` file. This is your "HTML adaptation" escape hatch — use it when Markdown can't do something:

```html
<div align="center">
  <img src="logo.svg" width="120">
  <h1>marC</h1>
</div>

<br>  <!-- "break tag" = line break -->
&nbsp; <!-- "ampersand nbsp" = non-breaking space -->
```

| Tag | Say it as | Purpose |
|---|---|---|
| `<br>` | "break tag" | Line break |
| `<div>` | "div tag" | Container / layout box |
| `<span>` | "span tag" | Inline wrapper for styling |
| `<!-- -->` | "comment tag" | Hidden note |
| `&nbsp;` | "ampersand n-b-s-p" | Non-breaking space |

---

## 8. Tools That Turn `.md` Into Slides / HTML

| Tool | What it does |
|---|---|
| **Marp** | `.md` → slides (PDF/HTML/PPTX). `---` = new slide |
| **Slidev** | Dev-focused slides, Vue + Markdown |
| **reveal.js** | HTML presentations, supports Markdown |
| **Pandoc** | Universal converter: `.md` → pptx / pdf / html / docx |

---
*Pro tip: write your deck once in `.md`, then export to both slides (Marp) and a webpage (Pandoc → HTML). One source, two outputs.*
