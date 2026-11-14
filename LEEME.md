# Visitas de Campo: publicar la app para usarla en el campo

Esta carpeta es la app completa. Publicada en una web propia (HTTPS) funciona **sin conexión**, con GPS, grabación de tracks, descarga de zonas PNOA y dictado por voz.

## Opción A: GitHub Pages (gratis, unos 10 minutos)
1. Crea una cuenta en https://github.com (si no la tienes).
2. Pulsa **New repository** → nombre, por ejemplo, `visitas-campo` → **Public** → **Create repository**.
3. En el repositorio: **Add file → Upload files** → arrastra **todos los archivos de esta carpeta** (index.html, sw.js, manifest.webmanifest, icon-192.png, icon-512.png) → **Commit changes**.
4. Ve a **Settings → Pages** → en *Branch* elige `main` y carpeta `/ (root)` → **Save**.
5. En un par de minutos la app estará en: `https://TU-USUARIO.github.io/visitas-campo/`

## Opción B: Netlify Drop (sin cuenta de GitHub)
1. Entra en https://app.netlify.com/drop
2. Arrastra esta carpeta completa. Te da una dirección https al instante (crea una cuenta gratuita para que no caduque).

## Instalarla en el móvil
- **Android (Chrome):** abre la dirección → menú ⋮ → **Instalar aplicación** (o el botón «Instalar app» en ⚙️).
- **iPhone (Safari):** abre la dirección → **Compartir → Añadir a pantalla de inicio**.

## Antes de salir al campo (con wifi)
1. Abre la app instalada → ⚙️ → **Mapas sin conexión → Descargar zona de ortofoto PNOA**.
2. Indica el centro (coordenadas, «Mi posición» o «Visita actual»), el radio y el detalle → **Descargar zona**.
3. Opcional: **Cargar ortofoto propia** (JPG + .jgw, KMZ o GeoTIFF).

## Actualizar la app
Sustituye `index.html` por la nueva versión y cambia el texto `VERSION` dentro de `sw.js` (por ejemplo, `visitas-v4`). Los datos guardados en los móviles no se pierden.

## Notas
- Los datos (borradores, fotos, mapas) se guardan solo en cada dispositivo; no se envían a ningún servidor.
- Ortofoto: PNOA máxima actualidad, © IGN, licencia CC BY 4.0 scne.es (la atribución se incluye automáticamente en el croquis).
- Mientras se graba un track, mantén la app abierta y la pantalla encendida.
