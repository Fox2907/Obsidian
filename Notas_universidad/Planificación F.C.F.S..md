First Come First Served
El primero en llegar es el primero en ser servido, se gestiona con una cola F.I.F.O. Cuando un proceso entra a la cola de preparados su BCP se coloca al final de la cola. Cuando la CPU queda libre, se asigna al proceso que esté al principio de la cola.
Ejemplo:

| Procesos | Tiempo de ejecución  | Tiempo de llegada |
|----------|----------------------|-------------------|
| A        | 5                    | 5                 |
| B        | 3                    | 8                 |
| C        | 4                    | 11                |
| D        | 8                    | 11                |
| E        | 1                    | 15                |
| F        | 3                    | 17                |

![[F.C.F.S]]


| Procesos | Tiempo de ejecución  | Tiempo de llegada | Tiempo de espera |
|----------|----------------------|-------------------|------------------|
| A        | 5                    | 5                 | 5 - 5 = 0        |
| B        | 3                    | 8                 | 10 - 8 = 2       |
| C        | 4                    | 11                | 13 - 11 = 2      |
| D        | 8                    | 11                | 17 - 11 = 6      |
| E        | 1                    | 15                | 25 - 15 = 10     |
| F        | 3                    | 17                | 26 - 17 = 9      |

TME = Total/#Procesos = 29/6 = 4.8 u.t.

