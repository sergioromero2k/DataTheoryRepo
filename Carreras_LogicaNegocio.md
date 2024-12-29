# Carreras

## Listado de Entidades

### carreras **(ED)**

- carrera_id **(PK)**
- nombre 
- tipo_carrera **(FK)**
- fecha
- tiempo
- mejor_tiempo
- altitud
- lugar
- pais **(FK)**
- foto

### tipos_carreras **(EC)**

- tipo_carrera_id **(PK)**
- descripcion
- distancia       **(UQ)**

## paises **(EC)**

- pais_id **(PK)**
- nombre  

## Relaciones

1. Una **carrera** _pertenece_ a un **tipo de carrera**. (_1 a 1_)
2. Una **carrera** se _corre_ en un **país**.           (_1 a 1_)

## Diagramas

### Modelo Entidad - Relación

![Modelo Entidad -Relación](./CarrerasModeloEntidadRelacion.jpg)

### Modelo Relacional de la BD 

![Modelo Relacional](./CarrerasModeloRelacionalBD.jpg)

## Reglas de Negocio

### carreras

1.  Crear el registro de una carrera.
2.  Leer el registro de una(s) carrera(s) dada un condición en particular.
3.  Leer todos los registros de la entidad carreras.
4.  Actualizar los datos de una carrera dada una condición en particular.
5.  Eliminar los datos de una carrera dada una condición en particular.

### tipos_carreras

1.  Crear el registro de un tipo de carrera.
2.  Leer el registro de uno(s) tipo(s) de carrera(s) dada un condición en particular.
3.  Leer todos los registros de la entidad tipos carreras.
4.  Actualizar los datos de un tipo de carrera dada una condición en particular.
5.  Eliminar los datos de una tipo de carrera dada una condición en particular.

### paises

1.  Crear el registro de un país.
2.  Leer el registro de un(os) pais(es) dada un condición en particular.
3.  Leer todos los registros de la entidad paises.
4.  Actualizar los datos de un(os) paises dada una condición en particular.
5.  Eliminar los datos de un país dada una condición en particular.


## Si funciona perfe
<!-- 
Falta paso 4. Asginar una nomenclatura adeacuada a las entidades y sus atributos.

# Carreras

## Listado de Entidades

### Carreras

- Id de Carrera **(PK)**
- Nombre 
- Tipo de Carrera **(FK)**
- Distancia
- Fecha
- Tiempo
- Mejor Tiempo
- Altitud
- Lugar
- País **(FK)**
- Foto

### Tipo de Carrera

- Id de tipo de carrera **(PK)**
- Descripción
- Distancia

## Paises

- Id de País **(PK)**
- Nombre -->


