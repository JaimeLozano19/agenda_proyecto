# Proyecto Django: Agenda y Herramienta de Tareas

Este proyecto Django consta de dos aplicaciones principales: una para gestionar una agenda de contactos y otra para la gestión de tareas. A continuación, se describen los modelos y las funcionalidades de cada una:

## Agenda de Contactos

La aplicación de la agenda permite realizar las siguientes operaciones sobre los contactos:

- **Agregar Contacto:**
  - `name` (Nombre): Campo obligatorio, hasta 30 caracteres.
  - `last_name` (Apellido): Campo opcional, hasta 30 caracteres.
  - `phone` (Teléfono): Campo opcional, hasta 12 caracteres.
  - `mobile` (Móvil): Campo obligatorio, hasta 12 caracteres.
  - `email` (Correo Electrónico): Campo obligatorio.
  - `compañia` (Compañía): Campo opcional, hasta 20 caracteres.
  - `date` (Fecha): Campo de fecha con valor predeterminado de la fecha actual.
  - `notes` (Notas): Campo de texto opcional.

- **Ver Contactos:**
  - Lista todos los contactos existentes.

- **Editar Contacto:**
  - Permite actualizar la información de un contacto existente.

- **Eliminar Contacto:**
  - Elimina un contacto de la agenda.

## Herramienta de Tareas

La aplicación de la herramienta de tareas permite gestionar tareas con los siguientes campos:

- **Agregar Tarea:**
  - `title` (Título): Campo obligatorio, hasta 100 caracteres.
  - `description` (Descripción): Campo de texto opcional.
  - `date` (Fecha de Creación): Campo de fecha con valor predeterminado de la fecha actual.
  - `estimated_end` (Fecha de Vencimiento Estimada): Campo de fecha opcional.
  - `priority` (Prioridad): Campo numérico opcional con valor predeterminado de 3.

- **Ver Tareas:**
  - Lista todas las tareas existentes.

- **Editar Tarea:**
  - Permite actualizar la información de una tarea existente.

- **Eliminar Tarea:**
  - Elimina una tarea de la herramienta.

## Configuración del Proyecto

Para ejecutar este proyecto en tu entorno local, sigue estos pasos:

1. Clona el repositorio: `git clone https://github.com/JaimeLozano19/django-agenda-proyectos`
2. Instala las dependencias: `pip install -r requirements.txt`
3. Aplica las migraciones: `python manage.py migrate`
4. Inicia el servidor de desarrollo: `python manage.py runserver`

Ahora podrás acceder a la aplicación de agenda en ` http://localhost:8000/` y a la herramienta de tareas en `http://localhost:8000/tareas/`.

¡Disfruta de tu aplicación Django de Agenda y Herramienta de Tareas!
