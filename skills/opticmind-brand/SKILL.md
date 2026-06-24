---
name: opticmind-brand
description: Use when creating or reviewing OpticMind Labs UI, copy, visual assets, decks, websites, or design tokens. Enforces the OpticMind brand system from brand-styles.json, including colors, typography, layout, voice, and agent prompts.
---

# OpticMind Labs Brand

Use this skill whenever output must follow the OpticMind Labs brand.

## Source Of Truth

1. Read `brand-styles.json` before making brand decisions.
2. Validate edited style JSON against `brand-styles.schema.json`.
3. Treat this skill as implementation guidance and the JSON as canonical tokens.

## Visual Direction

- Use Obsidian (`#0B0B0D`) as the dominant canvas.
- Use Graphite and Panel for dark cards and raised surfaces.
- Use Pearl for primary text on dark backgrounds.
- Use Ash and Mist for metadata, captions, and secondary text.
- Use Kintsugi Gold sparingly for signal, dividers, logo strokes, and primary actions.
- Keep component radii at `6px` unless a platform constraint requires otherwise.
- Prefer thin, meaningful gold connection lines over decorative texture.
- Avoid off-palette blues, pastels, playful gradients, ornamental clutter, and heavy glow effects.

## Typography

- Use Space Grotesk for headings, navigation, buttons, labels, and wordmarks.
- Use Manrope for body text, tables, dashboards, captions, and dense UI.
- Use Cormorant Garamond only for editorial accents or pull quotes.
- Keep letter spacing at `0` for most text; use uppercase tracked labels only for captions, eyebrows, and small metadata.

## Voice

Write with precision, composure, and human usefulness.

- Prefer measurable details and operational specifics.
- Avoid vague futurism and exaggerated claims.
- Avoid fear-based surveillance language.
- Frame technology as connecting, interpreting, and helping people act.

## Implementation Checklist

- Load `brand-styles.json`.
- Use the documented color tokens rather than inventing close variants.
- Use the documented font roles.
- Keep dark operational layouts quiet and scan-friendly.
- Reserve gold for emphasis and structure.
- Check contrast for text on dark surfaces.
- For generated JSON, validate against `brand-styles.schema.json`.
