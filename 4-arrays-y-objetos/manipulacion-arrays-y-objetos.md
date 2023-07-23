## Manipulación de Arrays y Objetos en JavaScript


## Arrays 


<h3>Crear un array</h3>

```
// Crear un array vacío
let arrayVacio = [];

// Crear un array con elementos
let miArray = [1, 2, 3, 4, 5];
```

<h3>Acceder a los elementos de un Array</h3>

```
// Acceder al primer elemento
let primerElemento = miArray[0];

// Acceder al último elemento
let ultimoElemento = miArray[miArray.length - 1];
```

<h3>Modificar elementos de un Array</h3>

```
let miArray = [1, 2, 3, 4, 5];
miArray[2] = 10; // Modifica el tercer elemento del array y le asigna el valor 10
```

<h3> Eliminar elementos de un array </h3>

Existen varios métodos para eliminar elementos de un array en JavaScript, como el método pop() que elimina el último elemento del array, el método shift() que elimina el primer elemento del array, y el método splice() que permite eliminar elementos en posiciones específicas del array. Por ejemplo:

```
let miArray = [1, 2, 3, 4, 5];
miArray.pop(); // Elimina el último elemento del array (5)
miArray.shift(); // Elimina el primer elemento del array (1)
miArray.splice(1, 2); // Elimina 2 elementos a partir del índice 1 del array ([2, 4])
```



## Objetos

<h3>Crear un Objeto</h3>

```
// Crear un objeto vacío
let objetoVacio = {};

// Crear un objeto con propiedades
let miObjeto = {
  nombre: "Juan",
  edad: 25,
  profesion: "programador"
};
```

<h3>Acceder a las propiedades de un Objeto</h3>

```
// Acceder a una propiedad
let nombre = miObjeto.nombre;

// Acceder a una propiedad con notación de corchetes
let edad = miObjeto["edad"];
```

<h3>Modificar propiedades de un Objeto</h3>

```
// Modificar una propiedad existente
miObjeto.edad = 30;

// Añadir una nueva propiedad al objeto
miObjeto.pais = "España";

// Eliminar una propiedad del objeto
delete miObjeto.profesion;
`````

Si necesitas ayuda adicional, no dudes en preguntar.

<b>References:</b><br>
<span> <a href='https://hackernoon.com/array-manipulation-understanding-javascript-array-methods' target='_blank' class='text-purple-1 underline'>Array Manipulation: Understanding JavaScript Array Methods</a></span><br>
<span> <a href='https://www.digitalocean.com/community/tutorials/how-to-use-array-methods-in-javascript-mutator-methods' target='_blank' class='text-purple-1 underline'>How To Use Array Methods in JavaScript: Mutator Methods</a></span><br>
<span><a href='https://www.freecodecamp.org/news/the-javascript-array-handbook/' target='_blank' class='text-purple-1 underline'>The JavaScript Array Handbook – JS Array Methods ...</a></span>