# SNGR-CZ5-ENOS v0.7.2

Versión de transición para control de acceso al área de Análisis de Riesgos.

## Cambios principales

- Acceso simplificado con **correo institucional + _ID F01**.
- Opción visual para **cambiar contraseña**. En esta versión se guarda solo en el navegador para validar el flujo; en producción debe hacerse en backend.
- La sesión abre y prioriza el módulo **Riesgo zonal / Análisis de Riesgos**.
- La autorización sigue siendo visual en GitHub Pages; no protege datos sensibles.

## Producción

Para uso real, mover validación de usuario, _ID y contraseña a Apps Script, Firebase, Supabase o backend institucional.
