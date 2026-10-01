# El Roble de Aritz — Prototipo Web

Prototipo estático del restaurante tradicional de leña "El Roble de Aritz" (Vitoria).
Proyecto académico de Ingeniería Web con HTML y CSS, sin JavaScript (página web estática).

## Páginas

| Página | Contenido |
|---|---|
| `index.html` | Inicio: concepto, platos estrella y ubicación (con mapa embebido). |
| `carta.html` | Carta de temporada (entrantes, principales, postres) con detalle de cada plato en modal solo con CSS. |
| `experiencia.html` | Menú degustación "Brasa Viva" (8 pases), origen de ingredientes y detalles prácticos, más vídeo de presentación. |
| `reservas.html` | Formulario de reserva (contacto, fecha/hora, comensales, documento adjunto para eventos privados, turno, alergias, observaciones) y política de cancelación. |
| `style.css` | Hoja de estilos única para todo el sitio. |
| `images/` | Logo, favicon e imágenes por sección (`index/`, `carta/`, `experiencia/`); `experiencia/` incluye además el vídeo del menú (`menu_degustacion.mp4`). |

## Ver el proyecto

- **Local:** no requiere instalación ni servidor, basta con abrir `index.html` en el navegador.
- **Online:** desplegado con Cloudflare Workers en [El Roble de Aritz](https://el-roble-de-aritz.aritz-gsc.workers.dev/). El despliegue se actualiza automáticamente al hacer push a GitHub.

## Uso de la IA

Todo lo que se pidió a la IA (salvo fotos y vídeo) se pidió a **Opencode (Muse Spark 1.3)**: un agente de código que trabaja en local sobre los ficheros del proyecto, así que lee y revisa el HTML y el CSS reales en lugar de pegar trozos de código en un chat. Las imágenes y el vídeo se generaron aparte, con Seedream + Seedance.

Según lo indicado en los comentarios de `index.html` y `style.css`:

- **HTML (hecho a mano):** la organización de los bloques es propia. Opencode (Muse Spark 1.3) solo ayudó a rellenar algunos textos y a explicar el uso de elementos como `figure`, `iframe` y `details`. Las imágenes y el vídeo se generaron con Seedream + Seedance.
- **CSS (con apoyo de IA, revisado a mano):** Opencode (Muse Spark 1.3) propuso la mayoría del diseño final (colores, fuentes, distribución y tamaños) sin tocar el HTML. Después todo se revisó y retocó manualmente (interacciones, tamaños, etc.).
- **Responsive:** hecho 100 % con Opencode (Muse Spark 1.3). Creo que no se pedía, pero me daba TOC dejarlo sin hacer :P

### ¿Por qué Opencode y no ChatGPT, Gemini o Claude?

Porque no es solo un chat: lleva skills y agentes instalados que me ayudan a aprender y a entender cada decisión de diseño en lugar de copiarme el resultado. Y como trabaja directamente sobre los ficheros del proyecto, las propuestas se hacen sobre la marcha y con el diseño real delante, que es lo que permitió pulirlo hasta dejarlo así.
