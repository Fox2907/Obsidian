
![[Excalidraw/Data Warehouse|Data Warehouse]]

# Modelos de datos
Los modelos de datos son representaciones abstractas y estructuradas de la información que se utiliza en un sistema de información, base de datos o aplicación. Estos modelos se utilizan para definir cómo se organizarán y almacenarán los datos, así como para proporcionar una comprensión común de la estructura de la información en un contexto determinado.
# Tipos de modelos de datos
### Modelo conceptual
Es el que esta orientado a decidir que datos son los interesantes y como se relacionan entre sí. Ejemplo: Modelo entidad-relación.
### Modelo lógico
Este modelo esta orientado a expresar las manipulaciones en forma abstracta para que sea viable realizar implementaciones sobre los varios tipos de manejadores disponibles. Ejemplo: Modelo Relacional y el modelo de datos NoSQL.
### Modelo Físico
Describe cómo se implementarán los datos en un sistema de almacenamiento específico. Puede incluir detalles como índices, particiones y métodos de acceso.

# Niveles en diseño de bases de datos


|            | Enfasis              | Modelo de Registros | Multidimensional                  |
|------------|----------------------|---------------------|-----------------------------------|
| Conceptual | Objetos y relaciones | Entidad-relación    |  -No hay estándares<br/>- CMDM    |
| Lógico     | Operaciones          | Relacional          | - MD específicos<br/>- Star-model |
| Físico     | Almacenamiento       | DBMSs               | Parámetros en servidores MD       |

# Enfoques del diseño conceptual
