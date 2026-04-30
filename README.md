# Bbethlehem Design Assets

Design system library curado para los proyectos de **Bakery Bethlehem LLC**.  
Basado en [nexu-io/open-design](https://github.com/nexu-io/open-design) (Apache-2.0), filtrado y extendido para nuestro stack.

---

## Estructura

```
bbethlehem-design/
├── skills/              # Plantillas de UI (24 skills)
├── design-systems/      # Sistemas de diseño (15 sistemas)
└── CLAUDE.md            # Instrucciones para Claude Code
```

---

## Skills disponibles

| Skill | Uso principal |
|-------|--------------|
| `dashboard` | Admin / analytics con sidebar |
| `mobile-app` | Pantallas con frame iPhone/Pixel |
| `mobile-onboarding` | Flujo de onboarding 3 pantallas |
| `saas-landing` | Hero + features + pricing + CTA |
| `web-prototype` | Landing page general |
| `blog-post` | Artículo editorial largo |
| `docs-page` | Documentación 3 columnas |
| `email-marketing` | Email HTML de producto |
| `social-carousel` | Carrusel 1080×1080 para redes |
| `invoice` | Factura / cotización PDF |
| `kanban-board` | Board de tareas snapshot |
| `finance-report` | Reporte ejecutivo financiero |
| `weekly-update` | Actualización semanal del equipo |
| `meeting-notes` | Acta de reunión |
| `pm-spec` | Especificación de producto |
| `hr-onboarding` | Plan de onboarding de empleado |
| `eng-runbook` | Runbook de incidente |
| `team-okrs` | OKRs del equipo |
| `pricing-page` | Tabla de precios standalone |
| `simple-deck` | Deck minimal horizontal |
| `magazine-poster` | Póster editorial |
| `digital-eguide` | E-guide dos columnas |
| `wireframe-sketch` | Wireframe de baja fidelidad |

---

## Design Systems disponibles

| Sistema | Uso recomendado |
|---------|----------------|
| `warm-editorial` | ⭐ Landing bakery, menú, marketing |
| `notion` | ⭐ Apps internas, dashboards operativos |
| `linear-app` | ⭐ Cake Orders App, interfaces técnicas |
| `stripe` | ⭐ Cotizaciones, pagos, formularios |
| `default` | Neutral moderno, comodín |
| `vercel` | Deploy tools, docs técnicos |
| `cursor` | Herramientas dev |
| `supabase` | Dashboards con data |
| `shopify` | E-commerce, catálogos |
| `airbnb` | Booking, listings |
| `apple` | Clean, premium |
| `figma` | Prototipos, design tools |
| `spotify` | Dark mode, media |
| `wired` | Editorial tecnología |
| `resend` | Email, transaccional |

---

## Cómo usarlo en un proyecto

### Opción 1 — Git submodule (recomendado)

```bash
# En la raíz del proyecto
git submodule add https://github.com/Bbethlehem/bbethlehem-design design-assets
git submodule update --init
```

Para actualizar cuando haya cambios:
```bash
git submodule update --remote
```

### Opción 2 — Copia directa

Descarga el repo y copia la carpeta `design-assets/` a tu proyecto.

---

## Cómo le dices a Claude Code que lo use

El archivo `CLAUDE.md` en la raíz del repo le da instrucciones automáticas a Claude Code.  
Si usas submodule, agrega esto a tu `CLAUDE.md` del proyecto:

```markdown
## Design Assets
Lee `design-assets/CLAUDE.md` antes de crear cualquier componente de UI.
```

---

## Agregar un design system custom (Bakery Bethlehem brand)

1. Crea `design-systems/bakery-bethlehem/DESIGN.md`
2. Define: colores, tipografía, componentes, voz de marca
3. Commit y push — todos los proyectos lo reciben con `git submodule update --remote`

---

## Créditos

- Skills y design systems base: [nexu-io/open-design](https://github.com/nexu-io/open-design) — Apache-2.0
- Curación y extensión: Bakery Bethlehem LLC

