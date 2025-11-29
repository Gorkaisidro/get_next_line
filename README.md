# get_next_line

Este proyecto consiste en la implementación de la función personalizada get_next_line en C, como parte del plan de estudios de la Escuela 42. Su objetivo es permitir la lectura de un archivo línea a línea, gestionando memoria de forma eficiente y comprendiendo en profundidad el uso de buffers, variables estáticas y la función `read()`.

---

## Tabla de Contenidos

- [Objetivo](#objetivo)
- [Funcionamiento](#funcionamiento)
- [Compilación](#compilación)

---

## 🎯 Objetivo

Implementar una función capaz de leer texto desde un file descriptor una línea completa por llamada, devolviendo dicha línea con su salto de línea final (si existe), y manejando correctamente el estado entre llamadas sucesivas gracias al uso de una variable estática.

---

## 📌 Funcionamiento


- Cada llamada a `get_next_line(fd)` devuelve **la siguiente línea** del archivo.
- Si no hay más contenido que leer o ocurre un error, devuelve **`NULL`**.
- La línea devuelta incluye el salto de línea `\n` si existe en el archivo.
- Debe funcionar leyendo desde un archivo y desde **stdin**.
- Utiliza un buffer cuyo tamaño se define mediante el flag:

  ```bash
  -D BUFFER_SIZE=<valor>

---

  ## ⚙️ Compilación

Para compilar el proyecto, simplemente ejecuta:

```bash
make
