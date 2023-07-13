## Objetos y manipulación del DOM

### Introducción a los objetos en JavaScript

En JavaScript, los objetos son estructuras de datos que contienen propiedades y métodos relacionados. Proporcionan una forma de organizar y manipular datos de manera más eficiente. Un objeto puede representar un concepto del mundo real o cualquier entidad que necesites modelar en tu aplicación.

#### Creación de objetos

En JavaScript, puedes crear un objeto utilizando la sintaxis de llaves (`{}`) y asignando propiedades y valores a ese objeto. Por ejemplo:

// Creación de un objeto persona
``````
let persona = {
nombre: 'Ramiro',
edad: 34,
profesion: 'Programador'
};
``````
En este ejemplo, se crea un objeto `persona` con tres propiedades: `nombre`, `edad` y `profesión`.

#### Acceso a propiedades de objetos

Puedes acceder a las propiedades de un objeto utilizando la notación de punto (`objeto.propiedad`) o la notación de corchetes (`objeto['propiedad']`). Por ejemplo:
``````
console.log(persona.nombre); // Salida: 'Ramiro'
console.log(persona['edad']); // Salida: 34
``````
### Manipulación del DOM (Document Object Model)

El DOM es una representación en forma de árbol de la estructura HTML de un documento. En JavaScript, puedes manipular el DOM para seleccionar y modificar elementos HTML.

#### Selección de elementos HTML

Puedes seleccionar elementos HTML utilizando métodos como `getElementById`, `getElementsByClassName`, `getElementsByTagName` o `querySelector`. Por ejemplo:

``````
let miParrafo = document.getElementById('miParrafo');
let misElementos = document.getElementsByClassName('misElementos');
let miBoton = document.querySelector('button');
``````
En este ejemplo, `getElementById` selecciona un elemento con el id `miParrafo`, `getElementsByClassName` selecciona elementos con la clase `misElementos` y `querySelector` selecciona el primer botón que encuentre en el documento.

#### Modificación de elementos HTML

Una vez que has seleccionado un elemento HTML, puedes modificar su contenido, atributos y estilos utilizando las propiedades y métodos del objeto seleccionado. Por ejemplo:
``````
miParrafo.textContent = 'Nuevo texto'; // Cambia el contenido del párrafo
miBoton.disabled = true; // Deshabilita el botón
miBoton.style.backgroundColor = 'red'; // Cambia el color de fondo del botón
``````

En este ejemplo, se cambia el contenido del párrafo utilizando la propiedad `textContent`, se deshabilita el botón utilizando la propiedad `disabled` y se cambia el color de fondo del botón utilizando la propiedad `style.backgroundColor`.

El objeto `document` es la entrada al árbol del DOM y proporciona métodos para interactuar con los elementos HTML.

---

¡Con esto concluye la introducción a los objetos en JavaScript y la manipulación del DOM! Estos conceptos son fundamentales para construir aplicaciones web interactivas.
