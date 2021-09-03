# Red Neuronal (*Feed Fordward Neural Network*)

## Neural Network Class

A continuación se detalla la definicion de la clase NeuralNetwork

````
 NeuralNetwork(input_dim,layers,cost_function,optimizer)
````

### Arguments

- input_dim: Tupla de n elementos indicando las dimensiones de los datos de
entrada a la red.

- layers: Lista de instancias de tipo layer indicando la arquitectura de la red a 
nivel de capas.

- cost_function: Instancia de una clase que define una funcion de costo.

- optimizer: Instancia de una clase que define un optimizador.

## Train Method

Metodo encargado de realizar en entrenamiento de la red neuronal.
    
````
 NeuralNetwork.train(x_train,y_train,learning_rate,num_epochs,test_data)
````

### Arguments

- x_train: Matriz correspondiente a los datos de entrada.

- y_train: Matriz correspondiente a los datos de salida.

- learning_rate: Tasa de aprendizaje del modelo.

- num_epochs: número de epocas de entrenamiento.

- test_data: Tupla con los datos de prueba.