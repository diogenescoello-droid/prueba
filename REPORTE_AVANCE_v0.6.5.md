# Reporte de avance — v0.6.5

Proyecto: Plataforma CZ5 ENOS 2026–2027  
Módulo: Riesgo Zonal  
Versión: v0.6.5 · Fortalecimiento dinámico por cantón

## Cambio aplicado

Se ajustó la ficha cantonal del enfoque **Fortalecimiento** para que los datos cambien al seleccionar cada cantón.

Antes, el bloque de Fortalecimiento mostraba principalmente la estructura del Kobo de sensibilización, pero como todavía no existe una exportación Kobo conectada por cantón, los campos se veían iguales: Pendiente / estructura esperada.

Ahora la ficha se divide en dos fuentes:

1. **Kobo Fortalecimiento / Sensibilización**: mantiene los campos del formulario usado por el equipo de Fortalecimiento.
2. **Plan legalizado / ficha PDF**: muestra líneas de fortalecimiento, brechas de acompañamiento CZ5, acciones del plan, monitoreo requerido, estado documental, condición técnica y prioridad de acompañamiento por cantón.

## Resultado funcional

Al seleccionar un cantón y activar **Fortalecimiento**, la ficha ya debe variar por cantón aun cuando el Kobo esté pendiente de conexión.

La plataforma distingue:

- Datos pendientes de Kobo.
- Datos preliminares extraídos de planes legalizados.
- Acción sugerida para acompañamiento CZ5.
- Prioridad de fortalecimiento por cantón.

## Archivos modificados

- `index.html`
- `data/riesgo_zonal_arquitectura_v0.6.5.json`
- `data/fortalecimiento_cantonal_schema_v0.6.5.json`

## Observación técnica

Los datos de Fortalecimiento provenientes de planes legalizados son preliminares y deben validarse con el equipo del área. Cuando se conecte la exportación real de Kobo, el bloque de sensibilización pasará de Pendiente a datos levantados por cantón.

## Estado

Ajuste funcional listo para revisión.
