# Modelado de datos

## Pasos a seguir 

1. Identificar las entidades del sistema.      => Definir como los titulos, Ejm: Carreras, Distancias, ...etc.
2. Identificar los atributos de las entidades. => Definir como los subtitulos, Ejm: Carreras: Id de carrera, nombre, ...etc.
3. Identificar las llaves primarias y foráneas.=> Relación, llave primaria y luego foraneas => PK, FK.
4. Asginar una nomenclatura adeacuada a las entidades y sus atributos.

        Las entidades, siempre en plural.
        Los atributos, siempre en singular.
        Siempre en minuscula, sin acento, y no espacio, sino "_" (Guion bajo).

5. Identificar las entidades pivote del sistema.
6. Identificar los catálagos del sistema.
7. Identificar los tipos de relaciones del sistema.
8. Crear el Modelo Entidad-Relación del sistema.

9. Crear el Modelo Relacional de la base de datos del sistema.
10. Identificar los tipos de datos de los atributos de las entidades del sistema.

        VARCHAR VS CHAR, uno es variable osea puede ir de 0-255, el otro siempre sera algo fijo y el resto 
                lo rellena de ceros.
        DATE, te interesa solo la fecha, DATETIME, te interesa fecha y hora, TIME, solo la hora.
        INT AUTO, lo hace incremental, 1,2,3,4,5.., solo se pone en la PK en la FK de otra tabla NO.
        Si tiene "foto" seria un archivo binario, pero no es ideal colocarlos asi pq a la hora de almacenarlo en la
                BBDD y luego consultarlo, exportarlo en la BBDD, va a demandar mucho rendimiento, mucho procesamiento
                de computo a la computadora donde este la BBDD, entonces si estamos almacenando archivos multimedia
                lo recomendable es subirlo a un servidor en alguna nuve, como google drive, dropbox, etc.. y copiar 
                la url y en la BBDD copiar la URL, por ello se pone VARCHAR(255) lo maximo si necesitas algo mas de 255 se usa el tipo de dato TEXT.
        FLOAT, tipo de dato con coma, OJO si no necesitaras operar con el tipo de dato, puedes usar VARCHAR.
        
        

11. Identificar los atributos que puedan ser únicos en el sistema.
12. Identificar las reglas de negocio (Operaciones CRUD) del sistema.

### Glosario

- **PK**: _Primary Key_
- **FK**: _Foreign Key_
- **UQ**: _Unique Attribute_


- **ED**: Entidad de datos
        Son entidades que contienen los datos principales del sistema. Representan las unidades fundamentales de información que se procesan y gestionan. 
        **Ejemplos:** Clientes, Productos, Ventas, Pedidos.

- **EP**: Entidad Pivote
        Actúan como intermediarios o conectores entre otras entidades. Su función principal es resolver relaciones de muchos a muchos (M:N) o agrupar datos relacionados. 
        **Ejemplos:** Detalles de Factura (conecta Facturas y Productos), Asignaciones de Roles (conecta Usuarios y Roles).

- **EC**: Entidad Catálogo
        Son tablas o entidades que contienen listas predefinidas de valores estáticos o semiestáticos. Sirven para estandarizar y facilitar la gestión de datos repetitivos.
        **Ejemplos:** Estados (Pendiente, Aprobado, Rechazado), Categorías de Productos, Tipos de Documentos.
