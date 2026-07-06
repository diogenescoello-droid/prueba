# SNGR-CZ5-ENOS v0.6.10

Versión de ajuste cartográfico del módulo Riesgo Zonal.

## Enfoque

La versión corrige la lectura del mapa cuando se trabaja con provincias, cantones y elementos F03. Los modos principales ahora son exclusivos para evitar capas superpuestas o filtros heredados que oculten información.

## Archivos principales

- `index.html`
- `data/riesgo_zonal_arquitectura_v0.6.10.json`
- `data/criterio_provincial_cartografia_v0.6.10.json`
- `assets/data/elementos_operativos_enos_v0.6.10.geojson`
- `REPORTE_AVANCE_v0.6.10.md`

## Nota

La capa F03 contiene 3 elementos demostrativos: punto, línea y polígono. Debe ser reemplazada por la exportación real de Kobo F03 o ArcGIS Online.
