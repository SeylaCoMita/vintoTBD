# API / Módulos

## Modelo de datos

```python
from typing import Optional
from datetime import datetime
from sqlmodel import SQLModel, Field


class Reporte(SQLModel, table=True):
    id: Optional[int] = Field(default=None, primary_key=True)
    titulo: str
    descripcion: str
    tipo: str
    latitud: float
    longitud: float
    foto: Optional[str] = None
    fecha: datetime = Field(default_factory=datetime.now)
```

## Servicio

```python
from sqlmodel import Session, select


def crear_reporte(session: Session, reporte: Reporte) -> Reporte:
    session.add(reporte)
    session.commit()
    session.refresh(reporte)
    return reporte


def listar_reportes(session: Session) -> list[Reporte]:
    return session.exec(select(Reporte)).all()
```

## Resumen de módulos

| Módulo | Función |
| --- | --- |
| `models` | Define la tabla `Reporte` |
| `services` | `crear_reporte`, `listar_reportes`, guardado de fotos |
| `components` | Mapa Leaflet y formulario de reporte |
| `pages` | Página principal y rutas |

!!! note
    Los fragmentos son ilustrativos de la estructura; ajústalos a tu código real.
