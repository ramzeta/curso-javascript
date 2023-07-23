<h3>

Aqui tenemos la solucion a la suma mas grande entre dos numeros adyacentes de un array:

</h3>


``````
function maxAdjacentSum(array) {
  if (array.length < 2) {
    return null; // o cualquier otro valor apropiado si el array no contiene suficientes elementos
  }

  let maxSum = -Infinity;

  for (let i = 0; i < array.length - 1; i++) {
    const currentSum = array[i] + array[i + 1];
    if (currentSum > maxSum) {
      maxSum = currentSum;
    }
  }

  return maxSum;
}
``````

<h3>

Otra solucion mas senior seria:


</h3>

``````
function maxAdjacentSum(array) {
  if (array.length < 2) {
    return null; // o cualquier otro valor apropiado si el array no contiene suficientes elementos
  }

  return array.slice(1).reduce((maxSum, current, index) =>
    Math.max(maxSum, current + array[index]), -Infinity);
}
``````