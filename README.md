# Mediakit — Betamina

Material de marca listo para producción: logotipos, paleta, tipografía, iconos, guías y assets de
broadcast, más la landing que los presenta en español, inglés y portugués.

## Descargar todo el mediakit

| Vía | Qué se baja | Link |
|---|---|---|
| Landing publicada | `Mediakit.zip` (126 MB) — el mediakit completo en un ZIP | https://tarsterminal.duckdns.org/betamina-mediakit/ |
| Link directo | el mismo ZIP, sin pasar por la página | https://tarsterminal.duckdns.org/betamina-mediakit/downloads/Mediakit.zip |
| GitHub | `Mediakit-Betamina.zip` (126 MB) | https://github.com/tonic1234/betamina-mediakit/releases/latest |
| GitHub | el repositorio entero tal como está | https://github.com/tonic1234/betamina-mediakit/archive/refs/heads/main.zip |

El ZIP del mediakit trae una carpeta `Betamina_Mediakit/` con los 93 archivos del repositorio (la
landing, la tipografía, las imágenes y los packs de `downloads/`). No se guarda dentro del
repositorio para no duplicar 126 MB en cada clon: vive en la landing y en la Release.

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

## Pendiente del material de origen

- **`downloads/Broadcast Assets.zip`** — el archivo del export original está **truncado**
  (72.196.096 bytes, sin índice ZIP: no se puede abrir con ninguna herramienta). No se incluye en el
  repositorio ni en el ZIP del mediakit; hay que re-exportarlo desde la fuente. La tarjeta
  «Broadcast Assets» de la landing queda pendiente de ese archivo.

## Notas de armado

- **`Mediakit.zip`** (el botón «Descargar .zip» de la landing) se armó con los cinco packs que sí
  llegaron en el export más la landing completa. La etiqueta del botón y la mención del FAQ decían
  «295 MB» por el tamaño del export original; ahora dicen el peso real: **126 MB**.
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
