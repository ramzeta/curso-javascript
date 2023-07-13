Para este reto tenemos que ordenar un array sin .sort.
Utilizaremos algoritmos de ordenamientos diferentes.
https://es.wikipedia.org/wiki/Algoritmo_de_ordenamiento

Aquí está el código en JavaScript que implementa Bubble Sort:

``````
function bubbleSort(arr) {
  var len = arr.length;
  for (var i = 0; i < len; i++) {
    for (var j = 0; j < len - 1; j++) {
      if (arr[j] > arr[j + 1]) {
        var temp = arr[j];
        arr[j] = arr[j + 1];
        arr[j + 1] = temp;
      }
    }
  }
  return arr;
}

// Ejemplo:
var myArray = [3, 2, 1, 5, 4];
console.log(bubbleSort(myArray)); // [1, 2, 3, 4, 5]



Aquí está el código en JavaScript que implementa ordenamiento por inserción:

function insertionSort(arr) {
  for (let i = 1; i < arr.length; i++) {
    let current = arr[i];
    let j = i - 1;
    while (j >= 0 && arr[j] > current) {
      arr[j + 1] = arr[j];
      j--;
    }
    arr[j + 1] = current;
  }
  return arr;
}

// Ejemplo:
var myArray = [5, 6, 4, 8, 7];
console.log(insertionSort(myArray)); // [ 4, 5, 6, 7, 8 ]
``````