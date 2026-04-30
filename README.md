<<<<<<< HEAD
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

=======
IyBCYmV0aGxlaGVtIERlc2lnbiBBc3NldHMKCkRlc2lnbiBzeXN0ZW0gbGlicmFyeSBjdXJhZG8gcGFyYSBsb3MgcHJveWVjdG9zIGRlICoqQmFrZXJ5IEJldGhsZWhlbSBMTEMqKi4gIApCYXNhZG8gZW4gW25leHUtaW8vb3Blbi1kZXNpZ25dKGh0dHBzOi8vZ2l0aHViLmNvbS9uZXh1LWlvL29wZW4tZGVzaWduKSAoQXBhY2hlLTIuMCksIGZpbHRyYWRvIHkgZXh0ZW5kaWRvIHBhcmEgbnVlc3RybyBzdGFjay4KCi0tLQoKIyMgRXN0cnVjdHVyYQoKYGBgCmJiZXRobGVoZW0tZGVzaWduLwrilJzilIDilIAgc2tpbGxzLyAgICAgICAgICAgICAgIyBQbGFudGlsbGFzIGRlIFVJICgyNCBza2lsbHMpCuKUnOKUgOKUgCBkZXNpZ24tc3lzdGVtcy8gICAgICAjIFNpc3RlbWFzIGRlIGRpc2XDsW8gKDE1IHNpc3RlbWFzKQrilJTilIDilIAgQ0xBVURFLm1kICAgICAgICAgICAgIyBJbnN0cnVjY2lvbmVzIHBhcmEgQ2xhdWRlIENvZGUKYGBgCgotLS0KCiMjIFNraWxscyBkaXNwb25pYmxlcwoKfCBTa2lsbCB8IFVzbyBwcmluY2lwYWwgfAp8LS0tLS0tLXwtLS0tLS0tLS0tLS0tLXwKfCBgZGFzaGJvYXJkYCB8IEFkbWluIC8gYW5hbHl0aWNzIGNvbiBzaWRlYmFyIHwKfCBgbW9iaWxlLWFwcGAgfCBQYW50YWxsYXMgY29uIGZyYW1lIGlQaG9uZS9QaXhlbCB8CnwgYG1vYmlsZS1vbmJvYXJkaW5nYCB8IEZsdWpvIGRlIG9uYm9hcmRpbmcgMyBwYW50YWxsYXMgfAp8IGBzYWFzLWxhbmRpbmdgIHwgSGVybyArIGZlYXR1cmVzICsgcHJpY2luZyArIENUQSB8CnwgYHdlYi1wcm90b3R5cGVgIHwgTGFuZGluZyBwYWdlIGdlbmVyYWwgfAp8IGBibG9nLXBvc3RgIHwgQXJ0w61jdWxvIGVkaXRvcmlhbCBsYXJnbyB8CnwgYGRvY3MtcGFnZWAgfCBEb2N1bWVudGFjacOzbiAzIGNvbHVtbmFzIHwKfCBgZW1haWwtbWFya2V0aW5nYCB8IEVtYWlsIEhUTUwgZGUgcHJvZHVjdG8gfAp8IGBzb2NpYWwtY2Fyb3VzZWxgIHwgQ2FycnVzZWwgMTA4MMOXMTA4MCBwYXJhIHJlZGVzIHwKfCBgaW52b2ljZWAgfCBGYWN0dXJhIC8gY290aXphY2nDs24gUERGIHwKfCBga2FuYmFuLWJvYXJkYCB8IEJvYXJkIGRlIHRhcmVhcyBzbmFwc2hvdCB8CnwgYGZpbmFuY2UtcmVwb3J0YCB8IFJlcG9ydGUgZWplY3V0aXZvIGZpbmFuY2llcm8gfAp8IGB3ZWVrbHktdXBkYXRlYCB8IEFjdHVhbGl6YWNpw7NuIHNlbWFuYWwgZGVsIGVxdWlwbyB8CnwgYG1lZXRpbmctbm90ZXNgIHwgQWN0YSBkZSByZXVuacOzbiB8CnwgYHBtLXNwZWNgIHwgRXNwZWNpZmljYWNpw7NuIGRlIHByb2R1Y3RvIHwKfCBgaHItb25ib2FyZGluZ2AgfCBQbGFuIGRlIG9uYm9hcmRpbmcgZGUgZW1wbGVhZG8gfAp8IGBlbmctcnVuYm9va2AgfCBSdW5ib29rIGRlIGluY2lkZW50ZSB8CnwgYHRlYW0tb2tyc2AgfCBPS1JzIGRlbCBlcXVpcG8gfAp8IGBwcmljaW5nLXBhZ2VgIHwgVGFibGEgZGUgcHJlY2lvcyBzdGFuZGFsb25lIHwKfCBgc2ltcGxlLWRlY2tgIHwgRGVjayBtaW5pbWFsIGhvcml6b250YWwgfAp8IGBtYWdhemluZS1wb3N0ZXJgIHwgUMOzc3RlciBlZGl0b3JpYWwgfAp8IGBkaWdpdGFsLWVndWlkZWAgfCBFLWd1aWRlIGRvcyBjb2x1bW5hcyB8CnwgYHdpcmVmcmFtZS1za2V0Y2hgIHwgV2lyZWZyYW1lIGRlIGJhamEgZmlkZWxpZGFkIHwKCi0tLQoKIyMgRGVzaWduIFN5c3RlbXMgZGlzcG9uaWJsZXMKCnwgU2lzdGVtYSB8IFVzbyByZWNvbWVuZGFkbyB8CnwtLS0tLS0tLS18LS0tLS0tLS0tLS0tLS0tLXwKfCBgd2FybS1lZGl0b3JpYWxgIHwg4q2QIExhbmRpbmcgYmFrZXJ5LCBtZW7DuiwgbWFya2V0aW5nIHwKfCBgbm90aW9uYCB8IOKtkCBBcHBzIGludGVybmFzLCBkYXNoYm9hcmRzIG9wZXJhdGl2b3MgfAp8IGBsaW5lYXItYXBwYCB8IOKtkCBDYWtlIE9yZGVycyBBcHAsIGludGVyZmFjZXMgdMOpY25pY2FzIHwKfCBgc3RyaXBlYCB8IOKtkCBDb3RpemFjaW9uZXMsIHBhZ29zLCBmb3JtdWxhcmlvcyB8CnwgYGRlZmF1bHRgIHwgTmV1dHJhbCBtb2Rlcm5vLCBjb21vZMOtbiB8CnwgYHZlcmNlbGAgfCBEZXBsb3kgdG9vbHMsIGRvY3MgdMOpY25pY29zIHwKfCBgY3Vyc29yYCB8IEhlcnJhbWllbnRhcyBkZXYgfAp8IGBzdXBhYmFzZWAgfCBEYXNoYm9hcmRzIGNvbiBkYXRhIHwKfCBgc2hvcGlmeWAgfCBFLWNvbW1lcmNlLCBjYXTDoWxvZ29zIHwKfCBgYWlyYm5iYCB8IEJvb2tpbmcsIGxpc3RpbmdzIHwKfCBgYXBwbGVgIHwgQ2xlYW4sIHByZW1pdW0gfAp8IGBmaWdtYWAgfCBQcm90b3RpcG9zLCBkZXNpZ24gdG9vbHMgfAp8IGBzcG90aWZ5YCB8IERhcmsgbW9kZSwgbWVkaWEgfAp8IGB3aXJlZGAgfCBFZGl0b3JpYWwgdGVjbm9sb2fDrWEgfAp8IGByZXNlbmRgIHwgRW1haWwsIHRyYW5zYWNjaW9uYWwgfAoKLS0tCgojIyBDw7NtbyB1c2FybG8gZW4gdW4gcHJveWVjdG8KCiMjIyBPcGNpw7NuIDEg4oCUIEdpdCBzdWJtb2R1bGUgKHJlY29tZW5kYWRvKQoKYGBgYmFzaAojIEVuIGxhIHJhw616IGRlbCBwcm95ZWN0bwpnaXQgc3VibW9kdWxlIGFkZCBodHRwczovL2dpdGh1Yi5jb20vQmJldGhsZWhlbS9iYmV0aGxlaGVtLWRlc2lnbiBkZXNpZ24tYXNzZXRzCmdpdCBzdWJtb2R1bGUgdXBkYXRlIC0taW5pdApgYGAKClBhcmEgYWN0dWFsaXphciBjdWFuZG8gaGF5YSBjYW1iaW9zOgpgYGBiYXNoCmdpdCBzdWJtb2R1bGUgdXBkYXRlIC0tcmVtb3RlCmBgYAoKIyMjIE9wY2nDs24gMiDigJQgQ29waWEgZGlyZWN0YQoKRGVzY2FyZ2EgZWwgcmVwbyB5IGNvcGlhIGxhIGNhcnBldGEgYGRlc2lnbi1hc3NldHMvYCBhIHR1IHByb3llY3RvLgoKLS0tCgojIyBDw7NtbyBsZSBkaWNlcyBhIENsYXVkZSBDb2RlIHF1ZSBsbyB1c2UKCkVsIGFyY2hpdm8gYENMQVVERS5tZGAgZW4gbGEgcmHDrXogZGVsIHJlcG8gbGUgZGEgaW5zdHJ1Y2Npb25lcyBhdXRvbcOhdGljYXMgYSBDbGF1ZGUgQ29kZS4gIApTaSB1c2FzIHN1Ym1vZHVsZSwgYWdyZWdhIGVzdG8gYSB0dSBgQ0xBVURFLm1kYCBkZWwgcHJveWVjdG86CgpgYGBtYXJrZG93bgojIyBEZXNpZ24gQXNzZXRzCkxlZSBgZGVzaWduLWFzc2V0cy9DTEFVREUubWRgIGFudGVzIGRlIGNyZWFyIGN1YWxxdWllciBjb21wb25lbnRlIGRlIFVJLgpgYGAKCi0tLQoKIyMgQWdyZWdhciB1biBkZXNpZ24gc3lzdGVtIGN1c3RvbSAoQmFrZXJ5IEJldGhsZWhlbSBicmFuZCkKCjEuIENyZWEgYGRlc2lnbi1zeXN0ZW1zL2Jha2VyeS1iZXRobGVoZW0vREVTSUdOLm1kYAoyLiBEZWZpbmU6IGNvbG9yZXMsIHRpcG9ncmFmw61hLCBjb21wb25lbnRlcywgdm96IGRlIG1hcmNhCjMuIENvbW1pdCB5IHB1c2gg4oCUIHRvZG9zIGxvcyBwcm95ZWN0b3MgbG8gcmVjaWJlbiBjb24gYGdpdCBzdWJtb2R1bGUgdXBkYXRlIC0tcmVtb3RlYAoKLS0tCgojIyBDcsOpZGl0b3MKCi0gU2tpbGxzIHkgZGVzaWduIHN5c3RlbXMgYmFzZTogW25leHUtaW8vb3Blbi1kZXNpZ25dKGh0dHBzOi8vZ2l0aHViLmNvbS9uZXh1LWlvL29wZW4tZGVzaWduKSDigJQgQXBhY2hlLTIuMAotIEN1cmFjacOzbiB5IGV4dGVuc2nDs246IEJha2VyeSBCZXRobGVoZW0gTExDCgo=
>>>>>>> e0719f941897621f61c91aaef6e1bf2cc1325099
