# Layer Interface

Esta interfaz define una capa de la red neuronal, la implementación expuesto corresponde a una capa de tipo FullyConnected.

## FullyConnected

A continuación se detalla la definición de la clase FullyConnected

````
 FullyConnected(size,activation)
````

### Arguments

- size: La cantidad de neuronas de dicha capa

- activation: Instancia de una clase que define una función de activación.


> Al momento de inicializar el modelo de red neuronal se realiza un
procedimiento por cada capa donde se obtienen las dimensiones de entrada a esta, inicializando de 
>esta manera sus respectivos pesos.


## Forward Method

Metodo encargado de realizar la propagación hacia adelante.

````
 forward(a_prev,training)
````

### Arguments

- a_prev: Valor de activación de la capa anterior

- training: Valor booleano que indica si el modelo está siendo entrenado.

### Return

- a: Valor de activación.

## Backward Method

Metodo encargado de realizar la propagación hacia atras.

````
 backward(da)
````

### Arguments

- da: Gradiente de la capa posterior.

### Return

- da_prev: Gradiente calculado

- dw: Gradiente correspondiente a los pesos

- db: Gradiente correspondiente al bias


