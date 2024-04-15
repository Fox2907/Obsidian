Los permisos especiales SUID (Set User ID) y SGID (Set Group ID) son atributos especiales que se pueden establecer en archivos ejecutables en sistemas Unix y Linux. Estos atributos permiten que los programas se ejecuten con los privilegios del propietario del archivo o del grupo asociado, en lugar de con los privilegios del usuario que los ejecuta.

# SUID (Set User ID)

   - Cuando se establece el bit SUID en un archivo ejecutable, el programa se ejecuta con los privilegios del propietario del archivo.
   - Esto es útil en situaciones donde un programa necesita acceder a recursos que solo están disponibles para el propietario, pero no para el usuario que lo ejecuta.
# SGID (Set Group ID)

   - Cuando se establece el bit SGID en un archivo ejecutable, el programa se ejecuta con los privilegios del grupo asociado al archivo.
   - Esto es útil en situaciones donde un programa necesita acceder a recursos que solo están disponibles para un grupo específico, pero no para el grupo del usuario que lo ejecuta.

Es importante tener en cuenta que el uso de SUID y SGID puede representar un riesgo de seguridad si se aplica incorrectamente, ya que un programa con estos atributos puede ser objeto de abuso si no está diseñado y configurado correctamente. Por lo tanto, su uso debe ser limitado y cuidadosamente considerado para evitar posibles vulnerabilidades de seguridad.

A continuación, podemos ver el funcionamiento de ambos tipos de permisos `SUID` y `SGID`:

- En primer lugar podemos ver como se asignan los permisos de `SUID` y `SGID`
![[Pasted image 20240201235427.png]]

- Para encontrar archivos que tengan permiso `SUID` podemos utilizar el siguiente comando:
![[Pasted image 20240201235750.png]]

- Los archivos ejecutables con permisos SUID y SGID que pertenecen al usuario root pueden representar un riesgo de seguridad, ya que al ejecutarlos, el programa se ejecuta con los privilegios del propietario del archivo (ya sea el usuario root o el grupo root). Esto significa que un usuario normal puede ejecutar estos programas y obtener temporalmente privilegios de root, lo que podría ser utilizado para inyectar comandos y escalar privilegios de root:

![[Pasted image 20240202000614.png]]

Por lo tanto, es importante tener cuidado al establecer permisos SUID y SGID en archivos ejecutables, ya que pueden ser utilizados maliciosamente para obtener acceso no autorizado a recursos del sistema. Se recomienda limitar su uso y garantizar que solo se apliquen a programas que realmente requieran privilegios elevados y que estén diseñados de manera segura para mitigar cualquier riesgo potencial de seguridad.


# Recursos adicionales

- Permisos SGID, SUID y Sticky Bit: [Permisos SGID, SUID y Sticky Bit](https://deephacking.tech/permisos-sgid-suid-y-sticky-bit-linux/#:~:text=Permiso%20SGID,-El%20permiso%20SGID&text=Si%20se%20establece%20en%20un,perteneciente%2C%20el%20grupo%20del%20directorio.)
- Permisos especiales en Linux: [Permisos especiales en Linux – Sticky Bit, SUID y SGID](https://www.ochobitshacenunbyte.com/2019/06/17/permisos-especiales-en-linux-sticky-bit-suid-y-sgid/)
- Los bits SUID, SGID y Sticky: [Los bits SUID, SGID y Sticky](https://www.ibiblio.org/pub/linux/docs/LuCaS/Manuales-LuCAS/SEGUNIX/unixsec-2.1-html/node56.html)