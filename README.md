# SNGR-CZ5-ENOS v0.7.7

Versión con acceso interno por credenciales F01 hash para Dashboard y Riesgo Zonal.

## Flujo

La plataforma abre sin login. Los módulos 1 a 4 permanecen libres. Dashboard y Riesgo Zonal solicitan correo + `_ID` F01 y aplican el alcance territorial del usuario.

## Nota

No publicar el Excel de credenciales en GitHub Pages. La base incluida no contiene correos ni `_ID` en texto plano.
