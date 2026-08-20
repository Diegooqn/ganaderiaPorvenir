# Ganadería El Porvenir — sitio web

Sitio estático (sin build) para `ganaderiaporvenir.com`, con la misma arquitectura que usaste en `ong-vida-biodiversidad`: un solo `index.html`, `_headers` para Cloudflare Pages, y una carpeta `documentos/` para PDFs públicos.

## Estructura
- `index.html` — toda la página (HTML + CSS + JS inline).
- `_headers` — cabeceras de seguridad y de caché para Cloudflare Pages.
- `documentos/` — 4 PDF del Régimen Tributario Especial (RTE): informe anual de gestión y resultados, certificación de requisitos, acta de asamblea de autorización y certificación de antecedentes judiciales. Listados en la sección "Documentos y trazabilidad".
- `assets/` — `logo.png` (optimizado a 300px de ancho, ~145KB). Integrado en el header y el footer.

## Pendientes antes de publicar
1. Añadir fotos reales de la finca/ganado en `assets/` (opcional, mejora mucho la página).
2. Revisar los textos de "Quiénes somos" y ajustar si algo no refleja la realidad del negocio.
3. Cuando lleguen más documentos oficiales (RUT, Cámara de Comercio, registro ICA, hierro/marca), agregarlos a `documentos/` y a la lista de la sección "Documentos".

## Publicar en Cloudflare Pages (igual que tu otro sitio)
1. Sube esta carpeta a un repositorio de GitHub (por ejemplo `ganaderia-el-porvenir`).
2. En el dashboard de Cloudflare → Workers & Pages → Create → Pages → Connect to Git, selecciona el repo.
3. Build command: (vacío). Output directory: `/` (raíz).
4. Despliega, luego en la pestaña "Custom domains" del proyecto agrega `ganaderiaporvenir.com` (y `www.ganaderiaporvenir.com` si quieres) — como el dominio ya está comprado, solo falta apuntar sus DNS a Cloudflare o, si ya está en tu cuenta de Cloudflare, activar el dominio ahí mismo.
