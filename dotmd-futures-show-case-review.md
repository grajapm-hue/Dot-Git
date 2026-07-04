# <span style="color:rgb(255, 0, 0)">DotMD : </span><span style="color:rgb(0, 128, 0)">write in Markdown,</span> <span style="color:rgb(0, 0, 255)">ship anything</span>

# <span style="color:rgb(0, 255, 255)">DotMD</span> <span style="color:rgb(255, 0, 255)">: write in Markdown,</span> <span style="color:rgb(255, 255, 0)">ship anything</span>

# DotMD - write in Markdown, ship anything

*Edit: Saving a new version*

**DotMD** is the markdown-native workspace where your **Docs**, **Slides**, and **Sheets** live in one place — plain text you own, rendered beautifully, powered by AI you control.



![DotMD hero — one workspace for docs, slides and sheets](/samples/hero.jpg)

This document is a *living demo*: every paragraph below is real Markdown you can edit, reformat, and export. Hit the toolbar, toggle a view, and watch the source and the rendered surface stay in lockstep.

---

## Why teams pick DotMD

DotMD treats Markdown as a first-class citizen, not an afterthought. You get the speed of plain text with the polish of a modern editor — and none of the lock-in.

- **Markdown-native** — your content is portable `.md`, readable in any editor, diff-able in any repo.
- **Real-time collaboration** — features multiplayer cursors, comments, and conflict-free synchronization built on CRDTs.

AI with BYOK — bring your own key and edit, summarize, or draft with the model you trust.

- **Agent-native via MCP** — let agents read and write your docs through the Model Context Protocol.
- **Three surfaces, one format** — Docs, Slides, and Sheets that all round-trip to clean Markdown.

### Formatting that just works

Style inline without leaving the keyboard: **bold** for emphasis, *italic* for nuance, ~~strikethrough~~ for edits, <u>underline</u> for headers, <mark>highlight</mark> to draw the eye, and `inline code` for the technical bits. Even footnotes read naturally — E = mc<sup>2</sup> and H<sub>2</sub>O render exactly as you'd expect.

You can chain marks too: a [link to dotmd.co](https://dotmd.co) sits comfortably beside <mark>highlighted</mark> and `code` spans in the same line.

## DotMD vs. the alternati

| Capability | DotMD | Generic docs | Slide tools | Remarks |
| --- | --- | --- | --- | --- |
| Markdown-native | Yes | Partial | No |  |
| Real-time collab | Yes | Yes | Sometimes |  |
| AI with your own key | Yes | No | No |  |
| Agent / MCP access | Yes | No | No |  |
| Export to clean code | Yes | No | No |  |

## A quick taste of the editor

Drop in a fenced code block and DotMD keeps it verbatim — perfect for runbooks, snippets, and docs-as-code:

```bash
# Publish a doc straight from your terminal via MCP
dotmd push ./release-notes.md --workspace acme
```

```ts
// Or call the API with your own model key (BYOK)
const draft = await dotmd.ai.edit(doc, { prompt: 'tighten the intro' });
```

> "We replaced three tools with DotMD and our docs finally match our code."
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
> — A very happy engineering lead

**Pro tip:** paste raw HTML and DotMD renders it inline — callouts, badges, and embeds round-trip through Markdown untouched.



![Collaborate in real time with multiplayer cursors and comments](/samples/collab.jpg)

## The roadmap (you can check these off)

- \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\[x\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\] Markdown-native Docs, Slides, and Sheets
- \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\[x\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\] Real-time collaboration with comments
- \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\[x\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\] BYOK AI editing and summaries
- \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\[ \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\] Native desktop and mobile apps
- \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\[ \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\] Offline-first sync everywhere

Get started in three simple steps:\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\ \\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

1. Create a workspace and invite your team.\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
2. Import existing Markdown or begin with a sample template.\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
3. Enable AI using your own API key and deploy.



![From idea to shipped — DotMD keeps your whole workflow in Markdown](/samples/workflow.jpg)

---

Made with DotMD. Export this Every document to Markdown, PDF, or HTML — your words, your format, anywhere.