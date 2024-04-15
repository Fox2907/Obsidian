---
tags:
  - Hack4u
  - Linux
---
El control de atributos de archivos en Linux se puede realizar mediante los comandos `chattr` y `lsattr`. Estos comandos permiten establecer atributos especiales en archivos y directorios que pueden controlar ciertas características y comportamientos de los mismos. Aquí hay una descripción de cada comando:
# chattr (Change Attribute):
   
- `chattr` se utiliza para cambiar los atributos de un archivo o directorio en Linux.
- Algunos atributos comunes que se pueden establecer con `chattr` incluyen `+i` (inmutable), `+a` (solo para agregar), `+d` (no respaldable) y `+s` (archivo seguro).
- Para establecer un atributo, se utiliza `chattr +atributo nombre_del_archivo`.
- Para eliminar un atributo, se utiliza `chattr -atributo nombre_del_archivo`.
- Por ejemplo, para hacer que un archivo sea inmutable y no pueda ser eliminado, se puede usar `chattr +i archivo`.
# lsattr (List Attributes):
 
- `lsattr` se utiliza para mostrar los atributos de un archivo o directorio en Linux.
- Simplemente se ejecuta `lsattr nombre_del_archivo` y muestra una lista de los atributos establecidos en ese archivo o directorio.
- Por ejemplo, para ver los atributos de un archivo llamado "ejemplo.txt", se puede usar `lsattr ejemplo.txt`.

Estos comandos proporcionan un control adicional sobre los archivos y directorios en Linux, permitiendo a los usuarios establecer atributos especiales para controlar el acceso, la protección y el comportamiento de los archivos y directorios en el sistema de archivos.

En la siguiente imagen podemos ver el funcionamiento de ambos comandos `lsattr` y `chattr`: 

![[Pasted image 20240201232656.png]]

# Recursos adicionales

- Control de atributos de ficheros Linux: [Chattr y Lsattr](https://rm-rf.es/chattr-y-lsattr-visualizar-y-modificar-atributos-en-sistemas-de-ficheros-linux/#:~:text=El%20primer%20comando%2C%20lsattr%20permite,chmod%2C%20chown%2Csetfacl%E2%80%A6)
- Comandos Chattr y Lsattr en Linux: [https://programmerclick.com/article/5604675172/](https://programmerclick.com/article/5604675172/)