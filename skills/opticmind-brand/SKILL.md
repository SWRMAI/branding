---
name: opticmind-brand
description: Use when creating or reviewing Optic MindLabs UI, copy, visual assets, decks, websites, or design tokens. Enforces the OpticMind brand system from brand-styles.json, including colors, typography, logo assets, the kintsugi motif, layout, voice, company facts, and agent prompts.
---

# Optic MindLabs Brand

Use this skill whenever output must follow the Optic MindLabs brand.

## Source Of Truth

1. Read `brand-styles.json` before making brand decisions.
2. Validate edited style JSON against `brand-styles.schema.json`.
3. Treat this skill as implementation guidance and the JSON as canonical tokens.

## Brand Idea

The brand is built on the kintsugi principle: **the fracture is where the gold goes**. OpticMind traces gaps in awareness and fills them with intelligence.

- Brand line: "Beauty in the break."
- Slogan (what we do): "Capture. Analyze. Optimize." — presented as fact, in the order we build.
- Tagline: "We proudly turn movements into meaning."

## Company Facts

Pull specifics from the `company` section of `brand-styles.json`. The essentials:

- Canadian-founded, anchored in North America, built for a global market.
- Sensing: vision, lidar, audio, and Wi-Fi capture detecting people, vehicles, animals, and objects in motion — direction, movement, size, colour, and safety details like hard hats and vests.
- Hardware (working name "da'box"): enterprise line for job sites, facilities, and fleets (purchase or rent), plus a retail residential product for households.
- Platform: cloud-based SaaS portal and mobile app, subscription tiers from homeowner to nonprofit to enterprise; analyzes patterns and anomalies and triggers real-world responses (text, email, control switch), enriched with weather and geolocation data.
- Research lab (the "Labs" the company is named for): fully funded partnerships with corporations and educational institutions, two to three industry papers a year.
- Leadership: Daniel Blair (Co-Founder & CTO — technology vision, hardware, AI, research) and Jerin Valel (Co-Founder & COO — operations and go-to-market).

**Naming:** written name is "Optic MindLabs"; the wordmark lockup renders OPTICMIND / LABS; the production logo art reads "Optic Mind Labs". Product names and division structure are working language and may evolve — do not invent new product names.

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

Write with precision, composure, plain-spoken confidence, and human usefulness.

- Prefer measurable details and operational specifics.
- Be plain-spoken and literal about what things do: "turns what a camera sees into what a business needs to know."
- Present the slogan as fact, in build order: "Capture. Analyze. Optimize. That's not just a slogan we picked for effect. It's the order we build in."
- Anchor benefits in outcomes: see clearly, decide faster, stay safer.
- Speak to every audience with the same respect — an enterprise job site tracking hard hats and a homeowner keeping an eye on their property get the same clarity.
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
