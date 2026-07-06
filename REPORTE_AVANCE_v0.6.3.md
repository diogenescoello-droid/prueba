# Reporte de avance — v0.6.3

Proyecto: Plataforma CZ5 ENOS 2026–2027  
Módulo intervenido: Riesgo Zonal / Ficha cantonal / Respuesta  
Estado: En revisión técnica

## Objetivo

Ajustar la ficha cantonal para que, al seleccionar el enfoque **Respuesta**, los criterios mostrados correspondan a las necesidades reales del equipo de respuesta y no al bloque genérico de análisis.

## Cambios aplicados

1. Se conectó el enlace del formulario Kobo de Respuesta Operativa Cantonal:
   https://ee.kobotoolbox.org/x/gbTK3ocC

2. Se ajustó la prioridad lógica de la ficha:
   - Si el usuario está en **Respuesta**, la ficha muestra criterios de respuesta aunque el tema activo sea Brechas, Amenazas u otro tema secundario.
   - Si el usuario está en **Análisis**, la ficha muestra amenazas, exposición, vulnerabilidad y brechas técnicas.
   - Si el usuario está en **Fortalecimiento**, la ficha mantiene los criterios del formulario de sensibilización.
   - Si el usuario está en **Monitoreo**, la ficha muestra seguimiento, evidencias, alertas y validación.

3. En Respuesta se incorporaron tres bloques mínimos:
   - Directorio Plenaria COE Cantonal.
   - Brigada Cantonal EVIN.
   - Gestores de Alojamientos Temporales.

4. Se agregó botón **Abrir Kobo Respuesta** en la ficha cantonal del enfoque Respuesta.

5. Se agregó botón **Ver estructura Respuesta** con los campos requeridos para validar la información.

6. Los KPI superiores cambian de etiquetas cuando el enfoque activo es Respuesta:
   - COE cantonal.
   - Brigada EVIN.
   - Gestores AT.
   - Brechas operativas.
   - Kobo Respuesta.

## Archivos modificados

- `index.html`
- `data/riesgo_zonal_arquitectura_v0.6.3.json`
- `data/respuesta_operativa_schema_v0.6.3.json`

## Archivos no modificados

- Arquitectura general de la plataforma.
- Pestañas principales.
- Cartografía base cantonal/provincial.
- Lógica de Fortalecimiento ya incorporada.

## Observaciones técnicas

Los planes legalizados permiten precargar algunos datos de respuesta, especialmente menciones a COE, alojamientos, rutas, recursos o acciones; sin embargo, no garantizan que exista directorio actualizado, brigada EVIN conformada ni gestores de alojamientos designados. Por eso la fuente de validación para respuesta pasa a ser el Kobo específico.

## Pendiente

Conectar la exportación real de Kobo Respuesta para que la ficha cantonal deje de mostrar valores pendientes y muestre datos validados por cantón.
