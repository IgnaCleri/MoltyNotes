# Requerimientos de MoltyNotes 🦎📝

Este documento detalla lo que debe tener la aplicación de notas para ser considerada completa.

## 1. Requerimientos Básicos (MVP)

- **Crear Nota:**
  - El usuario debe poder ingresar un título.
  - El usuario debe poder ingresar el contenido de la nota.
  - La nota debe guardarse en un archivo físico (recomendado: carpeta `notes/` con extensión `.txt` o `.md`).
  
- **Listar Notas:**
  - Mostrar una lista numerada de todos los títulos de las notas guardadas.
  
- **Leer Nota:**
  - El usuario elige una nota de la lista (por número o nombre).
  - La app muestra el contenido completo en la terminal.
  
- **Borrar Nota:**
  - El usuario puede seleccionar una nota para eliminarla permanentemente.

## 2. Características Avanzadas (Próximos Pasos)

- **Búsqueda por Palabras Clave:**
  - Implementar una función que busque un término dentro de todos los archivos de notas y devuelva cuáles lo contienen.
  
- **Categorización por Carpetas (Tags):**
  - Permitir guardar notas en subcarpetas (ej: `trabajo/`, `personal/`) para mantener el orden.
  
- **Cifrado de Seguridad:**
  - Al iniciar la app, pedir una contraseña. Si es incorrecta, las notas se guardan/leen de forma cifrada (ilegible para otros).
  
- **Auto-Backup en GitHub:**
  - Cada vez que se cierra la aplicación o se guarda una nota, realizar un `commit` y `push` automático a este repositorio.

## 3. Guía de Implementación sugerida

1. Crear la estructura de carpetas (ej: `main.py` y carpeta `notes/`).
2. Implementar un menú principal en un bucle `while`.
3. Crear funciones separadas para cada acción (`crear_nota`, `leer_nota`, etc.).
4. Usar la librería estándar `os` para manipular archivos y directorios.
