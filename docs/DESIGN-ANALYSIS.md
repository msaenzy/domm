# DESIGN-ANALYSIS — DOMM · Portafolio 2026

Fuente: `portafolio_domm_2026.pdf` (2 páginas largas, 1920 pt de ancho). Se trabajó en base 1440 px.

## Estructura detectada
1. **Hero** — óvalo blanco sobre forma roja con logotipo DOMM + «PORTAFOLIO».
2. **Programa Vacacional GD** — verde `#00a719`.
3. **Gente y Cultura (TH)** — verde oliva `#789d00`.
4. **Comunicación interna** — verde `#00ad19`.
5. **Equipos Ágiles** — verde oscuro `#026e32`.
6. **Orgullosamente Ecuatorianos** — azul marino `#1f396b`.
7. **IMPULSO – Academia de Emprendedores GD** — verde `#009d38`.

Cada sección repite el mismo patrón: llama + barra de color con título → introducción en 3 columnas con filetes verticales → galería de piezas con etiqueta de color.

## Sistema de diseño
- **Tipografías (extraídas del PDF):** Sora Light/Regular (títulos y texto) y Poppins Regular/SemiBold (etiquetas de paleta) — Google Fonts.
- **Color base:** tinta `#282347`, rojo llama `#e92e21`, fondo blanco. Paletas de marca mostradas en el PDF: Gente y Cultura (`#79A60D #F48644 #FCAE2A #8447C1 #4DB7F4`) e IMPULSO (`#ff7f00 #009d45 #ffb300 #606060`).
- **Forma:** plano, sin sombras; radios 12–20 px en cajas y muestras.
- **Movimiento:** fade-up corto, una sola vez; sin parallax.

## Recursos
- Vectoriales del PDF convertidos a SVG: fondo del hero, logotipo DOMM, «PORTAFOLIO», llama, Gente y Cultura, Bienestar, SSA, Salario Emocional, Equipos Ágiles (+ isotipo), IMPULSO (logotipo, elementos, backing).
- Rasters originales extraídos (piezas y fotos), optimizados a máx. 1400 px.
- Recortes del PDF a PNG (vector + foto enmascarada): `oe-key-visual.png`, `oe-generacion-d.png`.
- `og-image.jpg` generada desde el hero; favicon = llama.

## ASSUMPTION (decisiones no explícitas en el PDF)
- **Navegación fija** con 6 enlaces (el PDF no tiene menú). Etiquetas abreviadas: Vacacional GD, Comunicación, Ecuatorianos.
- **Pie de página** con © 2026 DOMM.
- **Correcciones ortográficas** del texto: «calidéz» → «calidez», «Convoctorias» → «Convocatorias»; «Desde de comunicación» se conservó como «Desde comunicación».
- **Recomposición móvil:** columnas apiladas, filetes verticales pasan a horizontales, texto justificado solo desde 768 px.
- **Etiquetas verdes** oscurecidas un 20 % (`color-mix`) para llegar a contraste AA con texto blanco pequeño; las barras de título usan el color exacto del PDF.
- **Muestras de color:** el fondo usa el hex impreso en el PDF (el relleno del PDF varía levemente); el texto de la etiqueta cambia entre blanco y tinta según contraste.
- Títulos de sección con mínimo 24 px para cumplir contraste de texto grande.

## Pendientes / avisos
- **Contraste** de la etiqueta hex en las muestras `#009d45` y `#ffb300`/`#ff7f00` queda por debajo de 4.5:1 con ambas tintas; es información secundaria fiel al PDF.
- **MISSING ASSET:** ninguno. `placeholder.svg` existe solo como respaldo del scaffold.
- Fuentes: requieren conexión a Google Fonts (en el sandbox de auditoría se bloquearon; el sitio cae a la tipografía del sistema).
- `canonical` / `og:url` / `og:image` absolutos: rellenar cuando exista la URL final.
