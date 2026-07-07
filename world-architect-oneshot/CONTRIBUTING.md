# Contributing

Thanks for your interest! This project is a prompt framework plus a small rendering tool.

## Good contributions

- **Prompt improvements** — sharper instructions, better continuity gates, clearer field lists.
  Keep the XML (`prompt/world-architect-oneshot.xml`) as the source of truth and mirror changes into
  the Markdown overview and `docs/output-contract.md`.
- **Model notes** — real-world tuning tips for specific models in `docs/using-with-models.md`.
- **Renderer** — new color themes in `tools/render.py`, layout fixes, or Markdown-convention support.
  Please keep it dependency-light and standalone.
- **Original example campaigns** — fully original settings only. Do **not** submit examples built on
  third-party IP; the existing fan-content example is a special, clearly-labeled case.

## Guidelines

- Discuss large changes in an issue first.
- Keep the prompt model-agnostic; put model-specific advice in the docs, not the prompt.
- For content contributions, confirm they are yours to license under CC BY 4.0.
- Test `tools/render.py` against an example before opening a PR.
