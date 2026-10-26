# Diagramas de Clases

## Modelo de datos

```mermaid
classDiagram
    class Reporte {
        +int id
        +str titulo
        +str descripcion
        +str tipo
        +float latitud
        +float longitud
        +str foto
        +datetime fecha
    }
    class ReporteService {
        +crear_reporte(session, reporte)
        +listar_reportes(session)
        +guardar_foto(archivo)
    }
    ReporteService ..> Reporte : usa
```

## Relaciones

* `ReporteService` depende de `Reporte` para crear y consultar registros.
* Las páginas y componentes dependen del servicio, no del modelo directamente.
