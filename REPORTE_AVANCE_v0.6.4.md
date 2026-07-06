# Reporte de avance — Versión v0.6.4

Proyecto: Plataforma CZ5 ENOS 2026-2027  
Versión: v0.6.4  
Tipo de cambio: C — módulo/funcionalidad sin alterar arquitectura base  
Estado: En revisión

## Objetivo

Ajustar el enfoque de **Análisis** dentro del botón **Riesgo Zonal** para que la ficha cantonal muestre criterios técnicos diferenciados de Respuesta y Fortalecimiento, e incorporar el soporte explícito para la cartografía F03: puntos, líneas y polígonos.

También se actualizó el **Dashboard** para mostrar el avance del entramado de datos de riesgo zonal y el estado de conexión F03.

## Cambios realizados

1. Se creó la versión visible **v0.6.4 · Análisis técnico + Cartografía F03**.
2. La ficha cantonal, al seleccionar el enfoque **Análisis**, ahora despliega:
   - Riesgo preliminar.
   - Confianza del dato.
   - Lectura técnica resumida.
   - Amenazas principales.
   - Sectores o sitios críticos.
   - Elementos expuestos.
   - Vulnerabilidad/exposición.
   - Brechas técnicas de análisis.
   - Calidad de extracción documental.
   - Condición técnica.
   - Acción sugerida CZ5.
   - Fuente principal.
3. Se incorporó el bloque **Cartografía F03 · puntos, líneas y polígonos** dentro de Análisis.
4. Se habilitaron filtros de elementos:
   - F03 puntos.
   - F03 líneas.
   - F03 polígonos.
5. Se agregó botón **Abrir Kobo F03** usando el enlace del formulario F03 existente.
6. Se agregó estructura requerida para **Análisis/F03**.
7. Se actualizó el Dashboard con un panel de integración de riesgo zonal, base PDF y F03.

## Archivos modificados

- `index.html`
- `data/riesgo_zonal_arquitectura_v0.6.4.json`
- `assets/data/elementos_operativos_enos_v0.6.4.geojson`
- `data/analisis_tecnico_schema_v0.6.4.json`
- `data/cartografia_f03_schema_v0.6.4.json`
- `docs/DICCIONARIO_ANALISIS_TECNICO_v0.6.4.md`
- `docs/DICCIONARIO_CARTOGRAFIA_F03_v0.6.4.md`

## Advertencia técnica

La capa `elementos_operativos_enos_v0.6.4.geojson` contiene tres geometrías demostrativas para validar visualización F03: un punto, una línea y un polígono. No son datos oficiales ni deben interpretarse como sitios críticos reales. Deben reemplazarse con la exportación real de Kobo F03 o ArcGIS Online.

## Pendientes

1. Conectar exportación real de Kobo F03.
2. Convertir `geopoint`, `geotrace` y `geoshape` a GeoJSON válido.
3. Validar coordenadas, duplicados, precisión y coherencia de geometrías.
4. Integrar evidencias y responsable del registro.
5. Recalcular KPI de Análisis con datos reales.

## Decisión solicitada

Validar si la estructura de Análisis y F03 responde a lo que necesita el departamento antes de conectar datos reales.
