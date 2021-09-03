# Activation Class

Este tipo de clases definen una función de activación, generalmente estas tienen dos metodos
correspondientes a aplicar la función y la derivada de esta misma.

Este framework cuenta con varias funciones de activación. 

- Sigmoid
- ReLu
- Softmax

***Los metodos de estas funciones son los siguientes.***

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


