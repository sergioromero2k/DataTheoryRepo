## Listado de Entidades

### carreras 

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

### tipos_carreras

- tipo_carrera **(PK)**
- descripcion 
- distancia

### paises

- pais **(PK)**
- nombre

### Relaciones

1.  Una **carrera** __pertenece__ a un **tipo de carrera* (_1 a 1_).
2.  Una **carrera** se __corre__ en un **país** (_1 a 1_).