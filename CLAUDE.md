# CLAUDE.md — biosaludclaret.org (sitio público)

Sitio web **público** de la Casa de la Biosalud Claret (Misioneros Claretianos
de Honduras, Arizona, Atlántida). HTML + CSS estático, **sin build ni
frameworks**. Vercel despliega cada commit a `main` en `biosaludclaret.org`
(~1 minuto).

## Relación con el sistema interno

- La gestión de pacientes (expedientes, citas, recetas) es **otro proyecto**
  y vive en `sistema.biosaludclaret.org`.
- Este repo solo aporta el redirect `/sistema` → `https://sistema.biosaludclaret.org`
  (definido en `vercel.json`).
- Aquí **nunca** va código del sistema ni datos de pacientes: todo lo
  commiteado se sirve públicamente.

## Estructura

Todo vive en la **raíz** (no existen `/img/` ni `/assets/`):

- `index.html` — todo el contenido del sitio
- `styles.css` — estilos
- `vercel.json` — headers de seguridad/caché y el redirect `/sistema`
- `robots.txt`, `sitemap.xml`
- Imágenes en la raíz: `logo-hero.png`, `symbol-bosque.png` (nav),
  `symbol-hueso.png` (footer), `symbol-brasa.png`, `og-image.png`,
  `favicon.ico`, `favicon-32.png`, `apple-touch-icon.png`

Imágenes nuevas también van en la raíz y se referencian sin carpeta.

## Reglas de edición (el cliente edita desde GitHub web, no es técnico)

- Cambios de texto/precios/productos/testimonios: editar `index.html`
  directamente; mantener el HTML simple y los textos en **español**.
- No mover archivos a subcarpetas ni renombrar imágenes: romperían las
  referencias y la memoria del cliente sobre "cómo se edita".
- No tocar `vercel.json`, `robots.txt` ni `sitemap.xml` salvo necesidad real;
  explicar el cambio en el commit.
- Commits descriptivos en español. `main` es producción: verificar el HTML
  antes de commitear (no hay CI ni build que atrape errores).
- Datos de contacto reales del titular (RTN, WhatsApp, correo) están en el
  README; si cambian, actualizar `index.html` y README juntos.
