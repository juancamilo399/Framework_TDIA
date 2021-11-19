# Activation Class

Esta interfaz define una función de activación, generalmente estas tienen dos métodos correspondientes a aplicar la función y la derivada de esta misma.

Este framework ofrece varias implementaciones de funciones de activación. 

- Sigmoid
- ReLu
- Linear
- Tanh


## Apply Method

Metodo encargado de calcular el valor de activación.

````
apply(x)
````

### Arguments

- x: Valor de preactivación


## df Method

Metodo encargado de calcular la derivada.

````
df(x)
````

### Arguments

- x: Valor de preactivación


