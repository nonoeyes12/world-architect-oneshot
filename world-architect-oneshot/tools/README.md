# tools/render.py — Campaign Markdown → styled PDF

An optional companion that turns a campaign Markdown file (for example, one produced by the
framework) into a two-column, "aged manuscript" PDF with a cover page, read-aloud boxes, styled
tables, and page numbers.

## Install

```bash
pip install -r requirements.txt
```

WeasyPrint needs its native libraries (Pango/Cairo). On Debian/Ubuntu:
`sudo apt-get install libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev`.
See the WeasyPrint docs for macOS/Windows. For the intended typography, install the free
**TeX Gyre Bonum** / **URW Bookman** fonts; without them the renderer falls back to Georgia/serif.

## Use

```bash
python render.py CAMPAIGN.md -o CAMPAIGN.pdf \
    --title "The Ethereal" \
    --subtitle "Drowned Light & Borrowed Souls" \
    --note "A GM-Ready One-Shot" \
    --footer "For D&D 5e (SRD 5.2)" \
    --theme maroon
```

Options: `--theme {maroon,rust,slate,forest,ink}`, `--running-header "..."`, `--no-cover`,
`--title/--subtitle/--note/--footer`. If `--title` is omitted it uses the first `# ` heading.

## Markdown conventions

| Markdown | Renders as |
|---|---|
| `# Title` | document title (cover only, then skipped) |
| `## Section` | full-width section header |
| `### Subsection` | in-column subheader |
| `#### Entry` | a bordered "card" (good for NPCs / locations / items) |
| `> text` | a boxed, italic read-aloud block |
| tables | styled; tables outside a card span the full width |
| `**bold**`, `_italic_` | inline emphasis (bold tinted with the theme accent) |

The renderer is intentionally standalone and dependency-light; copy it into any project.
