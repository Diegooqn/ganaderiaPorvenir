# Ganadería El Porvenir — sitio web

Sitio estático (sin build) para `ganaderiaporvenir.com`, con la misma arquitectura que usaste en `ong-vida-biodiversidad`: un solo `index.html`, `_headers` para Cloudflare Pages, y una carpeta `documentos/` para PDFs públicos.

## Estructura
- `index.html` — toda la página (HTML + CSS + JS inline).
- `_headers` — cabeceras de seguridad y de caché para Cloudflare Pages.
- `documentos/` — vacía por ahora. La sección "Documentos y trazabilidad" del sitio muestra un aviso de "No disponible aún" en lo que llegan el RUT, el certificado de Cámara de Comercio, el registro ICA, etc.
- `assets/` — vacía por ahora. No hay logo todavía: el header y el footer solo muestran el nombre en texto. Cuando tengas el logo, colócalo aquí y avísame para integrarlo.

## Pendientes antes de publicar
1. Agregar el logo cuando lo tengas (`assets/`) y volver a mostrarlo en el header/footer.
2. Cuando tengas los documentos oficiales (RUT, Cámara de Comercio, registro ICA, hierro/marca), colócalos en `documentos/` y pide que se vuelva a activar la lista con el visor de PDF en la sección "Documentos".
3. Añadir fotos reales de la finca/ganado en `assets/` (opcional, mejora mucho la página).
4. Revisar los textos de "Quiénes somos" y ajustar si algo no refleja la realidad del negocio.

## Publicar en Cloudflare Pages (igual que tu otro sitio)
1. Sube esta carpeta a un repositorio de GitHub (por ejemplo `ganaderia-el-porvenir`).
2. En el dashboard de Cloudflare → Workers & Pages → Create → Pages → Connect to Git, selecciona el repo.
3. Build command: (vacío). Output directory: `/` (raíz).
4. Despliega, luego en la pestaña "Custom domains" del proyecto agrega `ganaderiaporvenir.com` (y `www.ganaderiaporvenir.com` si quieres) — como el dominio ya está comprado, solo falta apuntar sus DNS a Cloudflare o, si ya está en tu cuenta de Cloudflare, activar el dominio ahí mismo.
