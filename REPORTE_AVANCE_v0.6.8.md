# Reporte de avance — v0.6.8

Proyecto: Plataforma CZ5 ENOS 2026-2027  
Versión: v0.6.8  
Tipo de cambio: ajuste funcional controlado  
Módulo: Riesgo Zonal · Análisis de Riesgo

## Cambios aplicados

- Se conectó el Kobo de **Asesoría Técnica de Análisis de Riesgo Cantonal** en el enfoque Análisis.
- URL integrada: `https://ee.kobotoolbox.org/x/u3ZnAY3b`.
- Se agregó botón **Abrir Kobo Análisis de Riesgo** dentro de la ficha cantonal de Análisis.
- Se agregó el botón en la estructura requerida de Análisis/F03.
- Se mantiene el botón **Abrir Kobo F03** para cartografía de puntos, líneas y polígonos.
- Se mantuvieron los ajustes de Fortalecimiento, Respuesta y Monitoreo.
- No se modificó la arquitectura base de navegación.

## Estado de datos

La plataforma queda lista para registrar asesorías técnicas del equipo de Análisis por cantón. Todavía falta conectar la exportación real de Kobo para que las respuestas registradas actualicen automáticamente los campos de la ficha cantonal.

## Archivos relevantes

- `index.html`
- `data/analisis_asesoria_kobo_schema_v0.6.8.json`
- `docs/DICCIONARIO_ANALISIS_ASESORIA_KOBO_v0.6.8.md`

## Pendiente

- Conectar exportación Kobo del formulario de Análisis.
- Cruzar registros por provincia/cantón.
- Reflejar acciones de mejora y brechas técnicas en la ficha cantonal.
