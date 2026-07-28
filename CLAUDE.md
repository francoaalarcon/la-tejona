# LA TEJONA — Proyecto Web

## Estado actual
**Versión:** v0.1.0  
**Fase:** Diseño / Landing pages HTML  
**Última sesión:** 2026-07-28  
**Repo:** https://github.com/francoaalarcon/la-tejona  
**Directorio local:** /home/franco/tejona  

---

## Estructura del proyecto

```
la-tejona/
├── version-1/          # Estilo EQUIP — marketplace B2B oscuro
│   ├── index.html
│   └── assets/         # Imágenes propias de esta versión
├── version-2/          # Estilo Pacasmayo — institucional limpio
│   ├── index.html
│   └── assets/         # Imágenes propias de esta versión
├── imagenes/           # Carpeta original de assets del cliente
├── sessions/           # Reportes de sesión
├── d1.png              # Diseño de referencia v1 (EQUIP)
├── d2.png              # Diseño de referencia v2 (Pacasmayo)
└── CLAUDE.md
```

---

## Sistema de diseño

### Paleta de colores (extraída de latejona.com)
| Rol | Hex |
|---|---|
| Azul principal (CTA, links) | `#0089e4` |
| Navy oscuro (navbar, footer) | `#192730` |
| Negro (texto) | `#000000` |
| Gris claro (fondo página) | `#f6f6f8` |
| Gris suave (secciones alt.) | `#ecedef` |
| Off-white (cards) | `#FBFCFF` |
| Blanco | `#ffffff` |
| Gris bordes | `#dddddd` |
| Dorado/acento v1 | `#e8a020` |

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
