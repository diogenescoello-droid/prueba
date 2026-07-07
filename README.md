# SNGR-CZ5-ENOS v0.7.3

Versión de Fase 2 con plataforma visible al ingresar y acceso restringido visualmente para Dashboard y Riesgo Zonal.

## Flujo de uso
La plataforma abre directamente en los módulos libres:

1. Formularios
2. Generar prompt
3. Chat institucional
4. Bibliografía

Al intentar abrir Dashboard o Riesgo Zonal, se solicita correo institucional y _ID F01 / contraseña.

## Nota de seguridad
Este control es visual y sirve para validación funcional. No debe usarse como seguridad real para datos sensibles. Para producción se requiere Apps Script, Firebase, Supabase o backend institucional.
