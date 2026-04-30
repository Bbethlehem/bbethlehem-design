# Design Assets — Instrucciones para Claude Code

## Regla fundamental
SIEMPRE leer el SKILL.md y el DESIGN.md relevante ANTES de escribir cualquier código de UI.
No improvisar colores, tipografía ni layouts.

## Flujo de trabajo

1. Identificar el skill adecuado en `skills/`
2. Leer su `SKILL.md` completo
3. Identificar el design system adecuado en `design-systems/`
4. Leer su `DESIGN.md` completo
5. Aplicar tokens exactos (colores hex, fuentes, espaciado) al código

## Skills por caso de uso — Bakery Bethlehem

| Necesito... | Usar skill |
|-------------|-----------|
| Panel de pedidos / ventas | `dashboard` |
| App móvil (cake orders) | `mobile-app` |
| Landing de la bakery | `saas-landing` o `web-prototype` |
| Cotización para cliente | `invoice` |
| Menú digital / TV | `magazine-poster` o `digital-eguide` |
| Email a clientes | `email-marketing` |
| Post para Instagram | `social-carousel` |
| Reporte semanal | `weekly-update` o `finance-report` |
| SOP / procedimiento | `pm-spec` o `eng-runbook` |

## Design systems por caso de uso — Bakery Bethlehem

| Contexto | Design system |
|----------|--------------|
| Cara al cliente (web/marketing) | `warm-editorial` |
| App interna (cake orders, dashboard) | `linear-app` |
| Documentos operativos | `notion` |
| Formularios de pago / cotización | `stripe` |

## Reglas de marca Bakery Bethlehem
- Tono: cálido, artesanal, colombiano, profesional
- Nunca usar gradientes agresivos ni elementos genéricos de AI
- Placeholders honestos: usar `—` en lugar de métricas inventadas
- Fotos: espacio reservado con etiqueta, nunca placeholder gris genérico

## Personalización
El design system `bakery-bethlehem` (cuando exista en `design-systems/`) tiene prioridad
sobre cualquier otro sistema para proyectos de la bakery.
