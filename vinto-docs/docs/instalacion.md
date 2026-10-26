# Instalación y Requisitos

## Requisitos previos

* Python **3.8 o superior** (se recomienda 3.10+ para NiceGUI).
* `pip` actualizado.
* Un editor de código (VS Code o PyCharm).

## Instalación

```bash
# Crear el entorno virtual
python -m venv venv

# Activar (Windows)
venv\Scripts\activate

# Activar (macOS / Linux)
source venv/bin/activate

# Instalar dependencias del sistema
pip install nicegui sqlmodel python-dotenv
```

## Configuración con `.env`

Crea un archivo `.env` en la raíz del proyecto:

```ini
DATABASE_URL=sqlite:///reportes.db
UPLOAD_DIR=uploads
APP_PORT=8080
```

!!! warning "Seguridad"
    No subas el archivo `.env` a GitHub. Agrégalo a `.gitignore`.

## Ejecución

```bash
python main.py
```

Abre `http://localhost:8080` en el navegador.
