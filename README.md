PARTE 01 : Resolver los siguientes casos usando íntegramente PHP
---

### Problema 01

Usando PHP, crear una clase llamada **ChangeString** que tenga un método llamado build
el cual tome un parámetro string que debe ser modificado por el siguiente algoritmo.

Reemplazar cada letra de la cadena con la letra siguiente en el alfabeto. 
Por ejemplo reemplazar ```a``` por ```b``` ó ```c``` por ```d```.

Finalmente devolver la cadena.

**Indicaciones**

- Crear la solución en un solo archivo llamado ChangeString.php
- El método build devuelve la salida del algoritmo
- Considerar el siguiente abecedario : a, b, c, d, e, f, g, h, i, j, k, l, m, n, ñ, o, p, q, r,s, t, u, v, w, x, y, z.

**Ejemplos**
- entrada: ```123 abcd*3``` - salida: ```123 bcde* 3```
- entrada: ```**Casa 52``` - salida: ```**Dbtb 52```
- entrada: ```**Casa 52Z``` - salida: ```**Dbtb 52A```

### Problema 02

Usando PHP, crear una clase llamada **CompleteRange** que tenga un método
llamado build el cual tome un parámetro de colección de números enteros
positivos (1,2,3, ...n). El algoritmo debe completar si faltan números en la
colección en el rango dado. Finalmente devolver la colección completa.

**Indicaciones**

- Crear la solución en un solo archivo llamado CompleteRange.php
- El método build devuelve la salida del algoritmo
- Considerar el parámetro de colecciones con números enteros positivos ordenados de manera ascendente. Ejemplo [4, 6, 7 ,10]

**Ejemplos**
- entrada: ```[1, 2, 4, 5]``` - salida: ```[1, 2, 3, 4, 5]```
- entrada: ```[2, 4, 9]``` - salida: ```[2, 3, 4, 5, 6, 7, 8, 9]```
- entrada: ```[55, 58, 60]``` - salida: ```[55, 56, 57, 58, 59, 60]```

### Problema 03

Usando PHP, crear una clase llamada **ClearPar** que tenga un método llamado
build que reciba como parámetro una cadena formada sólo por paréntesis. 
El algoritmo debe eliminar todos los paréntesis que no tienen
pareja. Finalmente devolver la nueva cadena.

**Indicaciones**

- Crear la solución en un solo archivo llamado ClearPar.php
- El método build devuelve la salida del algoritmo
- Considerar solamente cadenas formadas de paréntesis

**Ejemplos**

- entrada: ```()())()``` - salida: ```()()()```
- entrada: ```()(()``` - salida: ```()()```
- entrada: ```)(``` - salida: ``` ``` *(una cadena vacía)*
- entrada: ```((()``` - salida: ```()```


### Problema 04

Usando PHP, crear una clase llamada **Fibonacci** que tenga un método llamado
build que reciba como parametro un entero. 
Dentro de esta clase debes crear una funcion recursiva para calcular la serie de fibonacci hasta la posicion N comenzando desde 0
Esta funcion sera llamada por el metodo build con el parametro ingresado.
El termino maximo a calcular sera el 12

**Indicaciones**

- Crear la solución en un solo archivo llamado Fibonacci.php
- El método build devuelve la salida del algoritmo
- Considerar solamente numeros enteros
- Considerar que el maximo numero de terminos es 12 si es mayor lanzar una excepcion "El numero es muy grande"
- Considerar que el menor termino es 0 con resultado 0

**Ejemplos**
- entrada: 5 - salida: 5
- entrada: 6 - salida: 8
- entrada: 7 - salida: 13




### Problema 05

Usando PHP, crear una clase llamada **Matriz** que tenga un método llamado
build que reciba como parametro un entero. 
Dentro de este metodo deberas crear un algoritmo que te imprima una matriz de NxN tomando como caracter por cada punto el numero que ingresaste 
Hasta un maximo de 8 x 8 y un minimo de 3 x 3

**Indicaciones**

- Crear la solución en un solo archivo llamado Matriz.php
- El método build imprime en consola la matriz resultante
- Considerar solamente numeros enteros
- Considerar que el maximo numero 8 y minimo 3, de lo contrario lanzar una excepcion "El numero es muy grande o muy pequeño"

**Ejemplos**
- entrada: 3
- salida:

3   3   3

3   3   3

3   3   3

- entrada: 4
- salida:

4  4  4  4

4  4  4  4

4  4  4  4

4  4  4  4



PARTE 02 : Crear una pagina web
---

Utilizando la siguiente api como referencia https://random-data-api.com/api/v2/users?size=100
Dicho api te regresa una lista de usuarios e informacion de ellos

Realiza una pagina que te enliste el resultado del api que anteriormente se mostraba
La pantalla donde muestra la informacion debe cumplir con lo siguiente
  - Una tabla donde se muetra la informacion:
    - Nombre
    - Apellido
    - Correo
    - *Acciones*
  - La tabla debe contener una columna que se llame "Acciones" donde cada fila debe tener dos botones


    -  Ver mas: Este boton te debe de abrir un dialogo u otra pantalla donde muestra mas detalle del usuario
      - Avatar
      - Nombre
      - Apellido
      - Correo
      - Usuario
      - Numero de telefono


    -  Editar: Este boton te abrira un dialogo u otra pantalla para poder editar la informacion del usuario con un boton de guardar: Todos los campos son requeridos validar que todos los campos son validos
      - Nombre
      - Apellido
      - Correo
      - Usuario
      - Numero de telefono


    -  Eliminar: Este boton te debe mostrar un dialogo de confirmación para eliminar el usuario

Las acciones eliminar te debe mostrar en consola el id del usuario a eliminar
Las acciones Editar al pulsar el boton guardar debe de validarte los campos y si son validos poner en consola los campos a guardar
