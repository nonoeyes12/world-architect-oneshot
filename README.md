# World Architect + One-Shot Campaign Builder

A master prompt framework that turns a one-line idea into a complete, ready-to-run one-shot
tabletop RPG campaign — with a connected world, a fair-but-surprising mystery, real player
agency, and practical tools for running it at the table.

It is system-neutral by default (add D&D 5e, Pathfinder, Mothership, Blades in the Dark, or any
other ruleset in the brief), and it is designed to fight the most common failure of AI-generated
settings: lore that connects to nothing and never reaches the table.

## What's inside

- prompt/ — the framework itself: a fully structured XML prompt, a readable Markdown version,
  and a short copy-paste "quick-use" version.
- docs/ — the output contract (every section the framework produces), the continuity system,
  the design philosophy, and notes for using it with different models.
- tools/ — an optional Python script that turns a generated campaign into a print-ready,
  two-column "aged manuscript" PDF, in several color themes.
- examples/ — two complete, fully original sample campaigns (a fantasy mystery and a
  science-fiction mystery), each with source text and a rendered PDF.

## How to use it

1. Open the prompt in the prompt/ folder.
2. Fill in as much of the brief as you like. Anything left blank becomes a labeled assumption —
   the framework never stops to ask questions.
3. Paste it into your model of choice and send. You get a full campaign back, in order, ending
   with a continuity map and a one-page run sheet you can play from.
4. Optional: save the result as a Markdown file and run the renderer in tools/ to make a PDF.

## What makes it different

- The world is built as a pressure system: history creates institutions, institutions create
  factions, factions create conflicts, conflicts create secrets, secrets create discovery,
  discovery changes choices, and choices change the ending.
- Continuity checkpoints run while the campaign is built, and a required continuity map at the
  end proves that every faction, character, location, and secret connects to a cause and to play.
- The mystery is robust: many secrets, several clues each, and no single point of failure.
- The output is runnable, not just pretty: pacing by time block, an escalation clock,
  random tables, fallback clues, and a condensed run sheet.

## License

The prompt, documentation, and example campaigns are licensed under CC BY 4.0. The code in
tools/ is licensed under the MIT License. All example content is original and contains no
third-party intellectual property.
