# Centro Quiropráctico Talledos — landing

Sitio estático (un solo `index.html`). Sin build ni dependencias.

## Desplegar en Cloudflare
- Workers: `npx wrangler login` y luego `npx wrangler deploy`
- Pages: `npx wrangler pages deploy public --project-name talledos-quiropractico`
- Con repo: framework "None", build command vacío, output directory `public`.

## Antes de publicar
1. WhatsApp: en `index.html` busca `var PH=` y confirma que 664 531 5429 (Otay) y 664 187 4429 (Centro) reciben WhatsApp. Si no, cambia los números (formato 52 + 10 dígitos).
2. Dirección Otay: una reseña de Google dice que la dirección del mapa no es correcta. Confirma el punto exacto y ajusta el parámetro `q=` del iframe y el `destination=` del botón "Cómo llegar".
3. Logo: está en `assets/logo.png` (recortado del que enviaron). Si tienen el logo en SVG o PNG con fondo transparente, reemplázalo con el mismo nombre.
4. Servicios: los textos son de ejemplo. Ajusta a lo que ofrece el centro, con precios si quieren mostrarlos.
5. Reseñas: son citas reales de Google; confirma con el cliente que están de acuerdo en mostrarlas.
6. Coolvetica: copia `Coolvetica.woff2` a `public/assets/` y descomenta el `@font-face` (requiere licencia comercial).
7. Agrega `og:image` con URL absoluta cuando tengas dominio y foto.
