## Sintaxis básica de JavaScript

### Comentarios

Los comentarios en JavaScript son utilizados para agregar notas o explicaciones dentro del código. Se pueden escribir de dos formas:

```javascript
// Este es un comentario de una línea

/*
  Este es un comentario
  de múltiples líneas
*/
```

### Variables

En JavaScript, se utilizan variables para almacenar y manipular datos. La declaración de una variable se realiza utilizando las palabras clave `var`, `let` o `const`. Por ejemplo:

```javascript
// Declaración de variables
var x = 5;
let y = 10;
const z = 15;

// Modificación de variables
x = 8;
y = y + 2;
```

### Tipos de datos

JavaScript tiene varios tipos de datos integrados, entre ellos:

- Números: `let edad = 25;`
- Cadenas de texto: `let nombre = 'Juan';`
- Booleanos: `let esMayor = true;`
- Arreglos: `let numeros = [1, 2, 3, 4, 5];`
- Objetos: `let persona = { nombre: 'Juan', edad: 25 };`

### Estructuras de control

JavaScript ofrece varias estructuras de control para tomar decisiones y repetir acciones:

#### Condicional if-else

```javascript
let edad = 18;

if (edad >= 18) {
  console.log('Eres mayor de edad');
} else {
  console.log('Eres menor de edad');
}
```

#### Bucle for

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

#### Bucle while

```javascript
let contador = 0;

while (contador < 5) {
  console.log(contador);
  contador++;
}
```

### Funciones

Las funciones en JavaScript permiten agrupar instrucciones y reutilizar código:

```javascript
function saludar(nombre) {
  console.log('¡Hola, ' + nombre + '!');
}

saludar('Juan');
```

En este ejemplo, se define una función llamada `saludar` que recibe un parámetro `nombre` y muestra un saludo en la consola.

Esto es solo una introducción a la sintaxis básica de JavaScript. El lenguaje ofrece muchas más características y conceptos avanzados. ¡Explora y diviértete programando en JavaScript!

Si tienes más preguntas, no dudes en hacerlas.
