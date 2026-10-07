# Mediakit — Betamina

Material de marca listo para producción: logotipos, paleta, tipografía, iconos, guías y assets de
broadcast, más la landing que los presenta en español, inglés y portugués.

## Descargar todo el mediakit

| Vía | Qué se baja | Link |
|---|---|---|
| Landing publicada | `Mediakit.zip` (85 MB) — todos los packs en un ZIP | https://tarsterminal.duckdns.org/betamina-mediakit/ |
| Link directo | el mismo ZIP, sin pasar por la página | https://tarsterminal.duckdns.org/betamina-mediakit/downloads/Mediakit.zip |
| GitHub | `Mediakit-Betamina.zip` (85 MB) | https://github.com/tonic1234/betamina-mediakit/releases/latest |
| GitHub | el repositorio entero tal como está | https://github.com/tonic1234/betamina-mediakit/archive/refs/heads/main.zip |

El ZIP del mediakit trae **el contenido de `downloads/`**: los cinco packs más `paleta-color.css` y
`paleta-color.json`, tal como salen de la carpeta (sin la landing ni los archivos que ya están en el
repositorio). No se guarda dentro del repositorio para no duplicar 85 MB en cada clon: vive en la
landing y en la Release.

Los enlaces de descarga de la página son **nativos** (`<a download>`): el navegador baja el archivo
con su propia barra de progreso. No se usa `fetch` + `blob`, que obligaba a cargar los 85 MB en
memoria antes de ver cualquier señal —en conexiones lentas parecía que el botón no hacía nada.

## Ver la landing

- **Publicada:** https://tarsterminal.duckdns.org/betamina-mediakit/ — con selector de idioma en el
  encabezado (`index.html` ES · `index-en.html` EN · `index-pt.html` PT).
- **En local:** abrir `index.html` en el navegador (funciona sin servidor: no hay dependencias
  externas más allá de la fuente Prompt de Google Fonts).

## Estructura

```
index.html · index-en.html · index-pt.html    la landing en los tres idiomas
assets/
  favicon.png
  flag-es.png · flag-en.png · flag-pt.png     banderas del selector de idioma
  logo-betamina.webp · hero-mediakit.png      logotipo horizontal y mockup de portada
  mascota-mediakit.png                        render de la mascota (2150×1984)
  tipografia/                                 familia FT Calhern completa (69 archivos)
manual-de-marca/
  BETAMINA-BRAND-MANUAL.pdf                   brand manual (25,9 MB) para leer sin descomprimir
downloads/                                    packs descargables desde la landing
  Logos_betamina.zip
  Paleta_de_colores.zip
  FTCalhern.zip
  Iconos Betamina.zip
  Manuales de marca.zip
  paleta-color.css · paleta-color.json
```

Los cuatro cortes de FT Calhern que usa la landing son WideBold, WideBoldItalic, WideSemibold y
WideSemiboldItalic; en `assets/tipografia/` están todos los pesos y variantes.

## Contenido de cada pack

| Pack | Qué trae | Formatos | Tamaño |
|---|---|---|---|
| Logotipos | Logotipo, isotipo y favicon oficiales | PNG, WEBP, AI, PDF | 3,3 MB |
| Paleta de Color | Paleta oficial del brand book y sistema extendido con tokens | CSS, JSON | 2,4 KB |
| Tipografía | Familia FT Calhern completa (display, condensed y wide) | OTF, TTF | 5,0 MB |
| Set de Iconos | Iconos oficiales de categorías y productos | SVG | 187 KB |
| Guía de Marca | Brand manual y concepto de marca (3 PDF) | PDF | 76,7 MB |

## Pendiente del material de origen

- **`downloads/Broadcast Assets.zip`** — el archivo del export original está **truncado**
  (72.196.096 bytes, sin índice ZIP: no se puede abrir con ninguna herramienta). No se incluye en el
  repositorio ni en el ZIP del mediakit; hay que re-exportarlo desde la fuente. La tarjeta
  «Broadcast Assets» de la landing queda pendiente de ese archivo.

## Notas de armado

- **Estructura**: la landing se queda en la raíz (la URL pública la sirve desde ahí) y todo lo que
  cuelga de ella —imágenes, tipografías, manual y packs— vive en `assets/`, `manual-de-marca/` y
  `downloads/`. Las referencias del HTML apuntan a esas carpetas.
- **`Mediakit.zip`** (el botón «Descargar .zip» de la landing y el de portada) contiene sólo el
  contenido de `downloads/`. La etiqueta del botón y la mención del FAQ decían «295 MB» por el tamaño
  del export original; ahora dicen el peso real: **85 MB**.
- **`assets/favicon.png`**: se redujo de 2048×2048 (3,2 MB) a 256×256 (46 KB) para no servir 3 MB en
  cada visita. El original de 2048 px sigue dentro de `downloads/Logos_betamina.zip`.
- **`assets/flag-es.png`**: en el export la bandera de España venía con nombre aleatorio
  (`mox7bl7r-image.png`); se guardó con el nombre que usa el HTML.
- **`assets/mascota-mediakit.png`**: es el render de la mascota que origina la imagen de portada;
  venía con nombre aleatorio (`mox3txdx-Gemini_Generated_Image…png`).
- **`manual-de-marca/BETAMINA-BRAND-MANUAL.pdf`**: es el mismo documento que viaja dentro de
  `downloads/Manuales de marca.zip` (junto a los otros dos PDF), acá suelto para poder abrirlo sin
  descomprimir.
- **`downloads/Paleta_de_colores.zip`**: se armó con los dos archivos de la paleta (`paleta-color.css`
  y `paleta-color.json`) que sí venían sueltos en el export.
- Los archivos de tipografía **conservan el nombre del export original** (`mox3cc…-FTCalhern-*.otf`)
  porque así los referencia el CSS de la landing; renombrarlos la rompe.
- Quedaron afuera de la entrega: los borradores intermedios de la landing, las copias duplicadas de
  imágenes con nombre aleatorio (eran el mismo archivo que las versiones con nombre definitivo) y las
  capturas del proceso de diseño que no son assets de marca (versiones previas de las tarjetas de
  paleta y gradiente, un placeholder «Mediakit» y una captura de una plantilla de FAQ genérica).

## Créditos

Diseño y desarrollo: **Dendra**. Los assets de marca pertenecen a Betamina.
