# Cost Class

Esta interfaz define una función de costo, este tipo de clases tienen dos métodos correspondientes a aplicar la función y la derivada de esta misma.

Este framework ofrece varias implementaciones de funciones de costo. 

- MeanSquaredError
- SigmoidCrossEntropy

## Apply Method

Metodo encargado de calcular el costo.

````
apply(a_last,y)
````

### Arguments

- a_last: Valores de salida predichos.
- y: Valores de salida reales.


## Grad Method

Metodo encargado de calcular la derivada.

````
grad(a_last,y)
````

### Arguments

- a_last: Valores de salida predichos.
- y: Valores de salida reales.



