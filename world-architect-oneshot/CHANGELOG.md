# Changelog

All notable changes to this project are documented here.

## [1.0.0]
- Initial public release.
- `prompt/world-architect-oneshot.xml` — canonical, fully-structured prompt with the complete
  output contract and per-NPC/faction/location/encounter field lists.
- **Continuity Checkpoints** — build-time gates, global invariants, and a required World Continuity
  Map to guarantee a connected world with no orphaned lore.
- `prompt/quick-use.txt` and `prompt/world-architect-oneshot.md` — lighter and human-readable versions.
- `docs/` — output contract, continuity system, design philosophy, and model-specific notes.
- `tools/render.py` — optional Markdown-to-PDF renderer with five themes.
- Two original example campaigns: **The Ethereal** (fantasy) and **The Long Quiet** (science
  fiction), each with a rendered PDF and a World Continuity Map.
- GitHub scaffolding: issue forms, a pull-request template, and a CI workflow that validates the
  prompt XML and test-renders an example.
