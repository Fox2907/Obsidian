---
tags:
  - Hack4u
  - Linux
---

# One-liner
"One-liner" se refiere a un comando o una secuencia de comandos que se escribe en una sola línea de código y realiza una tarea completa o realiza una serie de tareas relacionadas. Estos comandos suelen ser concisos y se utilizan comúnmente en la línea de comandos de sistemas operativos basados en Unix, como Linux.

- **";":**  El punto y coma (`;`) se utiliza para separar múltiples comandos en una sola línea de entrada. Cuando se utiliza el punto y coma, los comandos se ejecutan de izquierda a derecha, independientemente de si el comando anterior fue ejecutado con éxito o no. En otras palabras, los comandos se ejecutarán secuencialmente, uno después del otro, sin importar el resultado del comando anterior.


![[Pasted image 20240117234348.png]]



![[Pasted image 20240117234441.png]]


![[Pasted image 20240117235044.png]]


- **"&&":** El operador `&&` en comandos de Linux se utiliza para ejecutar varios comandos en una sola línea y asegurarse de que el comando siguiente solo se ejecute si el comando anterior se ejecuta correctamente (es decir, si devuelve un código de salida 0). En otras palabras, el comando a la derecha de `&&` se ejecutará solo si el comando a la izquierda se ejecuta sin errores.

![[Pasted image 20240117234843.png]]


![[Pasted image 20240117235131.png]]


- **"||":** El operador `||` en comandos de Linux se utiliza para ejecutar el comando a la derecha solo si el comando a la izquierda falla, es decir, si el comando a la izquierda devuelve un código de salida diferente de cero. Este operador se utiliza para manejar el caso en el que deseas ejecutar un segundo comando solo si el primero falla.
  
  
![[Pasted image 20240117235627.png]]

# Stderr

Este canal estándar es la salida de error estándar, utilizado por los programas para mostrar mensajes de error o información de diagnóstico. Al igual que la salida estándar, normalmente se muestra en la pantalla, pero también puede redirigirse a un archivo separado.

Para que los errores no aparezcan en la terminal se puede aplicar la siguiente sintaxis de redireccion: 


![[Pasted image 20240118000144.png]]


# Stdout

Este canal estándar es la salida estándar, por donde un programa emite sus resultados o mensajes de éxito. La salida estándar se muestra generalmente en la pantalla (terminal), pero también puede redirigirse a un archivo.

Para evitar que la salida estándar aparezca en la terminal y, en su lugar, se redirija a un archivo, puedes utilizar la siguiente sintaxis de redirección:

![[Pasted image 20240118165925.png]]

Con esta sintaxis de comandos redirigimos la salida normal exitosa del comando:

![[Pasted image 20240118170639.png]]

Pero esta sintaxis no gestiona la salida de errores si estos existieran como se ve a continuación:

![[Pasted image 20240118170925.png]]

Para gestionar las salidas exitosas como erróneas se puede emplear la siguiente sintaxis:

- **Opción 1: **

![[Pasted image 20240118171124.png]]

- **Opción 2 (alternativa correcta): **

![[Pasted image 20240118171330.png]]


# Procesos

En el contexto de sistemas operativos, los procesos son programas en ejecución. Cada proceso tiene un identificador único, su propio espacio de memoria y recursos asignados. Los procesos pueden interactuar entre sí o pueden ser independientes.

- **Proceso Padre:** Cuando un programa se ejecuta, se inicia un proceso. Este proceso inicial se conoce como el "proceso padre". El proceso padre puede crear otros procesos, conocidos como "procesos hijos".
- **Proceso Hijo:** Un proceso hijo es un nuevo proceso creado por otro proceso, que actúa como su padre. El proceso hijo hereda ciertas características del proceso padre, como el entorno de ejecución y los recursos del sistema.

# Procesos en segundo plano

En un sistema operativo basado en Unix o Linux, un proceso en segundo plano es un proceso que se ejecuta sin interactuar directamente con el usuario a través de la terminal. Los procesos en segundo plano pueden ejecutarse simultáneamente con otros procesos y no bloquean la terminal, permitiendo que el usuario continúe interactuando con ella mientras el proceso está en ejecución.

La sintaxis siguiente nos permite que el comando o programa se ejecute en segundo plano sin bloquear la terminal, pero aun es dependiente del proceso padre (terminal), entonces si terminaramos el proceso padre, el proceso hijo tambien terminaria.

![[Pasted image 20240118170314.png]]

Para que el proceso hijo sea independiente del proceso padre podemos emplear el siguiente comando: 

![[Pasted image 20240118172125.png]]


# Recursos adicionales

-  Redirectores en Bash [Formato PDF]: [https://hack4u.io/wp-content/uploads/2022/05/bash-redirections-cheat-sheet.pdf](https://hack4u.io/wp-content/uploads/2022/05/bash-redirections-cheat-sheet.pdf)