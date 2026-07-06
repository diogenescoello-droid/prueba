# REPORTE DE AVANCE · v0.6.9

Proyecto: Plataforma CZ5 ENOS 2026-2027
Versión: v0.6.9
Tipo de cambio: Cartografía F03 / elementos operativos / semáforo provincial preliminar

## Resultado de conteo cartográfico actual

Elementos cartográficos registrados actualmente en la plataforma: **3**.

- Puntos / geopoint: **1**
- Líneas / geotrace: **1**
- Polígonos / geoshape: **1**
- Provincia: **Guayas**
- Cantón: **Salitre**
- Fuente actual: **Kobo F03 demo técnico no oficial**

## Cambios aplicados

1. Se refuerza la capa de elementos cartográficos F03.
2. Los elementos se proyectan en el mapa como punto, línea y polígono.
3. Cada elemento muestra una burbuja de datos al pasar el cursor.
4. Cada elemento mantiene ficha técnica al seleccionarlo.
5. Se agrega semáforo provincial preliminar de validación cartográfica.
6. Se crea archivo de criterio provincial para semaforización cartográfica.

## Advertencia técnica

El semáforo provincial incorporado en esta versión es de **validación cartográfica preliminar**, no diagnóstico oficial de riesgo físico. Los elementos actuales son demostrativos y deben ser reemplazados por exportación real Kobo F03, ArcGIS Online o CSV/GeoJSON validado.

## Archivos principales

- index.html
- data/riesgo_zonal_arquitectura_v0.6.9.json
- data/criterio_provincial_cartografia_v0.6.9.json
- assets/data/elementos_operativos_enos_v0.6.9.geojson
