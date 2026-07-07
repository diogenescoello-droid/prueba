# REPORTE DE AVANCE · SNGR-CZ5-ENOS v0.8.4

## Cambio principal
Se incorpora un espacio compacto de **prompt cartográfico para informe** dentro del área cartográfica de Riesgo Zonal.

## Ajustes aplicados
- Se mantiene la barra cartográfica simplificada de v0.8.3: Provincias, Cantones, Sitio crítico, Infraestructura y Elementos cartográficos.
- Se agrega un único bloque operativo para escribir palabras clave y generar un prompt de informe técnico cartográfico.
- El prompt se arma con el contexto visible: territorio autorizado, filtro cartográfico activo, conteos de elementos, geometrías visibles, semáforo y elemento seleccionado cuando exista.
- El bloque utiliza un solo botón: **Generar prompt**.
- El texto generado se copia automáticamente al portapapeles cuando el navegador lo permite y queda visible en un recuadro para revisión.

## Criterio UX
No se agregaron botones adicionales al mapa. La función queda como un espacio de apoyo técnico dentro de la misma lectura cartográfica.

## Uso previsto
El usuario escribe palabras clave como inundación, puente, aislamiento, socavación, vía, recinto, evidencia F03 o infraestructura crítica. La plataforma produce una instrucción para ChatGPT orientada a elaborar informes técnicos cartográficos.

## Limitación
El prompt no sustituye la validación técnica. Se exige declarar datos preliminares, brechas de información y necesidad de verificación CZ5/GAD cuando corresponda.
