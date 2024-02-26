# qué es la lógica de programación

La lógica de programación es un conjunto de técnicas y herramientas que se utilizan para diseñar y crear algoritmos que resuelvan problemas computacionales. Su objetivo principal es desarrollar la capacidad de diseñar soluciones de manera estructurada y sistemática, lo que a su vez permite desarrollar programas eficientes, fáciles de mantener y escalables.

Otro concepto fundamental es que esta es un conjunto de reglas y principios que se usan para desarrollar algoritmos, es decir, secuencias de instrucciones que permiten resolver un problema o realizar una tarea específica en un programa informático. La lógica de programación es esencial para los desarrolladores de software, ya que les permite generar soluciones informáticas eficientes y efectivas.

## Importancia

La lógica de programación se basa en la aplicación de la razón y el pensamiento lógico para analizar un problema y diseñar una solución algorítmica. Esto implica comprender la estructura de los datos y las instrucciones, así como la capacidad de ejecutar operaciones matemáticas, comparaciones y operaciones lógicas para crear algoritmos que resuelvan el problema en cuestión.

La importancia de esta radica en su capacidad para ayudar al desarrollador a crear programas informáticos que sean eficientes, fáciles de entender y mantener, además le permite organizar y estructurar sus ideas, definir los procesos necesarios para alcanzar un objetivo, y crear algoritmos eficientes y escalables. también ayuda a evitar errores comunes como bucles infinitos, condiciones mal definidas y otros problemas que pueden afectar negativamente el funcionamiento del programa. Un buen diseño de algoritmos puede mejorar el rendimiento del programa, reducir los errores y hacer que el código sea más fácil de entender y modificar. Además, la lógica de programación también puede ayudar a los desarrolladores a detectar y corregir errores en el código existente.

si eres nuevo en la programación es necesario que inicies con este tema y aprendas de una manera sólida los conceptos básicos y tengas un buen pensamiento lógico y critico. En esta web vamos a desarrollar los ejercicios con peseint por lo que si estás interesado puedes continuar leyendo.

Para utilizar PseInt, que es una herramienta de aprendizaje de programación basada en pseudocódigo, primeramente, descarga e instala el programa desde su [sitio oficial](https://pseint.sourceforge.net/). Asegúrate de que tu sistema operativo sea compatible con PseInt. Luego de la descarga, abre el archivo de instalación y sigue las indicaciones del asistente para completar la instalación. Durante este proceso, tendrás la opción de personalizar algunas configuraciones de acuerdo a tus preferencias. Una vez finalizada la instalación, inicia PseInt y estarás listo para comenzar a desarrollar algoritmos en pseudocódigo.

## Variables y tipos de datos

Las variables y tipos de datos son conceptos fundamentales en programación ya que permiten almacenar y manipular información en un programa. En general, las variables se utilizan para almacenar valores que pueden cambiar durante la ejecución del programa, mientras que los tipos de datos determinan el tipo de información que se puede almacenar en una variable.

las variables se declaran utilizando la palabra reservada "definir", seguida del nombre de la variable y su tipo de datos. Por ejemplo, para declarar una variable llamada "edad" que almacena un número entero, se puede utilizar la siguiente línea de código:

`definir edad como entero`

Existen diferentes tipos de datos en PSeInt, incluyendo enteros, reales, caracteres, boleanos y cadenas de texto. Por ejemplo, para declarar una variable llamada "nombre" que almacena una cadena de texto, se puede utilizar la siguiente línea de código:

`definir edad como texto`

Una vez que se han declarado las variables, se pueden asignar valores a ellas utilizando el operador de asignación "=", como se muestra en el siguiente ejemplo:

```js
edad = 25;
nombre = "Juan";
```

Además de los tipos de datos básicos, los programas también pueden utilizar estructuras de datos más complejas, como arreglos y registros, para almacenar y manipular información de manera más organizada pero eso lo vamos a ver mas adelante.

Un ejemplo práctico de uso de variables y tipos de datos en PSeInt podría ser el siguiente programa que solicita al usuario su nombre y edad, y luego muestra un mensaje personalizado de bienvenida:

```js
Algoritmo EjemploVariables
definir nombre como texto
definir edad como entero
escribir "Ingrese su nombre: "
leer nombre
escribir "Ingrese su edad: "
leer edad
escribir "Bienvenido/a " + nombre + "!"
escribir "Tu edad es ", edad
FinAlgoritmo
```

En este ejemplo, se utilizan variables de tipo "texto" y "entero" para almacenar el nombre y la edad del usuario, respectivamente. Luego, se utilizan las operaciones de concatenación de texto y numero "+" y "," para crear un mensaje personalizado de bienvenida que incluye el nombre y la edad del usuario.

## Condicionales

Los condicionales permiten realizar acciones en función de una condición específica. En otras palabras, se puede decir que son instrucciones que permiten que el programa tome decisiones basadas en ciertas condiciones.

Un ejemplo de un condicional sería: si el valor de X es mayor que 5, entonces hacer algo; de lo contrario, hacer algo más. En PseInt, un ejemplo sería el uso de la estructura "Si...Entonces...Sino" para controlar el flujo de ejecución del programa. Ahora miremoslo en codigo.

```js
Algoritmo ejemplo_si_sino
	Definir numero Como Entero
	Escribir "Introduce un número:"
	Leer numero
	Si numero >= 0 Entonces
		Escribir "El número es positivo"
	Sino
		Escribir "El número es negativo"
	FinSi
FinAlgoritmo
```

En este caso, si el número introducido por el usuario es mayor o igual que cero, se mostrará el mensaje "El número es positivo", de lo contrario se mostrará "El número es negativo".

## bucles

los bucles al igual que las condiciones son importates porque permiten la repetición de un conjunto de instrucciones. En PSeInt, existen tres tipos de bucles: el bucle para (for), el bucle mientras (while) y el bucle repetir HASTA QUE (do while), que en la mayoria de los lenguajes de programación estos son los mas comunes. El bucle para se utiliza para repetir un conjunto de instrucciones un número determinado de veces. Se utiliza una variable de control que va incrementando su valor en cada iteración. Por ejemplo:

```js
Algoritmo ejemplo_bucle_para
	para i = 1 hasta 10 con paso 1 hacer
		escribir(i)
	finpara
FinAlgoritmo
```

Este código escribirá los números del 1 al 10.

El bucle mientras se utiliza cuando no se conoce el número de veces que se debe repetir un conjunto de instrucciones. La repetición continúa mientras se cumpla una determinada condición. Por ejemplo:

```js
Algoritmo ejemplo_bucle_mientras
	Definir x Como Entero
	x = 0
	mientras x < 10 hacer
		x = x + 1
	finmientras
	Escribir x
FinAlgoritmo
```

Este código incrementará el valor de x hasta que sea menor que 10 e imprimira el resultado.

El bucle repetir HASTA QUE es similar al bucle mientras, pero se ejecuta al menos una vez antes de comprobar la condición. Por ejemplo:

``` js
Algoritmo ejemplo_bucle_repetir_HASTA_QUE
	Definir opcion Como Entero
	repetir
		Escribir "Ingrese una opción:"
		leer opcion
		Escribir "Opción ingresada: ", opcion
	Hasta Que  opcion = 0
FinAlgoritmo
```

Este código seguirá pidiendo al usuario que ingrese una opción hasta que la opción ingresada sea 0.

## Arreglos

Los arreglos en programación son una estructura de datos que permite almacenar una cantidad fija de elementos del mismo tipo en una sola variable. Los arreglos son muy útiles cuando se necesita manejar grandes cantidades de datos.

En Pseint, los arreglos se declaran especificando su tipo de dato, nombre y tamaño. Para acceder a los elementos del arreglo, se utiliza un índice que indica la posición del elemento que se quiere acceder. Un ejemplo práctico de uso de arreglos en Pseint sería el almacenamiento de calificaciones de estudiantes en un examen. En este caso, se podría declarar un arreglo de tipo numérico con el tamaño correspondiente al número de estudiantes, y luego ir asignando las calificaciones correspondientes a cada posición del arreglo. Aqui te dejo un ejemplo diferente para que analizes.

``` js
Algoritmo ejemplo_arreglos
    Dimension arreglo[5] 
    Para i = 1 Hasta 5 Con Paso 1 Hacer
        arreglo[i] = i
		Escribir "El valor del elemento ", i, " es: ", arreglo[i]
    FinPara
FinAlgoritmo
```

En este ejemplo, se declara un arreglo llamado arreglo que contiene 5 elementos de tipo entero. Luego, se utiliza un bucle Para para asignar valores a cada uno de los elementos del arreglo, que van desde 1 hasta 5. Finalmente, se muestra en pantalla el valor de cada elemento del arreglo mediante el mismo bucle Para.

## funciones o sobprocesos

Las funciones o subprocesos permiten reutilizar código y hacer que los programas sean más modulares y fáciles de entender y mantener. En PSeInt, al igual que en otros lenguajes de programación, las funciones se definen mediante la palabra clave "Funcion" seguida del nombre de la función y los parámetros que recibe entre paréntesis.

A continuación se muestra un ejemplo de función en PSeInt que recibe dos números como parámetros y devuelve el resultado de la suma:

``` js
SubProceso Sumar <- hazSumar(num1 Por Referencia, num2 Por Referencia)
	Definir resultado como Entero
	Sumar = num1 + num2
FinSubProceso

Algoritmo ejemplo_funcion
	Definir var1, var2, resultado2 como Entero 
	var1 = 3 
	var2 = 5 
	resultado2 = hazSumar(var1,var2)
	Escribir "La suma de ", var1, " y ", var2, " es " resultado2
FinAlgoritmo
```

En este ejemplo, la función Sumar recibe dos parámetros de tipo Entero y devuelve otro valor de tipo Entero que es el resultado de sumar los dos números. Luego, en el programa principal se definen las variables como enteros y se les asignan los valores 3 y 5 respectivamente. Finalmente, se llama a la función Sumar pasando como parámetros los valores por referencia y se asigna el resultado a la variable resultado2.

Al ejecutar este programa se mostrará en pantalla el mensaje "La suma de 3 y 5 es 8", ya que la función Sumar devuelve el valor 8 al sumar 3 y 5.

Si estudiantes cada uno de los puntos propuestos y practicaste los ejercicios ya tienes los fundamentos necesarios para comenzar a programar y crear tus propios scripts, espero que esta información haya sido útil y si deseas comunicarte conmigo abajo te dejo mis redes sociales. Que tengas excelente día.