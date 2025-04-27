#Sistema de Gestión de Torneos de eSports

## Autor
Aruzhan Dosmagambetova
aruzhanym

## Desarrollo de un sistema de gestión de torneos de eSports, aplicando Programación Orientada a Objetos (POO) y utilizando diagramas
UML para modelar su estructura y funcionalidad.
git@github.com:aruzhanym/torneo-esports-uml.git

##Diagramas UML
###Diagrama de Casos de Uso
![Diagrama de casos de uso](diagrams/casos-uso.png)

### Diagrama de Clases
![Diagrama de clases](diagrams/clases.png)

## Estructura del Proyecto
torneo-esports-uml/ ├── src/
├── diagrams/
│ ├── casos-uso.png
│ ├── clases.png
├── README.md
├── .gitignore


## Justificación del diseño
Clases de Entidad (Equipo, Jugador, Torneo): Representan el modelo de datos puro. 
Así separo la lógica de negocio (atributos y operaciones básicas) de cualquier otra capa 
lo que permite cambiar facilmente la estructura interna sin afectar el resto del sistema.

Clases de Control (GestorEquipos, GestorTorneos): Encapsulan las reglas de negocio y orquestan 
las operaciones entre entidades. De este modo evito que la lógica de gestión esté dispersa 
centralizando las interacciones (por ejemplo inscribir un equipo en un torneo o generar emparejamientos).

Clases de Interfaz (VistaConsola): Manejan la presentación y la interacción con el usuario. 
Al mantenerla aislada puedo cambiar la forma de entrada/salida 
(por ejemplo, pasar de consola a interfaz gráfica) sin tocar la logica de negocio ni la estructura de datos.

## Conclusiones
En este proyecto he aprendido a definir actores y casos de uso
a diseñar diagramas UML de uso y de clases y a organizar el sistema en capas de Entidad, Control e Interfaz, al tiempo que he comprendido la importancia
de documentar todo de forma clara en el README.md
