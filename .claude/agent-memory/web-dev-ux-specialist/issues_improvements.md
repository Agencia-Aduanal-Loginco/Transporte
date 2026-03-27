---
name: Problemas y mejoras Loginco
description: Bugs JS identificados, brechas de UX y mejoras de conversión priorizadas por impacto vs esfuerzo
type: project
---

**Bugs funcionales confirmados (código roto):**
1. Menú hamburguesa mobile — botón sin ID/JS, no abre/cierra menú móvil
2. FAQ accordion — chevrons decorativos, sin JS para expandir/colapsar
3. Botones Hero — son `<button>` sin href ni acción real
4. Formulario — sin validación JS ni backend (conocido/aceptado)

**Gaps de UX/conversión identificados:**
- Sin botón flotante de WhatsApp (canal preferido B2B México)
- Sin CTA sticky al hacer scroll (nav CTA solo visible al top)
- FAQ no colapsa — muestra toda la respuesta siempre, pierde efecto de "descubrir"
- Footer links de "Soluciones" apuntan a href="#" (no anclan a secciones)
- focus-ring del formulario usa `focus:ring-indigo-400` en lugar de la clase accent del proyecto
- La segunda ubicación mencionada en FAQ (Zihuatanejo) no aparece en el mapa ni en ninguna sección

**Mejoras priorizadas (impacto alto / esfuerzo bajo):**
1. JS menú hamburguesa — crítico para mobile, 5 líneas
2. JS FAQ accordion — mejora percepción de interactividad profesional
3. Botones Hero con href correcto (#bodega, #contacto)
4. WhatsApp float button — mayor impacto en conversión B2B México
5. Footer links — corregir href a anclas reales
6. Formulario: focus ring en color accent, no indigo genérico
