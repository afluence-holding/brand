# Afluence — Brand

Single source of truth for the Afluence brand system: design tokens, tone of voice,
logos, fonts and guidelines.

This repo **is** the `afluence-brand-core` agent skill. `SKILL.md` is the entry point
every AI agent reads; everything else is loaded on demand.

## Layout

```
SKILL.md              agent entry point (design tokens, tone of voice, values, anti-patterns)
assets/logos/         Horizontal/ and Symbol/, each in Dark, White, On-Black, On-White
assets/fonts/         Sora + Archivo (.ttf)
guidelines/           logo-usage, palette, tone-of-voice, quick-reference
brandbook/            AFLUENCE-Brandbook.pdf / .pptx
```

## Logos

The `assets/logos/` set is the **June 2026** artwork — the same files shipped by
web-blueprint, afluence-excalidraw and afluence-miro (verified byte-identical).

| Need | Path |
|---|---|
| Full lockup on dark background | `assets/logos/Horizontal/White/` |
| Full lockup on light background | `assets/logos/Horizontal/Dark/` |
| Mark only (favicon, avatar, app icon) | `assets/logos/Symbol/` |
| Print / vector handoff | any `*.pdf` or `*.svg` in the above |

Transparent variants are `Dark` and `White`. `On-Black` / `On-White` are baked-background
raster exports. Symbol ships down to 16px for favicon use.

## How agents reach this

```
~/.agents/skills/afluence-brand-core  ->  ~/Developer/afluence/BRAND
~/.claude/skills/afluence-brand-core  ->  ../../.agents/skills/afluence-brand-core
```

Codex, Gemini and Claude are pointed here from their global instruction files.

## Known gaps

Carried over from the imported material — not yet resolved:

1. **`SKILL.md` embeds the old March logo.** The inline SVG is the superseded
   polygon+arc mark, not the June artwork in `assets/logos/`.
2. **`guidelines/logo-usage.md` documents the old lockup system**
   (Primary / Compact / Icon-Only / Wordmark-Only, black-on-white / white-on-black / gray).
   The June set uses Horizontal / Symbol with Dark / White / On-Black / On-White.
3. **`#959899` is undocumented.** The June mark uses it for the sail element; it appears
   in neither `SKILL.md` nor `guidelines/palette.md`. Either adopt it as a token or
   normalize the SVGs to `#767676`.
4. **Two font weights referenced but not vendored.** `SKILL.md` imports Sora 400 and
   Archivo 700; `assets/fonts/` has neither. Fine over the Google Fonts CDN, a problem
   for offline, print and video work.

## Provenance

`SKILL.md` was imported from the `anthropic-skills` plugin copy (2026-04-07), which is a
strict superset of the `afluence-marketing-os` copy (2026-07-13) — the latter is identical
except that it drops the `## Visual System — NB2` section. Nothing was lost in the import.
