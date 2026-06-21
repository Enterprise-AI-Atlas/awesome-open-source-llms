# Contributing

Contributions are welcome. Please read this guide before opening a pull request.

## What belongs in this list

This registry is for open-weight / open-source large language models and closely related model families. Acceptable entries include:

- Foundation text LLMs with publicly downloadable weights.
- Domain- or task-specialized models (coding, reasoning, vision-language, multilingual, small/fast).
- High-quality community fine-tunes of open foundation models.
- Official Hugging Face collections or organization pages that group a model family.

## What does **not** belong

- Closed API-only models with no publicly downloadable weights.
- Commercial services that merely host open models without adding a distinct model artifact.
- Unmaintained or undocumented model checkpoints.
- Duplicate entries.

## Quality bar

Every submission must be:

1. **Publicly accessible weights** — the model files or GGUF/quantized variants must be downloadable without a paywall.
2. **Actively maintained** — last meaningful release or commit within the last 12 months (exceptions for historically important reference models).
3. **Documented** — a real model card with license, size, and usage information.
4. **Correctly categorized** — placed under the category that best matches its primary use case.
5. **Honestly labeled** — use the `Official` or `Community` badge.

## Entry format

Use this pattern:

```markdown
- **[Name](URL)** `Official` — One-sentence description.
  - Sizes: Xb, Yb
  - License: [License Name](license-url)
```

If there is no size variation, omit the sizes line. If the license is already obvious from the linked model card, the license line is optional.

## Category sections

The README is organized by **model use case**, not by organization. New category sections are allowed only if they contain at least five entries.

## Pull request process

1. Fork the repository.
2. Add your entry in the correct category section.
3. Run `./scripts/validate-links.sh` and fix any broken links or anchors.
4. Open a pull request with a clear description of the model, its license, and why it fits.

One model per pull request is preferred.
