## Librerías y Frameworks de JavaScript

1. React
Descripción: React es una biblioteca de JavaScript creada por Facebook que se utiliza para construir interfaces de usuario interactivas y reactivas. Es ampliamente utilizada en el desarrollo web moderno y se basa en el concepto de componentes reutilizables.

Ejemplo: Un componente simple de React que muestra un saludo.

``````
import React from 'react';

const Greeting = ({ name }) => {
  return <h1>Hola, {name}!</h1>;
};

// Uso del componente
ReactDOM.render(<Greeting name="Juan" />, document.getElementById('root'));
``````

2. Angular
Descripción: Angular es un framework de JavaScript desarrollado por Google que se utiliza para crear aplicaciones web de una sola página (SPA). Proporciona una estructura sólida y funcionalidades poderosas para crear aplicaciones complejas.

Ejemplo: Un componente simple en Angular que muestra un saludo similar al ejemplo anterior de React.


``````
<!-- archivo: greeting.component.html -->
<h1>Hola, {{ name }}!</h1>

// archivo: greeting.component.ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-greeting',
  templateUrl: './greeting.component.html',
})
export class GreetingComponent {
  name = 'Juan';
}

``````

3. Vue.js
Descripción: Vue.js es otro framework de JavaScript para construir interfaces de usuario interactivas. Es más liviano que React y Angular, lo que lo hace ideal para proyectos pequeños y medianos.

Ejemplo: Un componente simple de Vue.js que muestra un saludo similar al ejemplo anterior.

```````
<!-- archivo: greeting.vue -->
<template>
  <h1>Hola, {{ name }}!</h1>
</template>

<script>
export default {
  data() {
    return {
      name: 'Juan',
    };
  },
};
</script>

```````


4. Express.js
Descripción: Express.js es un framework minimalista de JavaScript para construir aplicaciones web y APIs. Es muy popular y se basa en Node.js, lo que lo hace adecuado para crear aplicaciones rápidas y escalables del lado del servidor.

Ejemplo: Un servidor HTTP simple utilizando Express.js que devuelve "Hola Mundo" como respuesta.

``````
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Hola Mundo');
});

app.listen(port, () => {
  console.log(`Servidor escuchando en http://localhost:${port}`);
});

``````