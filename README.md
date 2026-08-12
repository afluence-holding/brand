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

None outstanding.

### Resolved

- ~~Sora 400 referenced but not vendored~~ — added. Instanced from the upstream
  `Sora[wght].ttf` variable font at `wght=400`, same v2.000 as the other weights.
- ~~Archivo 700 imported but never used~~ — removed from the `@import`. Archivo runs
  400/500/600 only; Sora carries all heavy weights.

- ~~`SKILL.md` embedded a hand-drawn approximation of the logo~~ — the fake polygon+arc
  inline SVG is gone. `SKILL.md` now forbids drawing the logo and points at
  `assets/logos/` files only.
- ~~`guidelines/logo-usage.md` documented the old lockup system~~ — rewritten for
  Horizontal / Symbol with Dark / White / On-Black / On-White.
- ~~`#959899` undocumented~~ — adopted as the official hull color. `--af-hull` was
  `#767676` (the old mark); now `#959899`, matching what every product ships.

## Provenance

`SKILL.md` was imported from the `anthropic-skills` plugin copy (2026-04-07), which is a
strict superset of the `afluence-marketing-os` copy (2026-07-13) — the latter is identical
except that it drops the `## Visual System — NB2` section. Nothing was lost in the import.
