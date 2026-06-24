# OpticMind Labs Brand Kit

Static GitHub Pages brand kit for OpticMind Labs. The site documents the core identity, color system, typography, motif, voice, downloadable style JSON, schema, prompts, and reusable agent skill guidance.

## Files

- `index.html` - GitHub Pages entry point and visual brand guide.
- `brand-styles.json` - Agent-ready source of truth for brand tokens and usage rules.
- `brand-styles.schema.json` - JSON Schema for validating brand style files.
- `skills/opticmind-brand/SKILL.md` - Agent skill for implementing the brand consistently.

## Using the Brand JSON

Give agents both files when asking them to create UI, copy, decks, or visual assets:

```text
Use brand-styles.json as the source of truth and validate against brand-styles.schema.json.
Follow skills/opticmind-brand/SKILL.md for implementation decisions.
```

The site also includes a "Download JSON" action so the brand styles can be handed to external agents directly.

## GitHub Pages

This repo is static. Enable GitHub Pages from the repository settings and serve from the branch root. No build step is required.

## Local Preview

Open `index.html` directly in a browser, or run a tiny static server from this directory:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
