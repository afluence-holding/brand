# AFLUENCE — Color Palette: OBSIDIAN

## Palette

| Token | Name | HEX | RGB | HSL | Role |
|-------|------|------|------|------|------|
| AF-01 | Obsidian | `#000000` | `rgb(0, 0, 0)` | `hsl(0, 0%, 0%)` | Base principal, fondos dark |
| AF-02 | Abyss | `#0A0A0A` | `rgb(10, 10, 10)` | `hsl(0, 0%, 4%)` | Superficies, cards, elevacion |
| AF-03 | Slate | `#404040` | `rgb(64, 64, 64)` | `hsl(0, 0%, 25%)` | Texto secundario, bordes |
| AF-04 | Steel | `#E5E7EB` | `rgb(229, 231, 235)` | `hsl(220, 13%, 91%)` | Fondos claros, dividers |
| AF-05 | Blanco | `#FFFFFF` | `rgb(255, 255, 255)` | `hsl(0, 0%, 100%)` | Texto sobre dark, fondos light |

## Logo-specific colors

| Element | HEX | Usage |
|---------|------|-------|
| Casco del velero | `#959899` | Igual en ambas variantes del logo |
| Velas | `#000000` / `#FFFFFF` | Negro sobre fondo claro, blanco sobre fondo oscuro |
| Tagline | `#5C5C5C` / `#808080` | Texto "Building your empire" — claro / oscuro |

## Usage rules

- **Dark mode es el default.** El fondo principal es Obsidian (#000000).
- **Sin color de acento.** La tipografia y el contenido hacen todo el trabajo visual.
- **Monocromatico frio, quirurgico.** Inspirado en Vercel, Studio Aberrante, OpenAI.
- Usar Abyss (#0A0A0A) para crear elevacion y separacion sobre fondos Obsidian.
- Usar Slate (#404040) para texto secundario y elementos de menor jerarquia.
- Usar Steel (#E5E7EB) solo en contextos light mode o como divider sutil.

## CSS Variables

```css
:root {
  --af-obsidian: #000000;
  --af-abyss: #0A0A0A;
  --af-slate: #404040;
  --af-steel: #E5E7EB;
  --af-white: #FFFFFF;
}
```

## Tailwind Config

```js
colors: {
  af: {
    obsidian: '#000000',
    abyss: '#0A0A0A',
    slate: '#404040',
    steel: '#E5E7EB',
    white: '#FFFFFF',
  }
}
```
