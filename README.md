# Lab: Introducción a Arrays y Loops en JavaScript

Este laboratorio te ayudará a practicar los conceptos básicos de **arrays** y **loops** en JavaScript. Trabajarás con arrays, aprenderás cómo acceder a sus elementos y cómo recorrerlos utilizando bucles.

## Requisitos previos

Antes de comenzar este laboratorio, asegúrate de tener los siguientes conocimientos:

- Cómo declarar y utilizar variables
- Qué es un array y cómo se almacena una colección de datos en él
- Cómo funcionan los bucles (`for` y `while`)

---

## Ejercicio 1: Imprimir todos los elementos de un array

En este ejercicio, recorrerás un array e imprimirás cada uno de sus elementos.

### Instrucciones

1. Declara un array con algunos elementos, por ejemplo, nombres de frutas:
   ```javascript
   const frutas = ["manzana", "banana", "naranja"];
   ```
2. Usa un bucle `for` para recorrer el array y mostrar cada elemento en la consola.

### Pista

Recuerda que puedes acceder a los elementos de un array usando su índice, por ejemplo: `array[i]`.

### Ejemplo de código

```javascript
const frutas = ["manzana", "banana", "naranja"];

for (let i = 0; i < frutas.length; i++) {
  console.log(frutas[i]);
}
```

Esto debería mostrar en la consola:

```
manzana
banana
naranja
```

---

## Ejercicio 2: Encontrar el número más grande en un array

En este ejercicio, encontrarás el número más grande dentro de un array.

### Instrucciones

1. Declara un array de números, por ejemplo:
   ```javascript
   const numeros = [10, 3, 5, 20, 8];
   ```
2. Declara una variable llamada `max` y asígnale el valor del primer elemento del array.
3. Usa un bucle `for` para recorrer el array. Si encuentras un número mayor que `max`, actualiza el valor de `max`.
4. Al final, muestra el valor de `max` en la consola.

### Pista

Utiliza condicionales dentro del bucle para comparar los números.

### Ejemplo de código

```javascript
const numeros = [10, 3, 5, 20, 8];
let max = numeros[0]; // Inicializa con el primer número

for (let i = 1; i < numeros.length; i++) {
  if (numeros[i] > max) {
    max = numeros[i];
  }
}

console.log("El número más grande es:", max);
```

Esto debería mostrar en la consola:

```
El número más grande es: 20
```

---

## Ejercicio 3: Contar números pares en un array

En este ejercicio, contarás cuántos números pares hay dentro de un array.

### Instrucciones

1. Declara un array de números, por ejemplo:
   ```javascript
   const numeros = [1, 2, 3, 4, 5, 6];
   ```
2. Declara una variable llamada `contador` e inicialízala en 0.
3. Usa un bucle `for` para recorrer el array y, dentro del bucle, utiliza un condicional para verificar si un número es par (usa el operador `%`).
4. Si un número es par, incrementa `contador` en 1.
5. Al final, muestra el valor de `contador` en la consola.

### Pista

Un número es par si el resto de la división entre ese número y 2 es igual a 0 (es decir, `numero % 2 === 0`).

### Ejemplo de código

```javascript
const numeros = [1, 2, 3, 4, 5, 6];
let contador = 0;

for (let i = 0; i < numeros.length; i++) {
  if (numeros[i] % 2 === 0) {
    contador++;
  }
}

console.log("Cantidad de números pares:", contador);
```

Esto debería mostrar en la consola:

```
Cantidad de números pares: 3
```

---

## Ejercicio 4: Sumar todos los elementos de un array

En este ejercicio, sumarás todos los números dentro de un array.

### Instrucciones

1. Declara un array de números, por ejemplo:
   ```javascript
   const numeros = [1, 2, 3, 4, 5];
   ```
2. Declara una variable llamada `suma` e inicialízala en 0.
3. Usa un bucle `for` para recorrer el array y sumar cada número al valor de `suma`.
4. Al final, muestra el valor de `suma` en la consola.

### Pista

Asegúrate de sumar cada número del array a la variable `suma` dentro del bucle.

### Ejemplo de código

```javascript
const numeros = [1, 2, 3, 4, 5];
let suma = 0;

for (let i = 0; i < numeros.length; i++) {
  suma += numeros[i];
}

console.log("La suma total es:", suma);
```

Esto debería mostrar en la consola:

```
La suma total es: 15
```

---

## Notas adicionales

- Asegúrate de probar cada ejercicio con diferentes arrays para comprobar que tu código funciona correctamente.
- Si algo no funciona como esperabas, revisa cómo estás accediendo a los elementos del array o cómo estás utilizando los bucles.
- Usa `console.log()` para ver los resultados de tus pruebas y depurar tu código si es necesario.

¡Disfruta programando y practicando arrays y loops!
