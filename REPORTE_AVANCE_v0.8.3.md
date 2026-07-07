# REPORTE DE AVANCE · SNGR CZ5 ENOS · v0.8.3

## Cambio principal
Se simplificó la barra cartográfica del módulo **Riesgo Zonal** para reducir sobrecarga visual y mejorar uso operativo por perfiles GAD, provincial y zonal.

## Ajustes implementados

1. Se reemplazó la barra densa de filtros por cinco controles principales:
   - Provincias
   - Cantones
   - Sitio crítico
   - Infraestructura
   - Elementos cartográficos

2. Se retiraron de la vista principal los filtros secundarios:
   - Todos
   - Respuesta
   - Acciones
   - Monitoreo
   - F03 puntos
   - F03 líneas
   - F03 polígonos

3. La distinción entre punto, línea y polígono queda integrada dentro de **Elementos cartográficos**, evitando que el usuario deba decidir por tipo geométrico.

4. Las opciones de mapa no esenciales se movieron a un bloque colapsable:
   - Ver toda CZ5
   - Continental
   - Galápagos
   - Abrir ArcGIS Online

5. Se actualizó la lógica de filtros para aceptar el nuevo filtro general `ELEMENTOS_CARTOGRAFICOS`.

6. Se corrigió la activación visual de botones para que el botón activo refleje la capa o filtro seleccionado.

## Criterio de diseño
La versión reduce densidad de botones y prioriza la lectura por intención del usuario:

- ¿Quiero ver división territorial? → Provincias / Cantones.
- ¿Quiero revisar puntos críticos? → Sitio crítico.
- ¿Quiero revisar infraestructura expuesta? → Infraestructura.
- ¿Quiero ver toda la cartografía F03? → Elementos cartográficos.

## Estado de seguridad
Se mantiene la arquitectura de v0.8.2:

- Formularios, Generar prompt, Chat institucional y Bibliografía permanecen abiertos.
- Dashboard y Riesgo Zonal requieren credenciales.
- El control aún es visual/local; la seguridad real requiere backend institucional.

## Validación técnica
Se revisó la sintaxis JavaScript del `index.html` posterior al ajuste.

## Recomendación siguiente
Para v0.8.4 se recomienda revisar el panel derecho de ficha cantonal y convertir la lectura en tarjetas de decisión:

- Estado actual
- Brecha prioritaria
- Acción inmediata
- Formulario que debe completar
- Prompt sugerido
