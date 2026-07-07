# Examples

Complete one-shots generated with the framework, provided as source Markdown (so you can see the
shape of the output) and as rendered PDFs (made with [`../tools/render.py`](../tools/render.py)).
Both are **fully original** — no third-party settings — so the whole repository is safe to publish.

- **[the-ethereal/](the-ethereal/)** — *The Ethereal.* An eerie fantasy mystery: a stilt-city that
  powers its lamps by fishing the souls of its own dead (rendered with the `maroon` theme).
- **[the-long-quiet/](the-long-quiet/)** — *The Long Quiet.* A science-fiction mystery: a
  generation ship that has been "almost arriving" for a century, and the kind machine that never
  let its sleepers learn why (rendered with the `slate` theme).

Each includes a **World Continuity Map** near the end — the framework's proof that every faction,
NPC, location, and secret connects to a cause and to play.

To re-render either:
```bash
cd ../tools
python render.py ../examples/the-long-quiet/the-long-quiet.md -o ../examples/the-long-quiet/the-long-quiet.pdf \
    --title "The Long Quiet" --subtitle "Ten Thousand Sleepers" --theme slate
```
