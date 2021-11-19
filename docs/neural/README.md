# Red Neuronal (*Feed Fordward Neural Network*)

## Neural Network Class

A continuación se detalla la definición de la clase NeuralNetwork

````
 NeuralNetwork(is_classification,is_binary,input_dim,layers,cost_function,optimizer)
````

### Arguments

- is_classification: Valor booleano que indica el tipo de problema (clasificación o regresión).
- is_binary: Valor booleano que indica si es un problema de clasificación binaria o no.
  
- input_dim: Tupla de n elementos indicando las dimensiones de los datos de
entrada a la red.

- layers: Lista de instancias de tipo layer indicando la arquitectura de la red a 
nivel de capas.

- cost_function: Instancia de una clase que define una funcion de costo.

- optimizer: Instancia de una clase que define un optimizador.

## Train Method

Metodo encargado de realizar en entrenamiento de la red neuronal.
    
````
 neuralNetwork.train(x_train,y_train,learning_rate,num_epochs)
````

### Arguments

- x_train: Matriz correspondiente a los datos de entrada.

- y_train: Matriz correspondiente a los datos de salida.

- learning_rate: Tasa de aprendizaje del modelo.

- num_epochs: Número de epocas de entrenamiento.

- test_data: Tupla con los datos de prueba.





## Predict Method

Metodo encargado de realizar la predicción dado unos datos de entrada.
    
````
 neuralNetwork.predict(x)
````

### Arguments

- x: Matriz correspondiente a los datos de entrada.

### Returns

- a_last: Salida de la ultima capa de la red.



## Usage

A continuación se detalla el uso de este framework.

Primeramente es necesario definir el modelo de la red neuronal que se usará para esto es necesario instanciar un objeto del tipo NeuralNetwork.

A continuación se presenta un ejemplo de esta inicialización donde se especifica la dimensión de entrada, la lista de capas donde cada una indica su número de neuronas y función de activación, además se indica la función de costo y el optimizador a usar. De esta manera se definiria la arquitectura de la red neuronal para posteriormente entrenarla y usarla para predecir.

````
nn = NeuralNetwork(is_classification,is_binary,
    input_dim=(x_train.shape[1]),
    layers=[
            FullyConnected(64, ReLu),
            FullyConnected(32, ReLu),
            FullyConnected(10, Sigmoid)      
        ],
        cost_function=SigmoidCrossEntropy,
        optimizer=GradientDescent
        
    )
    
````

### Entrenamiento y predicción

Una vez definida la arquitectura de la red neuronal se procede a realizar el entrenamiento de la misma donde se especifican los datos de entrada y de salida con los que se entrenará, asi como la tasa de aprendizaje y el número de epocas.

Finalmente con el modelo entrenado este es capaz de realizar predicciones sobre a un conjunto de datos de entrada donde las diferencias entre las salidas predichas y las salidas reales será muy poca. 

