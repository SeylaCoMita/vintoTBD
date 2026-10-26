# Bienvenido a la Documentación del Proyecto

Este proyecto forma parte de la materia **Taller de Programación**.

Documenta el **Sistema de Reportes de Incidentes Ambientales del municipio de Vinto**,
una aplicación web hecha con **NiceGUI** que permite a los vecinos registrar incidentes
ambientales (basura, quema, contaminación de agua, etc.), ubicarlos en un mapa
y adjuntar fotos como evidencia.

**Autora:** Seyla Esther Coimbra Mita
**Carrera:** Ingeniería de Sistemas, Universidad Adventista de Bolivia

## Características Principales

* Arquitectura modular y escalable (páginas, componentes, modelo y servicio).
* Mapa interactivo con **Leaflet** y **OpenStreetMap**.
* Persistencia con **SQLModel** sobre **SQLite**.
* Carga de fotos con `ui.upload`.
* Configuración externa mediante archivo `.env`.
* Documentación generada con **MkDocs** y el tema **Material**.

## Contenido

| Sección | Qué encontrarás |
| --- | --- |
| [Instalación y Requisitos](instalacion.md) | Cómo preparar el entorno y ejecutar el sistema |
| [Arquitectura del Sistema](arquitectura.md) | Capas, carpetas y flujo de datos |
| [Guía de Uso](guia-uso.md) | Cómo registrar y consultar reportes |
| [API / Módulos](api.md) | Descripción de módulos, modelo y servicio |
| [Diagramas de Clases](diagramas-clases.md) | Modelo de datos y relaciones |
| [Pruebas](pruebas.md) | Casos de prueba manuales |
| [Conclusiones](conclusiones.md) | Resultados y mejoras futuras |

!!! note "Nota"
    Los nombres de archivos y clases son los de la estructura modular del proyecto.
    Si tu carpeta tiene nombres distintos, ajusta las rutas en estas páginas.
