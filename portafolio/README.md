# 📌 Portafolio Web Personal

Este proyecto es una aplicación web que esta siendo desarrollada con Django que me permitira gestionar mi portafolio personal. Incluye funcionalidades de blog, contacto, autenticación de usuarios y gestión de proyectos.
El objetivo final es poder desplegarlo una vez ya haya finalizado los ajustes finales del front y back

## 🛠️ Tecnologías Utilizadas  

- **Python 3.10+**  
- **Django 5.1.5**  
- **Bootstrap 5** (para la interfaz)  
- **MySQL** (como base de datos)  
- **HTML, CSS y JavaScript**  

---

## 🚀 Instalación  

### 1 Crear y activar un entorno virtual  

```bash
python -m venv env
source env/bin/activate  # Linux/Mac
env\Scripts\activate     # Windows
```

### 2 Instalar dependencias  

```bash
pip install -r requirements.txt
```

### 3 Configurar la base de datos  

1. **Crear una base de datos PostgreSQL** y actualizar `settings.py`:  

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'nombre_base_datos',
        'USER': 'usuario',
        'PASSWORD': 'contraseña',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

2.**Ejecutar las migraciones**:

```bash
  python manage.py migrate
```

### 4 Crear un superusuario

```bash
python manage.py createsuperuser
```

Sigue las instrucciones para establecer un nombre de usuario y contraseña.

### 5 Ejecutar el servidor

```bash
python manage.py runserver
```

Accede en tu navegador a: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## 📌 Funcionalidades

### 🔹 **Autenticación de Usuarios**

- Registro, inicio y cierre de sesión.  
- Panel de usuario con acceso restringido.  

### 🔹 **Gestión de Proyectos**

- Crear, editar y eliminar proyectos.  
- Solo accesible para usuarios autenticados.  

### 🔹 **Blog**

- Publicar y administrar artículos.  
- Vista de lista y detalle de publicaciones.  

### 🔹 **Contacto**

- Formulario de contacto con validaciones.  
- Envío de mensajes vía email.  

### 🔹 **Páginas de Error Personalizadas**

- Manejo de errores 404 y 500 con páginas personalizadas.  

---

## 📝 Estructura del Proyecto

``` bash
  portafolioPersonal/
  ├── accounts/         # Gestión de usuarios  
  ├── blog/            # Módulo de blog  
  ├── contacto/        # Formulario de contacto  
  ├── error/           # Páginas de error personalizadas  
  ├── home/            # Página principal  
  ├── proyectos/       # Gestión de proyectos  
  ├── static/          # Archivos estáticos (CSS, JS, imágenes)  
  ├── templates/       # Plantillas HTML  
  └── portafolio/      # Configuración principal de Django
  ```

---

## 🎯 Uso del Proyecto  

- **Acceder a la Página Principal:**  
  - `http://127.0.0.1:8000/`  
- **Blog:**  
  - `http://127.0.0.1:8000/blog/`  
- **Proyectos (requiere login):**  
  - `http://127.0.0.1:8000/proyectos/`  
- **Contacto:**  
  - `http://127.0.0.1:8000/contacto/`  
- **Administración Django:**  
  - `http://127.0.0.1:8000/admin/`  

---

## ✅ Recomendaciones

- **Usar un entorno virtual** para evitar conflictos de dependencias.  
- **Mantener la configuración de la base de datos segura** y no compartir credenciales.  
- **Probar cada funcionalidad** antes de usar en producción.  

---

## 📌 Autor

``` bash
  Proyecto desarrollado por Fernando De La Barra

```
