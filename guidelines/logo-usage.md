# AFLUENCE — Logo Usage Guide

Aplica al logo de **junio 2026**, el que vive en `assets/logos/`. Es el mismo que
embarcan web-blueprint, afluence-excalidraw y afluence-miro.

**Nunca dibujes ni reconstruyas el logo.** La marca es un velero con dos velas y casco.
Siempre usa un archivo de `assets/logos/`.

## Versiones

| Version | Contiene | Usar para |
|---------|----------|-----------|
| **Horizontal** | Velero + wordmark "Afluence" | Headers web, presentaciones, documentos, firmas, ads |
| **Symbol** | Solo el velero | Favicons, app icons, avatares, watermarks, perfiles sociales |

No existe una version "solo wordmark" ni una version con tagline embebido. Si necesitas
"Building your empire" como texto, tipografialo aparte en Archivo Medium (500),
letter-spacing 1.1.

## Variantes de color

| Variante | Fondo | Archivos |
|----------|-------|----------|
| **Dark** | Claro (blanco, Steel) | `*-dark-transparent.*` — fondo transparente |
| **White** | Oscuro (Obsidian, Abyss) | `*-white-transparent.*` — fondo transparente |
| **On-White** | — | Raster con fondo blanco horneado |
| **On-Black** | — | Raster con fondo negro horneado |

Prioriza siempre las transparentes (`Dark` / `White`). `On-White` y `On-Black` son solo
para contextos que no soportan transparencia.

## Formatos disponibles

| Formato | Donde | Usar para |
|---------|-------|-----------|
| SVG | `Dark/`, `White/` | Web, cualquier cosa que escale |
| PDF | `Dark/`, `White/` | Print, handoff a diseno |
| PNG | todas las variantes | Ads, social, docs, email |
| JPG | `On-White/`, `On-Black/` | Solo donde PNG no sirva |

Tamanos PNG: Horizontal en 512 / 1024 / 2048px. Symbol en 16 / 32 / 48 / 64 / 128 /
256 / 512 / 1024px — el rango bajo existe especificamente para favicons.

## Colores dentro de la marca

| Elemento | HEX |
|----------|-----|
| Velas | `#000000` sobre claro, `#FFFFFF` sobre oscuro |
| Casco | `#959899` |

`#959899` es el gris oficial del casco. No lo sustituyas por Slate (`#404040`) ni por
ningun otro gris.

## Tamanos minimos

| Version | Digital | Print |
|---------|---------|-------|
| Horizontal | 150px ancho | 40mm |
| Symbol | 16px (favicon), 32px en cualquier otro contexto | 10mm |

## Clear space

- Horizontal: espacio minimo = altura de la letra "A" del wordmark en cada direccion
- Symbol: 25% del ancho del simbolo en cada direccion

## Fondos permitidos

- Blanco (`#FFFFFF`) → Dark
- Negro (`#000000`) → White
- Abyss (`#0A0A0A`) → White
- Steel (`#E5E7EB`) → Dark
- Foto oscura con contraste suficiente → White

## 10 DON'Ts

1. No dibujar ni reconstruir el logo a mano — siempre usar el archivo
2. No rotar el logo
3. No estirar ni distorsionar
4. No cambiar los colores fuera de las variantes definidas
5. No agregar efectos (sombras, brillos, 3D, outlines)
6. No colocar sobre fondos de color (solo negro, blanco, Abyss, Steel)
7. No modificar la tipografia del wordmark
8. No agregar elementos al logo (bordes, contenedores, badges)
9. No reducir por debajo del tamano minimo
10. No usar la variante Dark sobre fondos oscuros (y viceversa)
