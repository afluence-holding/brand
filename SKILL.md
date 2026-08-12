---
name: afluence-brand-core
description: Shared brand foundation for all Afluence creative skills — design tokens, colors, typography, tone of voice, logo SVG, values, and anti-patterns. MUST be read before using any other afluence-* skill. Triggers on any request involving Afluence brand, brand guidelines, brand consistency, design system, tone of voice, or when any other afluence skill needs brand context.
---

# Afluence — Brand Core

This is the shared foundation for all Afluence creative skills. Each specialized skill (ads, social, landing, email) reads this file for brand consistency.

## Identity

**What:** AI Factory that builds digital empires for content creators.
**Not:** Agency, platform, course seller, guru operation.
**Mission:** Replace generic digital products with intelligent ecosystems that generate real results.
**Vision:** Define how content creators monetize in the age of AI.
**Tagline:** "Building your empire"
**Manifesto:** "We challenge what's broken. We build what's next."

---

## Design Tokens

### Colors — Obsidian Palette

| Token | HEX | Role |
|---|---|---|
| `--af-obsidian` | `#000000` | Primary backgrounds |
| `--af-abyss` | `#0A0A0A` | Cards, surfaces, elevation |
| `--af-slate` | `#404040` | Secondary text, borders |
| `--af-steel` | `#E5E7EB` | Light backgrounds, dividers |
| `--af-white` | `#FFFFFF` | Text on dark, light backgrounds |
| `--af-hull` | `#767676` | Logo hull only |
| `--af-tagline` | `#5C5C5C` | Logo tagline only |

NO accent color. No blues, greens, reds. Monochromatic only.

### CSS Variables

```css
@import url('https://fonts.googleapis.com/css2?family=Sora:wght@400;500;600;700;800&family=Archivo:wght@400;500;600;700&display=swap');

:root {
  --af-obsidian: #000000;
  --af-abyss: #0A0A0A;
  --af-slate: #404040;
  --af-steel: #E5E7EB;
  --af-white: #FFFFFF;
  --af-hull: #767676;
  --af-tagline: #5C5C5C;
  --af-font-heading: 'Sora', sans-serif;
  --af-font-body: 'Archivo', sans-serif;
  --af-space-xs: 8px;
  --af-space-sm: 16px;
  --af-space-md: 24px;
  --af-space-lg: 48px;
  --af-space-xl: 80px;
  --af-space-2xl: 120px;
  --af-radius: 0px;
  --af-max-width: 1200px;
}
```

### Typography

| Element | Font | Weight | Notes |
|---|---|---|---|
| H1 | Sora | 700 | uppercase |
| H2 | Sora | 600 | |
| H3 | Sora | 500 | |
| Body | Archivo | 400 | |
| Bold body | Archivo | 600 | |
| Caption | Archivo | 400 | color Slate |
| Code/Data | Sora | 400 | geometric feel |

### Components

**Buttons:** Outline style, Sora 600, 14px, uppercase, letter-spacing 1px, no border-radius. Hover inverts fill.
**Cards:** Background abyss, border 1px slate, no border-radius.
**Sharp corners everywhere.** Only exception: pill tags (border-radius: 100px).
**Section numbering:** 01, 02, 03 pattern with Sora, oversized or subtle.

---

## Tone of Voice

**60% Provocador + 40% Aspiracional**

Formula: Challenge the present → Elevate toward the future.

### Writing pattern
1. Open with provocation (uncomfortable truth, broken stat, direct challenge)
2. Follow with the shift (what's possible, what we built)
3. Close with power (last sentence is the strongest, mic drop)

### Tone Self-Check
Before delivering any copy, verify:
- Does the opening provoke discomfort or challenge a belief? (Provocador check)
- Does the closing feel aspirational or empowering? (Aspiracional check)
- Is there at least one concrete data point or contrast? (Specificity check)
- Would this message irritate a competitor? (Differentiation check)
If any answer is "no," rewrite that section.

### Copy rules
- Short sentences. Short paragraphs. Rapid rhythm.
- Use contrast: old (broken) vs new (built)
- Use concrete data (12% vs 90%)
- Speak as builder, not seller
- CTAs: direct, commanding ("Construye tu imperio" not "Aprende más")

### Vocabulary

**USE:** Construir, Imperio, Ecosistema, Infraestructura, Escalar, Automatizar, Factory, Motor de ventas, IA, Producto inteligente, Builder, Arquitectura, Sistema, Data, Resultado, Co-crear

**NEVER:** Curso, Mentoría tradicional, PDF, Ebook, Webinar, Gurú, Coach, Hack, Truco, Secreto, Fórmula mágica, Viral, Contenido orgánico, Emprendedor, Solopreneur, Hustle

### Vocabulary Expansion Rule
The USE list is a starting point, not a ceiling. Generate new vocabulary that fits the builder/empire/infrastructure tone. The NEVER list is a hard constraint — never use those words.

### Vocabulary Extensions by Niche
When generating for a specific niche, extend the USE vocabulary:
- **CREATOR/COACHING:** enrolled, certified, coaching model, client pipeline, session booking, group program, mastermind, community
- **SAAS/ENTERPRISE:** API, integration, implementation, deployment, pipeline, onboarding, churn, activation, retention
- **E-COMMERCE:** conversion funnel, AOV, repeat customer, fulfillment, catalog, checkout, cart recovery
- **EDUCATION:** enrollment, completion, curriculum, learning path, certification, cohort, outcome-based

### Signature phrases
- "Your course has 12% completion. Your empire deserves better."
- "Everyone sells followers. We build infrastructure."
- "From audience to asset. From content to company."
- "We don't pitch ideas. We build empires."
- "PDFs die in a folder. Empires don't."
- "Not a guru. Not an agency. An AI Factory."

### Creative Generation Rules

These signature phrases are TONE REFERENCES, not templates. They demonstrate the level of provocación and contraste Afluence operates at. When generating content:

1. **Never copy a signature phrase verbatim into output.** Generate original copy that matches this intensity level.
2. **Never default to the same stats.** The "12% vs 90%" comparison is ONE example of data contrast. Generate fresh, niche-specific data points every time:
   - If the user's niche is fitness: "Tu programa tiene 3x más inscripciones que finalizaciones"
   - If it's coaching: "El 80% de tus clientes no llegan a la sesión 4"
   - If it's education: "Tus alumnos pagan, entran, y desaparecen en 48 horas"
   - If no niche specified: Invent realistic data that varies each time
3. **Rotate pain points.** Don't always use "completion rate" as the pain. Rotate between: revenue leakage, time dependency, refund rates, audience waste, scaling ceiling, manual operations, low LTV, launch anxiety, platform dependency.
4. **Rotate proof metrics.** Don't always use "90% completion." Use: retention increase, revenue per follower, time saved, NPS, engagement multiplier, payback period, conversion rate lift.
5. **CTA expansion list** (minimum 12 options to rotate): "¿Hablamos?", "Agenda tu diagnóstico", "Construye con nosotros", "Reserva tu sesión", "Empieza aquí", "Ver cómo funciona", "Descubre tu potencial", "Transforma tu modelo", "Accede al sistema", "Inicia tu transformación", "Recibe tu auditoría", "Conecta con nuestro equipo"
6. **Contrast patterns should vary.** Don't always use "$9 PDF vs $50K ecosystem." Generate contrasts relevant to the user's specific situation, product, and audience size.

---

## Logo SVG

**Primary (black on white):**
```svg
<svg viewBox="0 0 220 68" xmlns="http://www.w3.org/2000/svg">
  <polygon points="42,2 42.5,44 8,44" fill="#000000"/>
  <path d="M4.5,47.5 A23.5,28.5 0 0,0 49,47.5" fill="#767676"/>
  <text x="58" y="43.5" font-family="'Sora',sans-serif" font-size="29" font-weight="600" fill="#000000">Afluence</text>
  <text x="58" y="58.5" font-family="'Archivo',sans-serif" font-size="12" font-weight="500" fill="#5C5C5C" letter-spacing="1.1">Building your empire</text>
</svg>
```

**Dark mode (white on black):**
```svg
<svg viewBox="0 0 220 68" xmlns="http://www.w3.org/2000/svg">
  <polygon points="42,2 42.5,44 8,44" fill="#E5E7EB"/>
  <path d="M4.5,47.5 A23.5,28.5 0 0,0 49,47.5" fill="#808080"/>
  <text x="58" y="43.5" font-family="'Sora',sans-serif" font-size="29" font-weight="600" fill="#FFFFFF">Afluence</text>
  <text x="58" y="58.5" font-family="'Archivo',sans-serif" font-size="12" font-weight="500" fill="#808080" letter-spacing="1.1">Building your empire</text>
</svg>
```

---

## Values

| # | Value | Phrase |
|---|---|---|
| 01 | Build Over Talk | "Pitching is easy. Shipping is Afluence." |
| 02 | Creator As CEO | "You have an audience. We give you a company." |
| 03 | Empire Mindset | "One product is a sale. An ecosystem is an empire." |
| 04 | Co-Create, Never Dictate | "Your expertise plus our engine. That's the formula." |
| 05 | Protect The Audience | "Their followers trusted them. We honor that trust." |
| 06 | Default To Action | "While others plan, we ship. Done beats perfect." |
| 07 | Radical Transparency | "Bad news fast. Good news faster." |

---

## Anti-Patterns

- No guru aesthetic (neon, "make money fast", stock beach photos)
- No corporate emptiness ("synergy", "paradigm", "holistic")
- No soft language ("perhaps", "maybe consider", "we'd love to")
- No rounded corners (exception: pill tags)
- No color accents
- No emojis in professional content (max 1-2 strategic in social)
- No excessive punctuation (!!! or ???)
- No apologies for being direct

---

## Visual System — NB2 (AI-Generated Backgrounds)

Afluence creative skills support two visual modes. Every visual skill (meta-ad, instagram-post, instagram-story, instagram-carousel) can operate in either mode.

### Mode A — Typography Only (Original)
Black background (#000000), text-driven. The headline IS the creative. No images.
Use for: brand content, thought leadership, pure messaging, organic social, low-budget testing.

### Mode B — NB2 Background (AI-Generated)
Surrealist AI image generated via `afluence-imagen-nb2` skill with built-in text-zone composition. Text overlaid in the designed clean zone — NO gradient overlay.
Use for: paid ads, campaign creatives, scroll-stopping visuals, launches, high-impact placements.

### NB2 Integration Rules
1. **Image first, text second.** Generate the NB2 base with text-zone composition before writing any overlay HTML.
2. **Text-zone composition is mandatory.** Every NB2 prompt for ads MUST include a composition instruction that reserves clean dark space for text. Default: left-side zone (subject on right two-thirds, left third clean black void).
3. **No gradient overlays.** The image is composed WITH the text space. If text isn't readable without a gradient, regenerate the image with better zone separation.
4. **Text styling unchanged.** Same Sora headlines, Archivo body, white on dark, brand tokens apply identically.
5. **Logo placement adapts.** Place logo in the corner opposite to the text zone (if text is bottom-left, logo goes top-left or top-right).
6. **NB2 images are niche-adapted.** Use the creator's specific items, pain visuals, and dream visuals — never generic stock-style imagery.
7. **Every NB2 image is unique.** The concept engine generates infinite variations. Never reuse concepts across campaigns.

### Text-Zone Composition Patterns
| Zone | Prompt Addition | Best For |
|------|----------------|----------|
| Left third | "Subject occupies right two-thirds. Left third is clean empty pure black void reserved for text." | Default — most reliable |
| Bottom 30% | "Subject occupies upper 65%. Bottom 35% is clean empty darkness." | Centered/symmetrical subjects |
| Right third | "Subject occupies left two-thirds. Right third is clean empty void." | Alternate when left feels repetitive |
| Upper-left quadrant | "Subject in lower-right. Upper-left quadrant clean black void." | Diagonal compositions |

### NB2 Skill Reference
The full NB2 generation system (concept engine, prompt engineering, batch workflow, scripts) lives in `afluence-imagen-nb2/SKILL.md`. Always read it before generating AI images.
