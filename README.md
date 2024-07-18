# Proyecto Final Cinema

## Descripción
Esta aplicación de cine, desarrollada en Python, utiliza SQLite3 para la base de datos y Tkinter para la interfaz gráfica. La aplicación ofrece dos modos de vista: uno para usuarios y otro para administradores. Los usuarios pueden ver películas, iniciar sesión, registrarse, y gestionar sus asientos, entre otras funcionalidades. Los administradores pueden gestionar películas, publicidad, productos, y salas con sus horarios, entre otras funcionalidades.

## Características

- **Vista del Usuario:**
  - Iniciar sesión y registrarse.
  - Ver la cartelera de películas.
  - Consultar su información.
  - Registrar asientos.

- **Vista del Administrador:**
  - Gestionar y editar películas.
  - Gestionar publicidad.
  - Gestionar productos.
  - Agregar películas y salas con sus horarios.

## Requisitos

- Python 3.x
- Tkinter (incluido en la biblioteca estándar de Python)
- SQLite3 (incluido en la biblioteca estándar de Python)
- Pillow
- ReportLab
- pdfkit => Ten en cuenta que para `pdfkit`, también necesitas instalar `wkhtmltopdf`.

  - Para Ubuntu/Linux:
    ```bash
    sudo apt update
    sudo apt install wkhtmltopdf
    ```

  - Para Windows:
    - Descarga el instalador desde [wkhtmltopdf](https://wkhtmltopdf.org/downloads.html) y sigue las instrucciones del asistente de instalación.


## Instalación de Paquetes

Para instalar las bibliotecas necesarias, usa los siguientes comandos:
- pip install Pillow
- pip install reportlab
- pip install pdfkit

## Estructura del Proyecto

```bash
proyecto_cine/
├── admin/
│   ├── __pycache__/
│   ├── admin_app.py
│   ├── constants.py
│   ├── db.py
│   ├── funciones.py
│   ├── gestor_productos.py
│   ├── info_usuario.py
│   ├── publicidad.py
│   ├── ui.py
│   └── utils.py
├── imagenes_comida/
├── imagenes_peliculas/
├── imagenes_publicidad/
├── cargar_cartelera.py
├── colores.py
├── configuracion.py
├── data_base.py
├── detalles_pelicula.py
├── eventos.py
├── imagenes.py
├── login.py
├── main.py
├── producto_comida.py
├── registrar_asientos.py
├── registro.py
├── tabla_productos.py
├── usuario_info.py
├── cartelera.db
├── tickets.json
└── usuarios.db
```

## Descripción de los Módulos

Este proyecto está compuesto por varios módulos con diferentes funciones. A continuación se detalla la estructura de los módulos y sus archivos asociados.

### `admin/`
Contiene módulos relacionados con las funciones administrativas.

- `admin_app.py`: Aplicación principal del administrador.
- `constants.py`: Constantes utilizadas en la aplicación.
- `db.py`: Funciones para manejar la base de datos.
- `funciones.py`: Funciones varias utilizadas en la administración.
- `gestor_productos.py`: Gestión de productos.
- `info_usuario.py`: Información del usuario registrado.
- `publicidad.py`: Gestión de publicidad.
- `ui.py`: Configuración de la interfaz de usuario del administrador.
- `utils.py`: Utilidades varias.

### Directorios de Imágenes
- `imagenes_comida/`
- `imagenes_peliculas/`
- `imagenes_publicidad/`
  
Estos directorios están destinados a almacenar imágenes correspondientes a comida, películas y publicidad, respectivamente.

### Archivos Principales

- `cargar_cartelera.py`: Carga de la cartelera de películas.
- `colores.py`: Definición de colores utilizados en la interfaz.
- `configuracion.py`: Configuración de la interfaz.
- `data_base.py`: Funciones para manejar la base de datos.
- `detalles_pelicula.py`: Mostrar detalles de las películas.
- `eventos.py`: Eventos y acciones en la interfaz.
- `imagenes.py`: Manejo de imágenes.
- `login.py`: Gestión de inicio de sesión y registro de usuarios.
- `main.py`: Punto de entrada de la aplicación.
- `producto_comida.py`: Gestión de productos de comida.
- `registrar_asientos.py`: Registro de asientos.
- `registro.py`: Gestión del registro de usuarios.
- `tabla_productos.py`: Tabla de productos.
- `usuario_info.py`: Información del usuario.
