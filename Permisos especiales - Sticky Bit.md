---
tags:
  - Hack4u
  - Linux
---
El *Sticky Bit* o bit adhesivo es uno de los permisos especiales de acceso utilizado en ficheros y directorios del entorno Unix y derivados como GNU/Linux. Su objetivo es que solo el usuario creador pueda eliminar o renombrar un archivo en sistemas donde todos los usuarios tienen permisos de lectura y escritura.

La configuración de este permiso de bit, sticky bit, pegajoso está a cargo del comando `chmod`, que tiene la función de gestionar y modificar los diferentes permisos de acceso del dispositivo. Por lo tanto, para la activación de este permiso deberás ejecutar alguno de los siguientes comandos:

```
chmod 1777 nombre_del_directorio
```

```
chmod +t nombre_del_directorio
```

En caso de querer desactivar el sticky bit, los comandos a emplear se escriben de la siguiente manera:

```
chmod 0777 nombre_del_directorio
```

```
chmod -t nombre_del_directorio
```

En el siguiente ejemplo, creamos un archivo llamado "test.txt", del cual el propietario es el usuario "fox". Sin embargo, al cambiar al usuario "fmluder", a pesar de que, con este usuario, con respecto al archivo pertenecemos al grupo "otros" y no tenemos los permisos de escritura, somos capaces de eliminar el archivo. Esto se debe a que los permisos del directorio al que pertenece el archivo para el grupo "otros" permiten la escritura, y son los permisos del directorio los que en este caso tienen mayor relevancia.


![[Pasted image 20240131234759.png]]

Para evitar este problema de permisos utilizaremos el *sticky bit* como se muestra a continuación:

![[Pasted image 20240131235119.png]]

La principal ventaja de la activación del *Sticky Bit* es su gran utilidad al momento de tener directorios compartidos entre varios usuarios, debido a que permite que solo el usuario creador de un archivo, el propietario del directorio o el usuario root pueda eliminarlo o renombrarlo, incluso si los demás usuarios tienen permisos de escritura para sticky bit Linux.


# Recursos adicionales

- ¿Qué es el Sticky Bit y cómo configurarlo?: [https://keepcoding.io/blog/que-es-el-sticky-bit-y-como-configurarlo/](https://keepcoding.io/blog/que-es-el-sticky-bit-y-como-configurarlo/)
- El bit Sticky | Tutorial de GNU/Linux: [https://www.fpgenred.es/GNU-Linux/el_bit_sticky.html](https://www.fpgenred.es/GNU-Linux/el_bit_sticky.html)