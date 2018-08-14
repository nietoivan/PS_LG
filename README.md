
###########
EJERCICIO 1
###########

PASOS:
1. Se definen 3 funciones para calcular si la suma de los divisores de un número es Abundante, Defectivo o Perfecto.
2. Se solicita al usuario una serie de números enteros para procesar, los cuales no podrán ser ni números negativos ni decimales, ya que no se han realizado prueba de errores para estos casos (tampoco texto).
3. Se crea una lista de numeros enteros tipo range(1, valor) dónde valor será la mitad del número introducido por el usuario + 1. Con ello, se evitarán la mitad de operaciones ya que no existen números divisibles entre un número si su divisible es mayor que la mitad de dicho número. Es decir, para el valor de 10, tomaremos una lista de valores de [1, 2, 3, 4, 5] descartando los restantes [6, 7, 8, 9, 10] ya que núnca obtendremos un valor entero (excepto el número divisible por sí mismo, los cuales quedan excluídos).
4. Se procesan llamando a las funciones del punto 1 y se muestra por pantalla si es un número Abundante, Defectivo o Perfecto.


MEJORAS:
1. Desarrollar diferentes pruebas de errores para evitar la introducción de valores negativos, decimales y letras (no se ha implementado por falta de tiempo).
2. Crear una pequeña función que detecte automáticamente los números primos introducidos por el usuario y calificandolos directamente como "numeros defectivos/deficientes" sin necesidad de ser procesados.


###########
EJERCICIO 2
###########

Ha sido más dificultoso de realizar ya que no tengo conocimientos en Javascript, ni del uso de AJAX ni HighCharts. Se ha copiado de internet una integración de Hashmaps con Javascript para su utilización (260 líneas de código sin contabilizar con esta implementación de Hashmaps).

PASOS:

1. Pese a saber que la tecnología AJAX es con fines asíncronos, se ha utilizado AJAX de manera síncrona ya que el enunciado no indica cómo aplicarlo.
2. Se han utilizado llamadas ajax síncronamente unas dentro de otras (de manera secuencial) para realizar cada una de las peticiones JSON.
3. Se ha creado un HashMap general cuyos keys values almacenarán el nombre de la categoría (key) y un hashmap de los datos (fecha y valores) (values).
4. Se han normalizado y ordenado númericamente cada una de las fechas obtenidas, teniendo en cuenta cada uno de sus valores respectivamente (ordenación necesaria a la hora de representar en highCharts).
5. Se han creado nuevos arrays para entregar los datos adaptados a highCharts según la documentación obtenida en la web y con ello poder mostrar de manera automatizada cada una de las categorias, fechas y valores, independientemente del número de categorías que puedan existir.

MEJORAS: 
Utilizar promesas o callbacks para trabajar con ajax asíncronamente.

