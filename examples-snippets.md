## HTML Table with Color Font Inline Styles

| Product | Price | Stock |
| --- | --- | --- |
| Laptop | $999 | 12 |
| Monitor | $250 | 8 |
| Keyboard | $45 | 25 |

---

## `HTML Table with Inline Styles`

| `Product` | `Price` | `Stock` |
| --- | --- | --- |
| `Laptop` | `$999` | `12` |
| `Monitor` | `$250` | `8` |
| `Keyboard` | `$45` | `25` |

---

# `Markdown Table Wrapping Examples`

`Standard Markdown pipe tables do not support automatic text wrapping based on column width. The text will typically expand the column unless it hits a screen edge. Below are the two best ways to force wrapping.`

## 1. Using \\

for Manual Line Breaks

This is the most compatible way to force wrapping in standard Markdown viewers.

| Item | Description | Item | Description |
| --- | --- | --- | --- |
| Project A | This is a short description. | Project B | This is a short description. |
| Project C | This is a long description that \\ has been manually forced to \\ wrap using the \\ tag. | Project D | This is a long description that \\ has been manually forced to \\ wrap using the \\ tag. |

---

---

## 9. DotMd Sanitizer Test — check preview and tick results

**T0 — Baseline pipe table (no HTML). Should render as a normal table.**

| Col A | Col B |
| --- | --- |
| short | wrap wrap wrap wrap \\ wrap wrap wrap\\ wrap wrap wrap\\ wrap wrap wrap wrap |

---

**T1 — **\\ **inside a pipe cell. PASS = two lines in one cell.**

| Col A | Col B |
| --- | --- |
| break test | line one\\ line two |

---

**T4 — HTML table, legacy **`width`** attribute **`only`**. PASS = T4 text wraps narrow.**

| T4.1 wrap wrap wrap wrap wrap wrap wrap wrap wrap wrap | T4.2-control rest of width | T4.3 wrap wrap wrap wrap wrap wrap wrap wrap wrap wrap | T4.4-control rest of width |
| --- | --- | --- | --- |

---

| T5 wrap wrap\\ wrap wrap wrap \\ wrap wrap\\ wrap wrap wrap | T5-control rest of width |
| --- | --- |

---

**Pattern 3 — **`colgroup`** **`Fixed`** **`column`** **`width`** attribute**

| This column 1 is fixed at 100px and text wraps here | This column 2 \\ takes the \\ wrap \\ remaining width | This column 3 is fixed at 120px and text wraps here |
| --- | --- | --- |

xxxxx

---

xxxxx

---

| <u>Colum 1</u> | <u>Colum 2</u> | <u>Colum 3</u> |
| --- | --- | --- |
| AAAA | AAAA | AAAA |
| AAAA | AAAA | AAAA |
| AAAA | AAAA | AAAA |
| AAAA | AAAA | AAAA |

---

xxxx

---

| A | B | C |
| --- | --- | --- |
| Joahn | 2500 | New York |
| Mary | 30 | London |
| John | 25 | New York |
| Mary | 30 | London |

---

## HTML Table with Color Font Inline Styles

| Product | Price | Stock |
| --- | --- | --- |
| Laptop | $999 | 12 |
| Monitor | $250 | 8 |
| Keyboard | $45 | 25 |

---

---

