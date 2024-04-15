---
tags:
  - Hack4u
  - Linux
---
Un descriptor de archivos es un número entero que actúa como un identificador para un archivo o una conexión de entrada/salida (E/S). Estos descriptores de archivos son utilizados por el kernel del sistema operativo para realizar operaciones de lectura, escritura y manipulación de archivos.

Hay tres descriptores de archivos estándar que están abiertos automáticamente para cada proceso:

- **0 (stdin):** Descriptor de entrada estándar. Por defecto, se asocia con la entrada estándar (por lo general, el teclado).
- **1 (stdout):** Descriptor de salida estándar. Por defecto, se asocia con la salida estándar (por lo general, la pantalla).
- **2 (stderr):** Descriptor de error estándar. Por defecto, se asocia con la salida de error estándar (por lo general, la pantalla).

Ejemplos: 

Creación de un archivo con descriptor de archivo y escritura dentro del archivo utilizando el descriptor de archivo. El símbolo "<" es para permitir lectura y ">" es para permitir la escritura.
![[Pasted image 20240118222654.png]]

![[Pasted image 20240118222848.png]]

Cerrar el descriptor de archivo:

![[Pasted image 20240118223339.png]]

Copia del descriptor de archivos y funcionamiento: 

![[Pasted image 20240118223756.png]]

Se puede también crear una copia del descriptor original y cerrarlo en el mismo comando (Esto en la shell zsh no se realiza correctamente, en bash sí): 

![[Pasted image 20240118230157.png]]



# Recursos adicionales

-  Redirectores en Bash [Formato PDF]: [https://hack4u.io/wp-content/uploads/2022/05/bash-redirections-cheat-sheet.pdf](https://hack4u.io/wp-content/uploads/2022/05/bash-redirections-cheat-sheet.pdf)