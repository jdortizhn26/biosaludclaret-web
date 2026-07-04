# Casa de la Biosalud Claret — Sitio Web

Sitio público de la Casa de la Biosalud Claret, proyecto de los Misioneros Claretianos de Honduras (Arizona, Atlántida).

## Cómo editar el sitio

Todo el contenido vive en `index.html`. Para cambiar texto, precios, productos o testimonios:

1. Abrí este repo en GitHub: `github.com/jdortizhn26/biosaludclaret-web`
2. Click sobre `index.html` → click el ícono de lápiz (✏️) arriba derecha
3. Editá lo que necesités directamente en el navegador
4. Bajá hasta abajo → "Commit changes" → "Commit changes" otra vez
5. En 60 segundos Vercel ya republicó el sitio en `biosaludclaret.org`

Para cambios de estilo, abrí `styles.css` con el mismo procedimiento.

## Estructura

Todos los archivos viven en la **raíz del repo** (no hay carpetas `/img/` ni `/assets/`):

```
biosaludclaret-web/
├── index.html              ← Contenido del sitio (HTML)
├── styles.css              ← Estilos
├── vercel.json             ← Configuración de Vercel (headers, redirect /sistema)
├── robots.txt              ← Permite a Google indexar
├── sitemap.xml             ← Mapa del sitio para buscadores
├── logo-hero.png           ← Logo lockup completo (sección héroe)
├── symbol-bosque.png       ← Símbolo color Bosque (nav)
├── symbol-hueso.png        ← Símbolo color Hueso (footer)
├── symbol-brasa.png        ← Símbolo color Brasa (decorativo)
├── og-image.png            ← Imagen de previa al compartir en WhatsApp/FB
├── favicon.ico             ← Icono del navegador
├── favicon-32.png          ← Icono del navegador (32px)
└── apple-touch-icon.png    ← Icono al guardar en pantalla de inicio (iOS)
```

> El pack completo del rebranding (logo original y las variantes de color del
> símbolo) **no** está en este repo; solo se suben las imágenes que la web usa.
> Si se agrega una imagen nueva, va también en la raíz y se referencia sin
> carpeta (ej. `src="foto-local.png"`).

## Stack

- HTML + CSS estático (sin frameworks, sin build)
- Tipografías: Bricolage Grotesque + Manrope (Google Fonts)
- Mapa: Google Maps embed
- WhatsApp: link wa.me
- Hosting: Vercel (despliega automáticamente cada commit a `main`)
- Dominio: biosaludclaret.org

## Sistema interno

El sistema de gestión de pacientes es un proyecto aparte y vive en
`sistema.biosaludclaret.org`. Desde este sitio, la ruta `/sistema` redirige
ahí (configurado en `vercel.json`). En este repo **no** va nada del sistema
ni datos de pacientes.

## Cambios estructurales (sección nueva, rediseño)

Para cambios mayores que no se hagan editando texto, coordinar con Claude/Daniel.

## Datos del titular

Asociación de Misioneros Claretianos de Honduras  
RTN: 08019021286302  
WhatsApp: +504 9812-0271  
Correo: hola@biosaludclaret.org  
Ubicación: Arizona, Atlántida, Honduras
