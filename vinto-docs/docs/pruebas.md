# Pruebas

Pruebas manuales realizadas sobre el sistema.

| N.º | Caso de prueba | Resultado esperado | Estado |
| --- | --- | --- | --- |
| 1 | Guardar un reporte con todos los campos | Se guarda y aparece en el mapa | Pendiente de marcar |
| 2 | Guardar sin título | Muestra mensaje de validación | Pendiente de marcar |
| 3 | Subir una foto válida | La foto se guarda en `uploads/` | Pendiente de marcar |
| 4 | Reiniciar la aplicación | Los reportes siguen disponibles (persistencia) | Pendiente de marcar |

!!! tip
    Cambia "Pendiente de marcar" por **Correcto** o **Falló** después de probar.

## Prueba de la documentación

```bash
mkdocs build --strict
```

Si termina sin errores, los enlaces y la navegación están bien.
