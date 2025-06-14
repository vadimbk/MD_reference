# Full Markdown Syntax Reference

A complete cheat sheet of Markdown formatting, compatible with GitHub Flavored Markdown (GFM).

---

## 📄 Text Formatting

| Markdown | Description | Example | Output |
|----------|-------------|---------|--------|
| `*text*` or `_text_` | *Italic* | `*italic*` | *italic* |
| `**text**` or `__text__` | **Bold** | `**bold**` | **bold** |
| `***text***` | ***Bold & Italic*** | `***bold italic***` | ***bold italic*** |
| `~~text~~` | ~~Strikethrough~~ | `~~struck~~` | ~~struck~~ |
| `` `code` `` | Inline `code` | `` `print()` `` | `print()` |
| `> quote` | Blockquote | `> This is a quote.` | > This is a quote |
| `\*` | Escape special character | `\*not italic\*` | \*not italic\* |

---

## 🧱 Headings

| Markdown | Description | Example | Level |
|----------|-------------|---------|-------|
| `# Heading` | H1 | `# Heading 1` | H1 |
| `## Heading` | H2 | `## Heading 2` | H2 |
| `### Heading` | H3 | `### Heading 3` | H3 |
| `#### Heading` | H4 | `#### Heading 4` | H4 |
| `##### Heading` | H5 | `##### Heading 5` | H5 |
| `###### Heading` | H6 | `###### Heading 6` | H6 |

---

## 🔗 Links and Images

| Markdown | Description | Example | Output |
|----------|-------------|---------|--------|
| `[text](url)` | Hyperlink | `[Google](https://google.com)` | [Google](https://google.com) |
| `[text](url "tooltip")` | Link with tooltip | `[site](https://example.com "tooltip")` | [site](https://example.com "tooltip") |
| `![alt](image.jpg)` | Image | `![img](image.jpg)` | ![img](image.jpg) |
| `<https://url>` | Auto link | `<https://github.com>` | <https://github.com> |

---

## 🔢 Lists
> **Note:** To create nested lists, indent with either **2 spaces, 4 spaces, or a tab** (`\t`). However, for consistent rendering across platforms, using **4 spaces or a tab** is recommended.


### Unordered Lists

```markdown
- Item 1
- Item 2
  - Subitem 2.1
  - Subitem 2.2
```

### Ordered Lists

```markdown
1. First
2. Second
   1. Substep
   2. Another substep
```

### Mixed Nested

```markdown
- Main
  1. Numbered inside bullet
  2. Another one
- Another Main
```

---

## 📋 Code

| Markdown | Description | Example | Output |
|----------|-------------|---------|--------|
| `` `code` `` | Inline code | `` `ls -la` `` | `ls -la` |
| <pre>```language<br>code block<br>```</pre> | Code block with syntax | ```bash<br>echo "hi"<br>``` | Syntax-highlighted |
| 4 spaces indent | Old-style code block |     indented line | Indented block |

---

## 📐 Tables
> **Tip:** Tables must begin with a header row, followed by a separator row using `-` and optional colons (`:`) for alignment:
> - `:---` for left-aligned
> - `:---:` for center-aligned
> - `---:` for right-aligned
>
> Table rows should be aligned using `|` between columns. All rows should have the same number of columns for best results.


```markdown
| Header 1 | Header 2 |
|----------|----------|
| Row 1    | Row 2    |
```

With alignment:

```markdown
| Left | Center | Right |
|:-----|:------:|------:|
| A    |   B    |     C |
```

---

## ✅ Task Lists (GFM)

```markdown
- [x] Completed
- [ ] Pending
```

- [x] Completed  
- [ ] Pending

---

## ⚙️ Other

| Markdown | Description | Example | Output |
|----------|-------------|---------|--------|
| `---` or `***` | Horizontal rule | `---` | --- |
| `<br>` | Line break | `Line 1<br>Line 2` | Line 1<br>Line 2 |
| `<span style="color:red">text</span>` | HTML in Markdown | if supported | HTML element |

---

## 💡 Notes

- GFM (GitHub Flavored Markdown) supports tables, task lists, and syntax highlighting.
- Use inline HTML sparingly to maintain compatibility.
---

## 🔢 Lists
> **Note:** To create nested lists, indent with either **2 spaces, 4 spaces, or a tab** (`\t`). However, for consistent rendering across platforms, using **4 spaces or a tab** is recommended.
 — Details and Pitfalls

### Key Points:
- You can use `-`, `*`, or `+` for unordered lists — they behave the same.
- For ordered lists, Markdown renders numbers sequentially regardless of what you type.
- **Indentation matters**: use **2 or 4 spaces**, or **1 tab**, for nested levels.

### Best Practices:
- Use **consistent indentation** (prefer 2 or 4 spaces, not mixed).
- GitHub supports both **tabs** and **spaces**, but spaces are safer for cross-platform rendering.

```markdown
1. Main item
   - Subitem (2 spaces)
     - Sub-subitem (4 spaces)
```

---

## 📐 Tables
> **Tip:** Tables must begin with a header row, followed by a separator row using `-` and optional colons (`:`) for alignment:
> - `:---` for left-aligned
> - `:---:` for center-aligned
> - `---:` for right-aligned
>
> Table rows should be aligned using `|` between columns. All rows should have the same number of columns for best results.
 — Markdown Style

Tables are defined using pipes `|` and dashes `-`.

### Basic Table

```markdown
| Column 1 | Column 2 |
|----------|----------|
| Data A   | Data B   |
| Data C   | Data D   |
```

Output:

| Column 1 | Column 2 |
|----------|----------|
| Data A   | Data B   |
| Data C   | Data D   |

### Aligned Table

```markdown
| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| A          |     B        |           C |
| D          |     E        |           F |
```

Output:

| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| A          |     B        |           C |
| D          |     E        |           F |

- `:---` = left align
- `:---:` = center align
- `---:` = right align
