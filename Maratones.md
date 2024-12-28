# Carreras

## Listado de Entidades

### carreras **(ED)**

- carrera_id **(PK)**
- nombre 
- tipo_carrera **(FK)**
- distancia
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
- distancia

## paises **(EC)**

- pais_id **(PK)**
- nombre

## Relaciones

1. Una **carrera** _pertenece_ a un **tipo de carrera**. (_1 a 1_)
2. Una **carrera** se _corre_ en un **país**.           (_1 a 1_)

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


