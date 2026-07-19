---
name: opticmind-brand
description: Use when creating or reviewing OpticMind Labs UI, copy, visual assets, decks, websites, or design tokens. Enforces the OpticMind brand system from brand-styles.json, including colors, typography, logo assets, the kintsugi motif, layout, voice, and agent prompts.
---

# OpticMind Labs Brand

Use this skill whenever output must follow the OpticMind Labs brand.

## Source Of Truth

1. Read `brand-styles.json` before making brand decisions.
2. Validate edited style JSON against `brand-styles.schema.json`.
3. Treat this skill as implementation guidance and the JSON as canonical tokens.

## Brand Idea

The brand is built on the kintsugi principle: **the fracture is where the gold goes**. OpticMind traces gaps in awareness and fills them with intelligence. Brand line: "Beauty in the break." Slogan: "Turning movements into meaning" (sentence case, no exclamation mark). Tagline: "Capture. Analyze. Optimize."

## Logo Assets

- `assets/opticmind-labs-logo.png` is the official production lockup (dome camera with AI core, particle ring, wordmark, tagline). Use it for outward-facing applications, on Obsidian or near-black backgrounds only. On dark UI, blend its black plate away with `mix-blend-mode: screen`.
- The vector mark system: Aperture Eye (primary mark), Swarm Iris (particle nodes resolving into an iris), Fractured O (monogram for favicons and tight spaces).
- Clearspace of one iris-height on all sides; minimum 28px for the monogram, 120px for full lockups.
- Never distort, recolor, blur, fade, or place marks on light or busy mid-tone backgrounds.

## Visual Direction

- Use Obsidian (`#0B0B0D`) as the dominant canvas.
- Use Graphite and Panel for dark cards; card stages use `radial-gradient(circle at 50% 40%, #161318, #0A0A0C)`.
- Use Pearl for primary text on dark backgrounds; Mist, Stone, and Ash for secondary text down to metadata.
- Use Kintsugi Gold sparingly for signal, seams, logo strokes, and primary actions — a seam, never a flood.
- Use the signature gradients from `colors.gradients` (135deg 4-stop `goldSignature`, vertical `goldVertical`, text-clip `goldText`) instead of flat gold fills for marks and headline words.
- Kintsugi photo textures (`assets/kintsugi-*.{jpg,webp,avif}`) may sit behind heroes at 0.2–0.3 opacity, vignetted into Obsidian with a radial gradient.
- Draw gold seams as thin (1–2.5px) irregular polylines — section dividers, hero edges, data flows. Always a path with meaning, never decorative noise.
- Keep component radii at `6px` unless a platform constraint requires otherwise.
- Avoid off-palette blues, pastels, playful gradients, ornamental clutter, and heavy glow effects.

## Typography

- Use Space Grotesk for headings, navigation, buttons, labels, and wordmarks.
- Use Manrope for body text, tables, dashboards, captions, and dense UI.
- Use Cormorant Garamond for hero statements and brand moments — typically 500 weight, tight line-height, with the key word in italic clipped to the gold text gradient — plus editorial accents and pull quotes.
- Keep letter spacing at `0` for most text; use uppercase tracked labels (up to `0.32em`, gold or ash) for eyebrows, captions, and small metadata.

## Voice

Write with precision, composure, and human usefulness.

- Prefer measurable details and operational specifics.
- Lean on the kintsugi idea — fractures traced and filled with intelligence — for brand moments.
- Avoid vague futurism and exaggerated claims.
- Avoid fear-based surveillance language: we connect, we don't surveil.

## Implementation Checklist

- Load `brand-styles.json`.
- Use the documented color tokens and gradients rather than inventing close variants.
- Use the documented font roles, including the serif hero treatment.
- Use `assets/opticmind-labs-logo.png` for official lockups and kintsugi textures for hero backdrops.
- Keep dark operational layouts quiet and scan-friendly; reserve gold for emphasis and structure.
- Check contrast for text on dark surfaces.
- For generated JSON, validate against `brand-styles.schema.json`.
