# Mediakit — Betamina

Material de marca listo para producción: logotipos, paleta, tipografía, iconos, guías y assets de
broadcast, más la landing que los presenta en español, inglés y portugués.

## Ver la landing

- **Publicada:** https://tarsterminal.duckdns.org/betamina-mediakit/ — con selector de idioma en el
  encabezado (`index.html` ES · `index-en.html` EN · `index-pt.html` PT).
- **En local:** abrir `index.html` en el navegador (funciona sin servidor: no hay dependencias
  externas más allá de la fuente Prompt de Google Fonts).

## Estructura

```
index.html · index-en.html · index-pt.html    la landing en los tres idiomas
favicon.png · flag-es.png · flag-en.png · flag-pt.png
logo-betamina.webp · hero-mediakit.png        logotipo horizontal y mockup de portada
mox3cc*-FTCalhern-*.otf                       familia tipográfica completa (los cortes que usa la
                                              landing son WideBold, WideBoldItalic, WideSemibold y
                                              WideSemiboldItalic; se incluyen todos los pesos)
downloads/                                    packs descargables desde la landing
  Logos_betamina.zip
  Paleta_de_colores.zip
  FTCalhern.zip
  Iconos Betamina.zip
  Manuales de marca.zip
  paleta-color.css · paleta-color.json
```

## Contenido de cada pack

| Pack | Qué trae | Formatos | Tamaño |
|---|---|---|---|
| Logotipos | Logotipo, isotipo y favicon oficiales | PNG, WEBP, AI, PDF | 3,3 MB |
| Paleta de Color | Paleta oficial del brand book y sistema extendido con tokens | CSS, JSON | 2,4 KB |
| Tipografía | Familia FT Calhern completa (display, condensed y wide) | OTF, TTF | 5,0 MB |
| Set de Iconos | Iconos oficiales de categorías y productos | SVG | 187 KB |
| Guía de Marca | Brand manual y concepto de marca | PDF | 76,7 MB |

## Pendientes del material de origen

Dos archivos que la landing enlaza no llegaron en el export y quedan documentados acá:

- **`downloads/Mediakit.zip`** — no existe todavía: es el bundle completo que ofrece el botón
  «Descargar .zip» de la sección final de la landing. Falta generarlo.
- **`downloads/Broadcast Assets.zip`** — el archivo del export original está **truncado** (72.196.096
  bytes, sin índice ZIP: no se puede abrir con ninguna herramienta). No se incluye en este
  repositorio; hay que re-exportarlo desde la fuente.

## Notas de armado

- **`favicon.png`**: se redujo de 2048×2048 (3,2 MB) a 256×256 (46 KB) para no servir 3 MB en cada
  visita. El original de 2048 px sigue dentro de `downloads/Logos_betamina.zip`.
- **`flag-es.png`**: en el export la bandera de España venía con nombre aleatorio
  (`mox7bl7r-image.png`); se guardó con el nombre que usa el HTML.
- **`downloads/Paleta_de_colores.zip`**: se armó con los dos archivos de la paleta (`paleta-color.css`
  y `paleta-color.json`) que sí venían sueltos en el export.
- Los archivos de tipografía **conservan el nombre del export original** (`mox3cc…-FTCalhern-*.otf`)
  porque así los referencia el CSS de la landing; renombrarlos la rompe.
- No se incluyeron los borradores intermedios de la landing ni las copias duplicadas de imágenes con
  nombre aleatorio (eran el mismo archivo que las versiones con nombre definitivo).

## Créditos

Diseño y desarrollo: **Dendra**. Los assets de marca pertenecen a Betamina.
