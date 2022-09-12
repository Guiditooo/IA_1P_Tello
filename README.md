# Parcial 1 de Inteligencia Artificial de 3er Año de Image Campus.

By: Guido Tello


CONSIGNA

El código del examen deberá estar alojado en un repositorio Git publico, de lo contrario no se corregirá.

Los repositorios serán clonados el día 28/09/2022 a las 23:59 (UTC - 3 hora estándar de Argentina) y se corregirá lo que se halla clonado.

En la actividad "Link al repositorio - Primer parcial" deberán poner el link al repositorio donde se aloja el código fuente del examen.


Mínimo de aprobación:

- Crear una simulación en la cual halla un Centro urbano y una cantidad N (modificable desde editor) de minas de oro que aparezcan en posiciones aleatorias del mapa.

- Los mineros deberán ir a recoger el oro, pasar un tiempo minando y luego regresar a depositarlo en el centro urbano.

- El mapa debe tener una grilla de nodos que le permita hacer a los mineros pathfinding.

- Los nodos deben de tener pesos diferentes entre sí, y algunos ser inutilizables.

- El minero decide cual es la mina más cercana utilizando un polígono de Thiessen (o diagrama de Voronoi) el cual tiene en cuenta los pesos de los nodos que tiene dentro para determinar las fronteras.

- Cuando una mina de oro se acaba, el polígono de Thiessen se recalcula.



Examen completo:

- En cualquier momento se puede dar un evento para que los mineros abandonan lo que están haciendo y vayan al centro urbano.

- En cualquier momento, si los mineros están dentro del centro urbano, se puede dar un evento para que continúen con su labor.

- Los mineros se mueven utilizando un algoritmo de Flocking.

- El peso de los nodos debe de poderse editar en tiempo de ejecución, lo cual dispara la re-calculacion de los polígonos de Thiessen y los paths calculados que se estén ejecutando.



Puntos extra:

- El movimiento de los mineros se hace en multi-threading.
