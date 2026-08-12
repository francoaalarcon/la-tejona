# LA TEJONA — Proyecto Web

## Estado actual
**Versión:** v0.1.0  
**Fase:** Diseño / Prototipo HTML completo (version-3 con 12 páginas + catálogo dinámico)  
**Última sesión:** 2026-08-12  
**Repo:** https://github.com/francoaalarcon/la-tejona  
**Directorio local:** /home/franco/tejona  

---

## Estructura del proyecto

```
la-tejona/
├── version-1/          # Estilo EQUIP — marketplace B2B oscuro
│   ├── index.html
│   └── assets/
├── version-2/          # Estilo Pacasmayo — institucional limpio
│   ├── index.html
│   └── assets/
├── version-3/          # ★ VERSIÓN ACTIVA — visual v1 + estructura v2
│   ├── index.html      # Landing principal con carousel hero
│   ├── nosotros.html
│   ├── productos.html  # Overview de categorías (4 destacados)
│   ├── catalogo.html   # ★ Tienda estilo WooCommerce — 50 productos con filtros
│   ├── producto.html   # ★ Página individual dinámica (?sku=XXXX)
│   ├── producto-single.html  # Template estático de referencia (TD244)
│   ├── proyectos.html
│   ├── novedades.html
│   ├── contacto.html
│   ├── privacidad.html
│   ├── cookies.html
│   ├── terminos.html
│   └── assets/         # 19 imágenes (9 nuevas específicas por producto)
├── imagenes/           # Carpeta original de assets del cliente
├── sessions/           # Reportes de sesión
├── d1.png              # Diseño de referencia v1 (EQUIP)
├── d2.png              # Diseño de referencia v2 (Pacasmayo)
└── CLAUDE.md
```

---

## Sistema de diseño

### Paleta de colores — identidad de marca La Tejona
| Rol | Hex |
|---|---|
| Rojo principal (CTA, links, acento) | `#cc0000` |
| Rojo oscuro (hover) | `#a80000` |
| Negro (navbar, footer, overlays) | `#1a1a1a` |
| Negro texto | `#000000` |
| Gris claro (fondo página) | `#f6f6f8` |
| Gris suave (secciones alt.) | `#ecedef` |
| Blanco | `#ffffff` |
| Gris bordes | `#dddddd` |
| Dorado/acento v1 stats | `#e8a020` |

### Tipografía
- **Version 1:** Poppins (headings 700/600) + Inter (body 400/500)
- **Version 2:** Montserrat (headings 700/600/500) + Open Sans (body 400/600)

### Assets principales
- Logo: `assets/TEJONA-LOGOS-E-IMAGENES-500X500.png`
- Hero bg: `assets/TEJONA-FOTOS-FONDOS-2.webp`
- Productos: TEJA-ESPANOLA-CERAMICA, FLEXITEJA-1, MAXIPLACA-2, TANQUE-BEIGE, TEJONA-PINTURAS
- Marcas: RIBEPAR-LOGO-HD, Mesa-de-trabajo (Duralit)

---

## Stack objetivo (WordPress)
- Cada versión se convertirá en tema WordPress independiente
- WooCommerce en modo catálogo (sin transacciones, solo visualización)
- Subpáginas: Productos, Marcas, Nosotros, Contacto

---

## Notas importantes
- Las landings son prototipos HTML para aprobación visual del cliente
- Cada versión tiene su propia carpeta `assets/` autocontenida
- El cliente aprueba una versión → se convierte a tema WordPress

---

## Historial de sesiones

### 2026-08-12 (sesión 2)
**Release:** sin release  
**Resumen:** Catálogo Duralit completo — tienda tipo WooCommerce con 50 productos, página individual dinámica por SKU y corrección total de enlaces en todas las páginas.  
**Cambios:**
- `version-3/catalogo.html` — página de catálogo estilo tienda con 50 productos Duralit, sidebar con filtros de categoría/color/búsqueda, grid responsivo, links a producto individual
- `version-3/producto.html` — página individual dinámica: lee `?sku=XXXX`, base de datos JS con 50 productos (specs, descripción, relacionados, galería de variantes)
- `version-3/producto-single.html` — template estático de referencia (ejemplo TD244)
- `version-3/assets/` — 9 imágenes específicas por color/categoría: TEJA-NATURAL, TEJA-ROJA, TEJA-LADRILLO, ROJO-CARMESI, TEJA-ESPANOLA-LADRILLO, MAXIPLACA-CEMENTO, PLACA-CEMENTICIA, TANQUE-NEGRO, TANQUE-SEPTICO
- Todos los navs (11 archivos) — "Productos" ahora apunta a `catalogo.html`; index.html usa páginas reales en vez de anclas internas
- Footer columna "Productos" (11 archivos) — links a `catalogo.html?cat=xxx` por categoría (teja-espanola, teja-duralit, maxiplaca, tanque, masilla)
- `index.html` — blog cards y "Ver todas las notas" apuntan a `novedades.html`

**Pendientes:**
- Revisión final del cliente de la version-3 completa (catálogo incluido)
- Agregar imágenes reales de cumbreras (no existen en imagenes/)
- Agregar imágenes de masillas/pernos cuando el cliente las provea
- Decisión: convertir version-3 a tema WordPress

### 2026-08-12
**Release:** sin release  
**Resumen:** Versión 3 completa — prototipo HTML con 9 páginas (landing + subpáginas + legales) aprobado visualmente por el cliente.  
**Cambios:**
- `version-3/index.html` — landing principal, visual v1 + estructura v2, carousel hero 3 slides, stats animados, marcas marquee, secciones Proceso/Categorías/Diferencial
- `version-3/nosotros.html` — página Historia, Misión/Visión, Valores, Stats
- `version-3/productos.html` — grid de categorías + 4 fichas de producto detalladas + marcas
- `version-3/proyectos.html` — 4 tipos de proyecto, proceso en 4 pasos, CTA
- `version-3/novedades.html` — artículo destacado + 9 cards de blog + newsletter
- `version-3/contacto.html` — formulario con validación JS, sucursales, mapa placeholder
- `version-3/privacidad.html` — Política de privacidad con layout 2 columnas (TOC sidebar + body)
- `version-3/cookies.html` — Política de cookies con tabla de cookies tipificadas
- `version-3/terminos.html` — Términos y condiciones (13 secciones, jurisdicción La Paz, Bolivia)
- Footer de las 9 páginas — actualizado con enlaces completos (Empresa + links legales en footer-bottom)

**Pendientes:**
- Revisión final del cliente de la versión 3 completa
- Decisión: convertir version-3 a tema WordPress

### 2026-07-28 (sesión 2)
**Release:** sin release  
**Resumen:** Corrección de paleta — rojo/negro de marca reemplaza azul/navy; assets integrados por versión.  
**Cambios:**
- `version-1/index.html` y `version-2/index.html` — paleta corregida: `#0089e4` → `#cc0000` (rojo), `#192730` → `#1a1a1a` (negro)
- `version-1/assets/` y `version-2/assets/` — cada versión ahora tiene su propia carpeta de imágenes autocontenida
- Rutas de imágenes actualizadas de `../imagenes/` a `assets/` local

**Pendientes:**
- Revisión visual del cliente con la paleta rojo/negro correcta
- Ajustes adicionales de diseño según feedback
- Definir cuál versión se convierte a WordPress

### 2026-07-28
**Release:** v0.1.0  
**Resumen:** Sesión inicial — setup del repo y creación de ambas landing pages HTML.  
**Cambios:**
- Repo GitHub creado (`francoaalarcon/la-tejona`) y clonado localmente
- Paleta de colores extraída de latejona.com
- Diseños d1.png (EQUIP) y d2.png (Pacasmayo) analizados
- `version-1/index.html` — landing estilo EQUIP/marketplace B2B (2371 líneas)
- `version-2/index.html` — landing estilo Pacasmayo/institucional
- `version-1/assets/` — 10 imágenes integradas
- `version-2/assets/` — 9 imágenes integradas
- Rutas actualizadas para que cada versión sea autocontenida

**Pendientes:**
- Revisión visual del cliente (las versiones aún no fueron aprobadas)
- Ajustes de diseño según feedback
- Definir cuál versión se convierte a WordPress
