# AprendizajeProfundo

### Integrantes:

#### BORNANCINI, Veronica
#### FERNANDEZ, Maria Soledad
#### LOTO, Patricia
#### OLARIAGA, Sandra

**Este repositorio contiene:**

* el [código](https://github.com/msoledadfernandez/AprendizajeProfundo/tree/main/experiment) en donde se han analizado y modelado Redes Neuronales de tipo **Perceptrón Multicapa** (**MLP**) y **Convulsionales** (**CNN**). 
* [documento pdf](https://github.com/msoledadfernandez/AprendizajeProfundo/blob/main/resultados_experimentos_utilizando_mlp_y_cnn.pdf) con el detalle de cada experimento con sus hiperparámetros y gráficos correspondientes.

Los resultados de los experimentos utilizando MLP se encuentran en [mlrunsMLP](https://drive.google.com/file/d/13wxlh7DO11PZBOKDP0--OMsrs8sApoU3/view?usp=sharing)
y los resultados utilizando CNN se encuentran en [mlrunsCNN](https://drive.google.com/file/d/1oZNxKjFs0E7u9NMMHJffwV9DB444xVWT/view?usp=sharing).

### **Conclusiones**

Como sabemos, el train loss representa el error en el conjunto de datos de entrenamiento, y el validation loss el error después de ejecutar el conjunto de datos de validación a través de la red entrenada. Por lo tanto, debemos tener cuidado cuando observamos un validation loss mucho mayor que el train loss ya que puede ser una señal de que el modelo está sobreajustado y aprende "supersticiones", es decir, patrones que accidentalmente eran ciertos en sus datos de entrenamiento pero que no tienen una base en la realidad y, por lo tanto, no son ciertos en sus datos de validación.

En los distintos experimentos realizados se observa que, 

* cuando la métrica **balance accuracy** aumenta, disminuyen tanto la **función loss de validation** como la de **train** 

* aunque no pudimos utilizar muchas épocas por la limitación de recursos pudimos observar que a medida que estás aumentan, el balanced accuracy aumenta y disminuyen tanto el error en la validación como en el entrenamiento.

* con los hiperparámetros que usamos en base a los recursos disponibles podemos decir que el modelo que tuvo un nivel de acierto superior en las fase de training y validation es el experimento nro. 1 de la red neuronal tipo Perceptrón Multicapa o MLP, con un balancend accuracy igual a **0.482**. 
* también se observa una disminución de los valores de pérdidas de los conjuntos de validation y train, con un train loss igual a **2,485** y un validation loss igual a **2,459**.

Por último, cabe aclarar que los casos de prueba fueron restringidos por la situación mencionada anteriormente, por lo cual no se descarta que con otros seteos de hiperpárametros se alcanzaría un nivel superior de acierto.
