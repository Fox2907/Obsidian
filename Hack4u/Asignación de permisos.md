---
tags:
  - Hack4u
  - Linux
---
Para asignar permisos, se utiliza el comando `chmod` seguido de la notación simbólica o octal y el nombre del archivo o directorio.
También es posible cambiar el grupo al que pertenece un archivo con el comando `chgrp`. 

1. Con el comando `chmod` + las letras `u, g, o` + `+` o `-` + `r, w, x` se pueden añadir o quitar permisos al propietario, grupo u otros.

![[Excalidraw/chmod_1]]

![[Pasted image 20240124233922.png]]


2.  Con el comando `chgrp` + `<nombre del grupo>` + `<directorio>`, cambiamos el grupo al que pertenece el directorio.

![[Pasted image 20240124233506.png]]



3. Creación de un usuario con directorio y bash, con el comando `useradd`. Además se le puede asignar una contraseña.


![[Pasted image 20240124235735.png]]

<hr>

![[Pasted image 20240125001055.png]]

<hr>

![[Pasted image 20240125000146.png]]

<hr>

![[Pasted image 20240125001347.png]]


4. Cambiar el propietario y el propietario y el grupo con el comando `chown`.

![[Pasted image 20240125001943.png]]


5. Creación de grupos con el comando `groupadd`.

![[Pasted image 20240125002711.png]]


6. Añadir un usuario a un grupo.

```
sudo usermod -a -G sudo <nombre_de_usuario>
```


El comando `usermod` en Linux se utiliza para modificar las propiedades de un usuario. En este caso específico, `usermod -a -G sudo` se utiliza para agregar un usuario a un grupo en particular, y en este contexto, al grupo `sudo`. Aquí está el significado de las opciones utilizadas:

- `-a`: Esta opción indica que se va a añadir al usuario a un grupo en lugar de reemplazar sus grupos actuales.
- `-G sudo`: Esta opción especifica el grupo al que se añadirá el usuario. En este caso, el grupo `sudo` es un grupo especial que generalmente tiene permisos para ejecutar comandos con privilegios de administrador mediante el comando `sudo`.


![[Pasted image 20240125003643.png]]


![[Pasted image 20240125004313.png]]


7. Eliminar usuarios de un grupo con el comando `gpasswd`.

```
sudo gpasswd -d nombre_de_usuario nombre_del_grupo
```


![[Pasted image 20240125004707.png]]


8. Eliminar un grupo con el comando `groupdel`.

```
sudo groupdel nombre_del_grupo
```


![[Pasted image 20240125004913.png]]
# Recursos adicionales

- Asignación de permisos: [https://www.ionos.es/digitalguide/servidores/know-how/asignacion-de-permisos-de-acceso-con-chmod/](https://www.ionos.es/digitalguide/servidores/know-how/asignacion-de-permisos-de-acceso-con-chmod/)
- Propietarios y permisos: [https://atareao.es/tutorial/terminal/propietarios-y-permisos/](https://atareao.es/tutorial/terminal/propietarios-y-permisos/)
- Gestión de usuarios, grupos y permisos en Linux: [https://computernewage.com/2016/05/22/gestionar-usuarios-y-permisos-en-linux/](https://computernewage.com/2016/05/22/gestionar-usuarios-y-permisos-en-linux/)
- Gestión de usuarios y grupos en Linux: [https://atareao.es/como/gestion-de-usuarios-y-grupos-en-linux/](https://atareao.es/como/gestion-de-usuarios-y-grupos-en-linux/)