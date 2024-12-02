# Front-End-M3-AE3
Laboratorio Virtual 1

1. Manejo de Objetos JSON (2 puntos)
Implementa un objeto JSON que represente el listado de doctores en el hospital (nombre, especialidad, años de experiencia, disponibilidad).
1.1. Usa objetos anidados para organizar información adicional de cada doctor, como horarios disponibles y contacto.
Se implementó en el archivo equipo.js, en el objeto json: const doctores = [...
1.2. Utiliza destructuring para acceder a las propiedades de estos objetos y mostrar la información de un doctor específico en la consola y en la interfaz web.
Se implemento en el archivo equipo.js
Se despliega en la vista equipo.html

2. Operaciones con JSON (1.5 puntos)
Realiza las siguientes operaciones con los objetos JSON:
2.1. Clonación: Crea una copia de un objeto JSON y modifícalo sin afectar el original.
2.2. Merge: Fusiona dos objetos JSON. Por ejemplo, puedes fusionar la información de doctores con la lista de servicios médicos disponibles.
2.3. Recorrido y stringify: Recorre los objetos JSON para mostrar en el navegador la lista de doctores disponibles. Convierte el objeto a una cadena JSON usando JSON. stringify() y muestra el resultado en la consola.

Para esta actividad se tomo como referencia la libreria json.js del repositorio de adalid, la cual fue extendida y adaptada para este proposito.
Se crearon botones para asignar json hospital1 u hospital2 para probar el boton mostrar.
La variable currentJSON se declaró con let lo que permite reasignar su valor dentro del bloque.
La funcion merge une hospital1 y hospital2
Se ocupa la funcion recorrido y stringify para mostrar el resultado en la consola y en el cuerpo de la página.

3. Implementación de Estructuras de Datos (2 puntos)
Implementa estructuras de datos en el sitio web del hospital para gestionar mejor la información de los doctores:

Se tomo como referencia el repositorio de ayuda de adalid

3.1. Arreglos: Utiliza un arreglo para almacenar la lista de doctores. Implementa operaciones como agregar, eliminar y buscar doctores dentro del arreglo.
El arreglo comienza vacío
Se creó un boton para cargar el arreglo desde el JSON
El botón mostrar despliega en consola el arreglo
El botón agregar desde el prompt da error incluso dandole formato json (lo recibe como txt, no veo darle mas vueltas)
El botón agregar interno, agrega un elemento en el formato esperado y se puede visualizar en conjunto con el boton mostrar
El botón eliminar, quita el ultimo elemento del arreglo.

3.2. Pilas: Implementa una pila para gestionar las citas de los pacientes (última cita agendada, próxima cita a atender, etc.).
Se agregaron botones para simular la agenda de 3 (o más) pacientes, desapilar pacientes y mostrar estado de la pila.

3.3. Colas: Crea una cola para simular el orden de llegada de los pacientes en la página de contacto.
Se agregaron botones para simular la cola de atención de 3 (o más) pacientes, desapilar pacientes y mostrar estado de la pila.


4. Programación de Algoritmos (1.5 puntos)
4.1. Implementa un algoritmo de búsqueda que permita encontrar un doctor específico dentro del arreglo de doctores.
Se implentó una funcion para buscar un doctor desde un texto ingresado en el prompt. El resultado se despliega en la consola.

4.2. Implementa un algoritmo de ordenamiento para organizar la lista de doctores por años de experiencia.
Se implementó la función de ordenamiento Descendente y Ascendente a través de dos botones, el resultado se observa en la consola.
En cada ejecución se inicializa la lista de doctores y a continuación se muestra el log del resultado de ordenamiento.

4.3. Explica en el archivo README la complejidad de los algoritmos utilizados, aplicando conceptos de Big-O y complejidad ciclomática.
El algoritmo de búsqueda de 4.1 es O(n) porque se revisa secuencialmente cada elemento.
El algoritmo de ordenamiento de 4.2 es O(n log n) por se usa la función sort.