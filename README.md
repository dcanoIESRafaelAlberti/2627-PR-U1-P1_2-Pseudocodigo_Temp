# 2627-PR-U1-P1_2-Pseudocodigo

En esta práctica desarrollarás cinco algoritmos para trabajar la entrada y salida de datos, las condiciones y los bucles.

Utiliza las primitivas estudiadas en [Unidad 1.1.1 — El pseudocódigo](https://revilofe.github.io/section1/u01/teoria/PROG-U1.1.1-Pseudocodigo/).

## Instrucciones

- Escribe cada algoritmo en un archivo independiente: `ejercicio1.txt`, `ejercicio2.txt`, …, `ejercicio5.txt`.
- Incluye `Inicio` y `Fin` para delimitar cada algoritmo.
- Utiliza nombres de variables descriptivos y sangría para distinguir los bloques.
- Muestra mensajes claros para solicitar datos y presentar resultados.
- Emplea las siguientes primitivas según las necesites:

| Elemento | Para qué sirve | Ejemplo |
|---|---|---|
| `Inicio` y `Fin` | Marcar el principio y el final del algoritmo. | `Inicio ... Fin` |
| `Lee` | Recibir un dato. | `Lee edad` |
| `Escribe` | Mostrar un mensaje o resultado. | `Escribe total` |
| `=` | Asignar un valor a una variable. | `total = precio * cantidad` |
| `Si ... Sino` | Elegir entre caminos según una condición. | `Si nota >= 5 entonces` |
| `Según` | Elegir entre varias opciones. | `Según opcion entonces` |
| `Mientras` | Repetir mientras se cumpla una condición. | `Mientras contador > 0 hacer` |
| `Para` | Repetir un número conocido de veces. | `Para i en (1...10) hacer` |

No es necesario utilizar todas las primitivas. Para estos ejercicios, considera que el usuario introduce números enteros; no tienes que validar entradas de texto.

## Ejercicio 1 — Validar rango

**Archivo:** `ejercicio1.txt`

Solicita un número entre **1 y 10**, ambos incluidos. Si está fuera del rango, muestra un aviso y vuelve a pedirlo. Repite la petición hasta recibir un número válido y muestra un mensaje de confirmación.

**Ejemplo de interacción:**

```text
Introduce un número entre 1 y 10: 15
¡Inténtalo otra vez!
Dime un número (1-10): -2
¡Inténtalo otra vez!
Dime un número (1-10): 7
¡Correcto!
```

## Ejercicio 2 — Serie entre dos números

**Archivo:** `ejercicio2.txt`

Solicita dos números y muestra la serie de números enteros que los une, **incluyendo ambos extremos**.

- Si el primero es menor que el segundo, muestra la serie en orden ascendente.
- Si el primero es mayor, muestra la serie en orden descendente.
- Si son iguales, muestra ese número una sola vez.

Puedes mostrar los números separados por comas, espacios o saltos de línea.

**Ejemplo de interacción:**

```text
Introduce el primer número: 3
Introduce el segundo número: 8
Serie = 3, 4, 5, 6, 7, 8
```

**Otros casos:**

```text
Primer número: 5
Segundo número: 2
Serie = 5, 4, 3, 2
```

```text
Primer número: 4
Segundo número: 4
Serie = 4
```

## Ejercicio 3 — Ordenar tres números

**Archivo:** `ejercicio3.txt`

Solicita tres números y muéstralos en **orden ascendente**, de menor a mayor.

Utiliza variables y condiciones para ordenarlos, sin recurrir a funciones de ordenación. Si hay números repetidos, deben aparecer tantas veces como se hayan introducido.

**Ejemplo de interacción:**

```text
Introduce el primer número: 8
Introduce el segundo número: 3
Introduce el tercer número: 5
Números ordenados = 3, 5, 8
```

## Ejercicio 4 — Suma y cantidad de números

**Archivo:** `ejercicio4.txt`

Solicita números hasta que el usuario introduzca un **0**. Al terminar, muestra:

- Cuántos números se han introducido, **sin contar el 0**.
- La suma de todos ellos.

Los números pueden ser positivos o negativos. Si el primer número es 0, la cantidad y la suma deben ser 0.

**Ejemplo de interacción:**

```text
Introduce un número (0 para terminar): 5
Introduce un número (0 para terminar): 8
Introduce un número (0 para terminar): -2
Introduce un número (0 para terminar): 4
Introduce un número (0 para terminar): 0

Números introducidos = 4
Suma = 15
```

## Ejercicio 5 — Adivinar un número

**Archivo:** `ejercicio5.txt`

Genera **una sola vez**, al inicio del juego, un número secreto aleatorio entre **1 y 100**, ambos incluidos, utilizando:

```text
numSecreto = Aleatorio(1, 100)
```

Después:

- Pide números al usuario hasta que adivine el número secreto.
- Si no acierta, indica si el número secreto es **mayor o menor** que el introducido.
- Al acertar, muestra un mensaje de felicitación y el número total de intentos.

Cada número introducido cuenta como un intento, incluido el acierto final.

**Ejemplo de interacción:**

```text
ADIVINA EL NÚMERO ALEATORIO ENTRE 1 Y 100
---------------------------------------

Adivina el número: 25
El número secreto es mayor.

Adivina el número: 60
El número secreto es menor.

Adivina el número: 42
¡Correcto! Lo has conseguido en 3 intentos.
```
