# CNN: Detección de Neumonía a partir de imágenes de rayos X

[Joel Ricci López](http://joelriccilopez.com/), 2021. 

***

## 🤔 Descripción

Implementación de un **modelo de clasificación mediante redes neuronal convolucionales** para la **identificación de casos de neumonía**  presentado  en [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).  

### Objetivos

- Obtendrémos el *dataset* y procesaremos las imágenes y realizaremos un análisis exploratorio de éstas.
  - Tendremos en cuenta el desbalance de clases al momento de obtener los conjuntos de `entrenamiento`, `validación`, y `prueba`.
- Usaremos `Keras` y su API `Sequential` para crear una red capa por capa. 
- Además compararemos el desempeño de nuestra red contra un modelo creado a partir de **Transfer Learning**, utilizando la red preentrenada (`VGG16`)[https://arxiv.org/abs/1409.1556].`
- Evaluaremos la "Explicabilidad" del modelo utilizando el método Grad-CAM, en el que visualmente exploraremos en qué zonas de las imágenes se enfocó el modelo de DeepLearning para llevar a cabo la clasificación.

## 📊 Contenido

El orden de los notebooks es el siguiente:

| Nombre del notebook | Descripción | Abrir en Colab |
| ------------- | ------------- | ------------- |
| `1_Preprocess_CNN_Pneumonia` | Obtención y preprocesamiento | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jRicciL/ML_and_DataScience_projects/blob/master/ConvNets_and_GradCAM_Xray_dataset/1_Preprocess_CNN_Pneumonia.ipynb)`|
| `2_ConvolutionalNN_PNEUMONIA_X_ray` | Implementación de la ConvNet y *Transfer Learning*| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jRicciL/Aprendizaje_profundo_tareas_CICESE/blob/master/ConvNets_and_GradCAM_Xray_dataset/2_ConvolutionalNN_PNEUMONIA_X_ray.ipynb) |
| `3_GradCAM_ConvNet_Explainability` | *Model Explainability* mediante Grad-CAM | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jRicciL/Aprendizaje_profundo_tareas_CICESE/blob/master/ConvNets_and_GradCAM_Xray_dataset/3_GradCAM_ConvNet_Explainability.ipynb)|


## 📚 Referencias

1. Mariano Rivera (2018). **[Reeuso de Redes Preentrenadas](http://personal.cimat.mx:8181/~mrivera/cursos/aprendizaje_profundo/preentrenadas/preentrenadas.html)**. *Consultado el 18 de marzo del 2021.*
2. Eunjoo Byeon (2020). **[Exploratory Data Analysis Ideas for Image Classification](https://towardsdatascience.com/exploratory-data-analysis-ideas-for-image-classification-d3fc6bbfb2d2)**. En towardsdatascience.com. *Consultado el 18 de marzo del 2021.*
3. Paul Mooney (2018). **[Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)**. En kaggle.com. *Consultado el 18 de marzo del 2021.*
4. Chollet, Francois (2017). **Deep Learning with Python.** New York, NY: Manning Publications.
