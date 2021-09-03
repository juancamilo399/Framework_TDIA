# Cost Class

Este tipo de clases definen una función de costo, este tipo de clases tienen dos metodos
correspondientes a aplicar la función y la derivada de esta misma.

Este framework cuenta con varias funciones de costo. 

- SoftmaxCrossEntropy
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



