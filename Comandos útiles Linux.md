1. Cerrar sesión mediante terminal.
	```
	pkill -KILL -u nombredeusuario
	```

2. Apagar computadora.

	- Apaga la computadora inmediatamente.

		```
		shutdown -h now
		```

	- Apaga la computadora dentro de `n` minutos.
	
		```
		shutdown -h +n
		```

3. Reiniciar computadora.

	- Reinicia la computadora inmediatamente.
		```
		shutdown -r now
		```

	- Reinicia la computadora dentro de `n` minutos.

		```
		shutdown -r +n
		```