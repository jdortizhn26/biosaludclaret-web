# Casa de la Biosalud Claret — Sitio Web

Sitio público de la Casa de la Biosalud Claret, proyecto de los Misioneros Claretianos de Honduras (Arizona, Atlántida).

## Cómo editar el sitio

Todo el contenido vive en `index.html`. Para cambiar texto, precios, productos o testimonios:

1. Abrí este repo en GitHub: `github.com/<tu-usuario>/biosaludclaret-web`
2. Click sobre `index.html` → click el ícono de lápiz (✏️) arriba derecha
3. Editá lo que necesités directamente en el navegador
4. Bajá hasta abajo → "Commit changes" → "Commit changes" otra vez
5. En 60 segundos Vercel ya republicó el sitio en `biosaludclaret.org`

Para cambios de estilo, abrí `styles.css` con el mismo procedimiento.

## Estructura

```
biosaludclaret-web/
├── index.html              ← Contenido del sitio (HTML)
├── styles.css              ← Estilos
├── vercel.json             ← Configuración de Vercel (headers, redirects)
├── robots.txt              ← Permite a Google indexar
├── sitemap.xml             ← Mapa del sitio para buscadores
├── /img/                   ← Imágenes usadas por la web (optimizadas)
│   ├── logo-hero.png       ← Logo lockup completo
│   ├── symbol-bosque.png   ← Símbolo color Bosque (para nav)
│   ├── symbol-hueso.png    ← Símbolo color Hueso (para footer)
│   ├── symbol-brasa.png    ← Símbolo color Brasa (decorativo)
│   ├── og-image.png        ← Imagen de previa al compartir en WhatsApp/FB
│   ├── favicon.ico         ← Icono del navegador
│   └── apple-touch-icon.png
└── /assets/                ← Pack completo del rebranding (originales)
    ├── logo-biosalud-claret.png
    ├── symbol-color-*.png (10 variantes de color)
    ├── symbol-light.png
    └── symbol-transparent.png
```

## Stack

- HTML + CSS estático (sin frameworks)
- Tipografías: Bricolage Grotesque + Manrope (Google Fonts)
- Mapa: Google Maps embed
- WhatsApp: link wa.me
- Hosting: Vercel
- Dominio: biosaludclaret.org

## Cambios estructurales (sección nueva, rediseño)

Para cambios mayores que no se hagan editando texto, coordinar con Claude/Daniel.

## Datos del titular

Asociación de Misioneros Claretianos de Honduras  
RTN: 08019021286302  
WhatsApp: +504 9812-0271  
Correo: hola@biosaludclaret.org  
Ubicación: Arizona, Atlántida, Honduras
