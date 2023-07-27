## Introducción a JavaScript

JavaScript es un lenguaje de programación interpretado utilizado principalmente para desarrollar aplicaciones web interactivas. Es un lenguaje de scripting del lado del cliente, lo que significa que se ejecuta en el navegador del usuario.

### Características principales

- **Interpretado**: JavaScript no requiere un proceso de compilación. El código fuente se interpreta directamente en tiempo de ejecución.

- **Lenguaje orientado a objetos**: JavaScript admite la programación orientada a objetos, lo que permite la creación y manipulación de objetos y clases.

- **Dinámico**: Las variables en JavaScript no están vinculadas a tipos de datos específicos y pueden cambiar su tipo durante la ejecución del programa.

### Uso en el navegador web

JavaScript se utiliza principalmente para mejorar la interactividad de los sitios web. Puede ser utilizado para:

- **Manipulación del DOM**: JavaScript puede modificar y manipular elementos HTML en tiempo real, lo que permite actualizar el contenido y responder a eventos del usuario.

- **Validación de formularios**: Puedes utilizar JavaScript para validar los datos ingresados por los usuarios en formularios web antes de enviarlos al servidor.

- **Animaciones y efectos visuales**: JavaScript puede controlar la animación y los efectos visuales en un sitio web, creando una experiencia más dinámica y atractiva.

### Uso en el servidor

Además de su uso en el navegador, JavaScript también se puede utilizar en el lado del servidor utilizando entornos como Node.js. Algunos casos de uso comunes en el desarrollo del lado del servidor son:

- **Manipulación de archivos**: JavaScript puede leer y escribir archivos en el sistema de archivos del servidor.

- **Construcción de API**: Puedes crear y exponer API RESTful utilizando JavaScript en el lado del servidor para permitir la comunicación con aplicaciones cliente.

- **Acceso a bases de datos**: JavaScript puede interactuar con bases de datos y realizar consultas para recuperar o modificar datos.

### Ejemplo básico

Aquí hay un ejemplo simple de código JavaScript que muestra un mensaje de saludo en el navegador:

```javascript
// Definición de una función para mostrar un saludo
function saludar(nombre) {
  console.log('¡Hola, ' + nombre + '!');
}

// Llamada a la función de saludo
saludar('Ramiro');
