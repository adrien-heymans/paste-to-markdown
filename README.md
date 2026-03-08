# 📝 Paste to Markdown

A minimal, instant Paste-to-Markdown converter — paste anything and your Markdown is ready to copy in one keystroke.

**[→ Try it live](https://adrien-heymans.github.io/paste-to-markdown/)**

---

## What it does

Paste plain text, rich text copied from Word, Notion, emails, or websites — it converts instantly and **selects all the output automatically**, so you just press `Ctrl+C` / `⌘C` and you're done.

No buttons to click. No form to submit. Just paste, then copy.

### Conversion support

| Input | Output |
|---|---|
| Headings (H1–H4, ALL CAPS lines, setext) | `#` `##` `###` `####` |
| Bold / italic (rich text) | `**bold**` `_italic_` |
| Bullet lists (`-` `*` `•` `►`) | `- item` |
| Numbered lists | `1. item` |
| Hyperlinks | `[text](url)` |
| Inline code & code blocks | `` `code` `` and ` ```blocks``` ` |
| Blockquotes | `> quote` |
| Tables (from rich text) | `\| col \| col \|` |
| Horizontal rules | `---` |
| URLs & emails (plain text) | `<url>` auto-linked |

---

## How it works

- **Rich text paste** (from Word, Notion, websites): uses the clipboard's `text/html` data and walks the DOM tree to produce clean Markdown
- **Plain text paste**: applies heuristics to detect headings, lists, blockquotes, and inline formatting
- After conversion, `textarea.select()` is called automatically — the result is pre-selected and ready to copy

Zero dependencies. Zero backend. One HTML file.

---

## Run locally

Just open the file — no server needed.

```bash
git clone https://github.com/adrien-heymans/paste-to-markdown.git
cd paste-to-markdown
open index.html
```

---

## Deploy your own

Since it's a single static HTML file, you can host it anywhere.

**GitHub Pages** (what this repo uses)
1. Fork this repo
2. Go to Settings → Pages → Deploy from branch → `main` → `/ (root)`
3. Done — live at `your-username.github.io/paste-to-markdown/`

---

## Design

Built with a **claymorphism** aesthetic — soft pastel backgrounds, frosted glass cards, and pill-shaped UI elements. Fonts: [Syne](https://fonts.google.com/specimen/Syne) + [Nunito](https://fonts.google.com/specimen/Nunito) via Google Fonts.

---

## Author

**Adrien Heymans** — Senior Analyst in Enterprise Architecture, MSc AI, University of Ottawa.

[Portfolio](https://adrien-heymans.github.io) · [LinkedIn](https://www.linkedin.com/in/adrien-heymans/)# paste-to-markdown
