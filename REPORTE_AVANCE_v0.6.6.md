# Reporte de avance — v0.6.6

Proyecto: Plataforma CZ5 ENOS 2026–2027  
Versión: v0.6.6 · Fortalecimiento legible por cantón  
Estado: Ajuste funcional sobre arquitectura existente.

## Cambios aplicados

- Se mantuvo la arquitectura base del módulo Riesgo Zonal.
- Se ajustó la ficha de Fortalecimiento para que priorice primero la lectura del plan legalizado por cantón.
- El bloque Kobo de sensibilización queda separado y muestra explícitamente “sin registros Kobo conectados para este cantón” hasta integrar la exportación real.
- Se ajustaron los KPI superiores cuando el enfoque activo es Fortalecimiento:
  - Prioridad de acompañamiento.
  - Líneas del plan.
  - Brechas CZ5.
  - Kobo sensibilización.
  - Estado del plan.
- Se mantiene la lógica de selección cantonal, provincial, mapa, F03, Respuesta y Análisis sin rediseño general.

## Motivo del ajuste

En v0.6.5 el bloque Kobo aparecía primero y como todos los campos estaban pendientes, parecía que la ficha no cambiaba por cantón. En v0.6.6 se muestra primero el bloque que sí cambia por cantón desde los planes legalizados, y Kobo queda como fuente complementaria pendiente de conexión.

## Pendiente

Conectar exportación real de Kobo Fortalecimiento/Sensibilización para que los campos de campañas, público objetivo, sectores, comités, canales y ejecución cambien con datos verificados por cantón.
