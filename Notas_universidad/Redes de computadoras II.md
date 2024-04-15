Rutas dinámicas
Protocolos de Re-encaminamiento/ Redireccionamiento: OSPF 
Topología o jerarquización de red (Conmutada o ruteado)
Gestión de redes

Capa 2 Enlace de datos : protocolo 802.11 (Wifi)

Capa 4 Transporte : puertos, UDP o TCP, 
Capa 5 Sesión : Conexión de extremo a extremo 

Ethernet: 802.3
Bluetooth: 802.15  

Modelo TCP/IP o modelo OSI

Laboratorio 4: Redireccionamiento dinámico
Técnica para disponer de manera continua de un servicio
Criterio: Calidad de servicio 
Parámetro: Alta disponibilidad
Métrica: Tiempo promedio de fallas/duración de fallas en el sistemas

Garantizar que el servicio funcione 24/7

Centro de Proceso de Datos (CPD)

Criterio ----> Varios métricas/parámetros
Métricas ----> Jerarquía de las IP, la mas importante

Una maquina con dos IP para conectarse a dos subredes diferentes, direccionamiento dinámico

Configuración sin equipos de respaldo, 

Investigar
Rangos para designar IP:  Equipos de comunicación, Servidores, Terminal de usuario (Subcategorías)
Default Gateway: Ruta por defecto, Internet?
ISP
Loopback
NAT (Network Address Translation), para servidores, evitar spoofing
NAT dinámico???
Spoofing
DHCP: asigna de forma dinámica las IP 
Diferencia entre Hub y Switch
Hub distribuye el canal para todos 
Switch da un ancho de banda para una cantidad de puertos


Analizador de trafico

Router: solo dos puertos Ethernet
Switch: Configurable
Objetivo
Instalar y configurar un enlace de alta disponibilidad empleando protocolos de redireccionamiento dinámico

Tres tipos de direccionamiento:
- Inicio: Configuración de IP, mascara, default gateway y métrica
- Enrutamiento estático: Next Hop, es vigente siempre
- Enrutamiento dinámico: Cambia en función del tráfico

Tres tipos de equipos: 
- Terminal de usuario
- Servidor
- Equipo de comunicación  

Equipos de comunicación del laboratorio
Software de simulación

Aplicación (Diagram de flujo)
Procedimiento a seguir para el redireccionamiento dinámico
Ruta alterna (alta disponibilidad)

Pregunta de examen
Por que seleccionaste el equipo de comunicación Cisco 2911
En su configuración básica permite utilizar 3 puertos GigabitEthernet
Serial modem

Switch para poder conectar una LAN
Router con Switch, necesario que todos salgan por el router
No es conexión broadcast
Red en triangulo: uso de tres puertos
Puertos --> jerarquías
Rutas directas (3)
Rutas alternas (3)

Condición de saturación

Proceso de restauración: Volver a las condiciones iniciales

Ambigüedad --> caída de red

catch server YT
Acelerador de tráfico 

Protocolos OSPF STP RIP 2
red en loopback???

Práctica Nro. 4 : Ruteado vs Conmutado
Min. 3000 palabras

Normas

Metro Ethernet (Mezcla de LAN y WAN)

Red telefónica (PSTN) y red de datos (ET) ---> Infraestructura hibrida
Tecnología convergente

Objetivo 
Estudiar/Investigar/Analizar las tecnologías PSTN y la red de datos y sus puntos de convergencia

Red de telefonía
Red conmutada ---> Asignación directa, Asigna un recurso de manera exclusiva a un cliente temporalmente (Asignación directa/Conmutación de circuitos-Switchado), garantizan el recurso, capacidad rígida.
El recurso obtenido persiste durante toda la conexión. 

Red de datos
Red ruteada ---> Conmutación de paquetes, Asignación compartida, capacidad flexible, degradación del servicio (Saturación), red dinámica 
Utiliza router, manejamos direcciones IP, 

UTP
Fiber channel

3 tipos de redes LAN
- Ethernet
- Fieldbus (Entornos industriales)
- 
Core, middle, Borde

Switching ---> Veloz en Punto a Punto
               ----> Lenta en broadcast
Core --> Switching
Borde --> Routing

Armar una topología con la configuración mas eficiente y explicarla

Quality of Service ---> Protocolo???

Libro de Cisco Interworking 2.0, CCNA

Que equipos son de conmutación y cuales son de enrutamiento

Practica 2 : Protocolos orientados a la conexión y conexionless


Criterio: Quality of services
Parámetro: Alta disponibilidad

Tiempo medio de caidas
Capa 4 TCP UDP 


Laboratorio 5: Quality of service 
Cuadrado ---> Dos Triángulos

Examen 
- Parte teórica 
- Parte práctica 

Laboratorio 5: Rutas alternas

Criterio: Balanceo y carga

CSMA/CD dirección de portadora/conexiones ---> Escucha el canal
Logical Link control

Wireless ---> cambia en MAC
LLC es transparente

OSPF 

Enlace disponible ---> Pero debe ser eficiente

Oracle ---> No aguanta timeouts, si existe timeout se corta
					Enlace de mejor calidad, se mide con tiempo de latencia

Data y Señalización

Mayor ancho de banda ---> Mas señalización, mas sincronización

Video IP ---> Cifrado, compresión, codificación
Load balanced ---> Dos canales y decidir por donde mandar
nivel de eficiencia

RIP de segunda jerarquía 

Método de selección ---> tiempo de latencia
Quality of service 

Armar rutas por nodos

Definir la jerarquía de rutas

6 rutas directas
9 rutas

RIP 
Funciones: 
- Ruta por defecto
- Ruta alterna
- En que casos cambiar

Capa 2: Resuelve la ruptura de enlace, detección de portadora, escucha el medio CSMA/CD, acceso al medio

Diagrama de rutas, jerarquía de rutas

Doble configuración: Genera ambigüedad en el router

Árbol de decisiones

Por fibra el enlace con más tráfico 
Loopback
