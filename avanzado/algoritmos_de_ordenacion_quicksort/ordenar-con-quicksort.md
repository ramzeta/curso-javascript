<h3>Quicksort se creó como un algoritmo de ordenación eficiente y rápido. Fue desarrollado por el científico británico Tony Hoare en 1959. Quicksort se destaca por su eficiencia en la práctica y su capacidad para manejar grandes volúmenes de datos de manera efectiva.</h3>

La función quicksort recibe un array (arr) que se desea ordenar, junto con dos índices low y high que representan el rango de elementos en el array que se deben ordenar.
Dentro de la función, se verifica si el índice low es menor que high. Si esto se cumple, significa que hay al menos dos elementos en el rango actual que deben ser ordenados.
A continuación, se llama a la función partition pasando el array, low y high. La función partition se encarga de encontrar un pivote y reorganizar los elementos del array de manera que los elementos menores al pivote estén a su izquierda y los mayores estén a su derecha.
Después de obtener el índice de partición, se llama recursivamente a la función quicksort dos veces más para ordenar los subarreglos. La primera llamada es para ordenar los elementos a la izquierda del pivote, desde low hasta partitionIndex - 1. La segunda llamada es para ordenar los elementos a la derecha del pivote, desde partitionIndex + 1 hasta high.
Este proceso de partición y recursión se repite hasta que no haya más elementos por ordenar, es decir, cuando low sea mayor o igual a high. En ese punto, la recursión se detiene y el array se considera completamente ordenado.


``````
function quicksort(arr, low, high) {
  if (low < high) {
    const partitionIndex = partition(arr, low, high);
    quicksort(arr, low, partitionIndex - 1);
    quicksort(arr, partitionIndex + 1, high);
  }
}

``````

La función partition es utilizada por quicksort para encontrar el índice de partición. Toma el array, low y high como parámetros.
La función selecciona un pivote, que en este caso es el último elemento del rango (arr[high]).
Se inicializa una variable i con el valor low - 1.
A continuación, se itera desde low hasta high - 1 utilizando la variable j.
En cada iteración, se compara el elemento arr[j] con el pivote. Si es menor o igual, se incrementa i y se realiza un intercambio de posiciones entre los elementos arr[i] y arr[j] utilizando la función swap.
Después del bucle, se realiza un último intercambio de posiciones entre arr[i + 1] y el pivote arr[high].
Por último, se devuelve i + 1, que representa el índice de partición.

``````
function partition(arr, low, high) {
  const pivot = arr[high];
  let i = low - 1;

  for (let j = low; j < high; j++) {
    if (arr[j] <= pivot) {
      i++;
      swap(arr, i, j);
    }
  }

  swap(arr, i + 1, high);
  return i + 1;
}
``````

La función swap se utiliza para intercambiar dos elementos en el array. Toma como parámetros el array y los índices i y j.
Se almacena temporalmente el valor del elemento en arr[i] en la variable temp.
Luego, se asigna el valor del elemento en arr[j] a arr[i].
Finalmente, se asigna el valor almacenado en temp a arr[j], completando así el intercambio.

``````
function swap(arr, i, j) {
  const temp = arr[i];
  arr[i] = arr[j];
  arr[j] = temp;
}
``````
// Ejemplo de uso:


Este fragmento de código muestra un ejemplo de uso del algoritmo Quicksort. Crea un array llamado array con una serie de números desordenados.
Luego, se llama a la función quicksort pasando el array, el índice inicial (0) y el índice final (array.length - 1).
Después de que quicksort haya finalizado la ordenación, se imprime el array ordenado utilizando console.log(array).

``````
const array = [7, 2, 1, 6, 8, 5, 3, 4];
quicksort(array, 0, array.length - 1);
console.log(array);
``````

Los algoritmos de ordenación se crearon para mejorar la eficiencia de las operaciones, facilitar la búsqueda y la visualización de datos, permitir el análisis y procesamiento de datos de manera más efectiva, y cumplir con los requisitos de estructuras de datos específicas. Son una herramienta fundamental en ciencias de la computación y juegan un papel crucial en numerosas aplicaciones y problemas.
