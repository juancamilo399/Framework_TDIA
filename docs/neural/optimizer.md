# Optimizer Interface

Esta interfaz define un optimizador. Este define la forma en la que la red neuronal es optimizada, es decir la forma en la que sus pesos son actualizados. La implementación expuesta corresponde a un optimizador del tipo GradientDescent .

## GradientDescent

A continuación se detalla la definición de la clase GradientDescent

````
 GradientDescent(trainable_layers)
````

### Arguments

- trainable_layers: Lista de capas sobre las cuales se actualizaran los pesos

## Update Method

Metodo encargado de realizar la actualizacion de los pesos de capa capa.

````
 update(learning_rate,w_grads,b_grads)
````

### Arguments


- learning_rate: Valor de la tasa de aprendizaje

- w_grads: Gradientes correspondientes a los pesos.

- b_grads: Gradientes correspondientes al bias



