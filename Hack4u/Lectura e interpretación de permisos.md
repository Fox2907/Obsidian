---
tags:
  - Hack4u
  - Linux
---
  
En sistemas operativos basados en Unix y Linux, los permisos de archivos son un mecanismo fundamental para controlar el acceso a los archivos y directorios. Cada archivo o directorio tiene asociados tres conjuntos de permisos: uno para el propietario, otro para el grupo y otro para otros usuarios. Estos permisos definen quién puede realizar acciones específicas, como leer, escribir o ejecutar un archivo.

![[Tipos de usuario en Linux]]

Los permisos de archivos se representan mediante una notación octal o simbólica. La notación simbólica es más común y se presenta en el siguiente formato:

- **r (read):** Permite leer el contenido del archivo o listar el contenido del directorio.
- **w (write):** Permite modificar el contenido del archivo o crear, renombrar o eliminar archivos en un directorio.
- **x (execute):** Permite ejecutar el archivo como un programa o atravesar (navegar) un directorio.

![[Tipos de permisos]]


La estructura típica de la notación simbólica es `rwx`, donde cada letra indica la presencia (si está presente) o ausencia (si está ausente) del permiso correspondiente. Estos conjuntos de permisos se aplican al propietario, al grupo y a otros usuarios.

Ejemplo de notación simbólica:

- `rwxrw-r--`: El propietario tiene permisos de lectura, escritura y ejecución; el grupo tiene permisos de lectura y escritura; otros usuarios solo tienen permiso de lectura.

![[Notación permisos]]

Para poder ver los detalles de permisos de un archivo se puede utilizas el comando `ls -l`.


![[Pasted image 20240119231333.png]]




# Recursos adicionales

- Permisos y derechos en Linux: [https://blog.desdelinux.net/permisos-y-derechos-en-linux/?msclkid=22f8cb88ba8111ecb5d8a3db91f066ab](https://blog.desdelinux.net/permisos-y-derechos-en-linux/?msclkid=22f8cb88ba8111ecb5d8a3db91f066ab)
- Permisos básicos en Linux: [https://www.profesionalreview.com/2017/01/28/permisos-basicos-linux-ubuntu-chmod/](https://www.profesionalreview.com/2017/01/28/permisos-basicos-linux-ubuntu-chmod/)
- Permisos en Linux | Cómo son y cómo se cambian: [https://www.softzone.es/programas/linux/permisos-archivos-directorios-linux/](https://www.softzone.es/programas/linux/permisos-archivos-directorios-linux/)
- Cambiar permisos con comandos: [https://www.hostinger.es/tutoriales/cambiar-permisos-y-propietarios-linux-linea-de-comandos/](https://www.hostinger.es/tutoriales/cambiar-permisos-y-propietarios-linux-linea-de-comandos/)