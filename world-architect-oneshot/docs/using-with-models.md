# Using the Framework with Different Models

The framework is model-agnostic, but a few notes help.

**Claude (Opus/Sonnet 4.x) — recommended.** Use the XML prompt
([`../prompt/world-architect-oneshot.xml`](../prompt/world-architect-oneshot.xml)); Claude follows
XML-tagged structure closely and honors the continuity checkpoints and output contract well. Paste
the whole file, fill the `<inputs>` fields, and send. It is happy to make strong labeled
assumptions instead of asking.

**GPT-class models.** The XML works, or use [`../prompt/quick-use.txt`](../prompt/quick-use.txt) for
a lighter footprint. Be explicit that it should not stop to ask questions and should produce all
sections in one pass; you may need to say "continue" if output is truncated.

**Gemini.** Works well with the long structured prompt; if it drifts from the section order, add
"Follow the Output Contract section order exactly." Ask it to flag any invented real-world facts.

**Reasoning-native models (o-series, R1, thinking modes).** Prefer the concise quick-use prompt;
don't add extra "think step by step" scaffolding — they reason internally.

**Local / open-weight models.** Use the quick-use prompt and expect to run section-by-section
(e.g., "now produce the World Bible," then "now the Factions"), since long single-pass generation
can lose coherence.

**Tips for any model**
- Fill as much of the brief as you can; blanks become the model's labeled assumptions.
- If a run feels thin, paste back the *Continuity Checkpoints* section and ask it to audit and fix
  orphans.
- Generate into Markdown, then use [`../tools/render.py`](../tools/render.py) to make a
  print-ready PDF.
