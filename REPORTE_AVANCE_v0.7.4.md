# REPORTE DE AVANCE — v0.7.4

Proyecto: SNGR CZ5 ENOS 2026-2027  
Versión: v0.7.4  
Cambio: Acceso protegido Dashboard/Riesgo Zonal con base F01 importada

## Cambios realizados

- Se incorporó la base F01 cargada por la Coordinación Zonal.
- El acceso a Dashboard y Riesgo Zonal valida correo institucional + `_ID` F01.
- Se aceptan múltiples `_ID` para correos con varios registros F01.
- Se guardan hashes SHA-256 de correo e `_ID`, no los valores planos.
- Al ingresar como GAD cantonal, Riesgo Zonal aplica automáticamente el cantón autorizado cuando existe código cantonal reconocido.
- Al ingresar como perfil provincial, Riesgo Zonal aplica la provincia autorizada.
- Se mantiene libre el acceso a Formularios, Generar prompt, Chat institucional y Bibliografía.

## Resultados del procesamiento F01

- Usuarios únicos con correo: 51.
- GAD cantonal: 42.
- Alcance provincial/delegado: 6.
- Administrador CZ5: 1.
- Equipo Análisis CZ5: 1.
- Consulta restringida/parroquial: 1.

## Limitación crítica

La protección sigue siendo estática si se publica en GitHub Pages. Los hashes reducen exposición directa, pero no sustituyen autenticación real. Para producción se requiere Apps Script, Firebase, Supabase o backend institucional.

## Estado

Listo para prueba interna de flujo F01 con correo + `_ID`. No usar como control definitivo de información sensible.
