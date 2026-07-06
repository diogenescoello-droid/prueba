# Reporte de avance — v0.6.10

Proyecto: Plataforma CZ5 ENOS 2026–2027  
Módulo: Riesgo Zonal · Cartografía F03  
Estado: Ajuste funcional y visual

## Cambios aplicados

1. Se ajustó el comportamiento de los botones cartográficos principales: **Provincias**, **Cantones** y **Elementos F03** ahora funcionan como modos exclusivos. Al activar Cantones o Elementos, la capa provincial se apaga automáticamente.

2. Se incorporó semaforización provincial cartográfica. En modo Provincias, cada provincia se pinta según el estado de sus elementos F03 registrados:
   - Rojo: existe al menos un elemento rojo.
   - Amarillo: existe al menos un elemento amarillo y no hay rojos.
   - Verde: existen elementos verdes y no hay amarillos/rojos.
   - Pendiente: no existen elementos F03 registrados o no tienen semáforo.

3. Las tarjetas provinciales alrededor del mapa ahora muestran datos cartográficos básicos:
   - Cantones por provincia.
   - Total de elementos F03 registrados.
   - Conteo de puntos, líneas y polígonos.
   - Conteo por semáforo provincial.

4. Se mejoró la visualización de puntos, líneas y polígonos F03:
   - Puntos más grandes y con borde contrastado.
   - Líneas más gruesas.
   - Polígonos con mayor opacidad.
   - Burbuja al pasar el cursor y ficha técnica al seleccionar el elemento.

5. Al activar Elementos F03 desde la barra principal, se limpia la selección provincial/cantonal previa para evitar que el mapa quede vacío por filtros territoriales heredados.

## Conteo actual de elementos cartográficos F03

La base actual contiene 3 elementos demostrativos:

- 1 punto / geopoint.
- 1 línea / geotrace.
- 1 polígono / geoshape.

Los 3 elementos pertenecen a Guayas · Salitre y tienen semáforo provincial preliminar **AMARILLO** por estar pendientes de validación técnica.

## Observación crítica

Estos elementos siguen siendo de prueba técnica. No constituyen cartografía oficial ni diagnóstico de riesgo físico. La estructura queda lista para reemplazar la capa demo por la exportación real de Kobo F03 o por capas oficiales de ArcGIS Online.
