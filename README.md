# Defectos-superficiales
  En la producción de laminados en caliente el control de calidad es un proceso necesario, para que el mismo esté libre de defectos y con ello evitar perjuicios económicos. Con lo cual se requiere de una optimización en el control de calidad.
  
  ----------
  # Objetivo #
  
  El objetivo de este trabajo es realizar un sistema que nos permita la detección de defectos existentes en las láminas en caliente de manera automática. 
  
 # Dataset #
 
 Este conjunto de datos de Kechen Song, Northeastern University (NEU). Se puede acceder por medio de la página  http://faculty.neu.edu.cn/me/songkc/Vision-based_SIS_Steel.html, compuesto por 1800 imágenes en escala de grises. El mismo está  constituido por los 6 tipos de defectos superficiales más comunes  de los laminados en caliente. 
 
 # Procesamiento #
 
 A partir del dataset, de manera aleatoria, se procedió a crear un conjunto de datos de entrenamiento y de testeo del 80% y 20% respectivamente.
 Dado que se tiene una cantidad limitada de imágenes, se realizó a un aumento de los mismos. 
 
 # Modelo #
 
 Para la extracción de características de los datos, se procedió a realizar una red neuronal convolucional por medio de las librerías TensorFlow y Keras.
 Se definió al modelo para un tamaño de muestras de 128, con 80 épocas. Teniendo una taza de aprendizaje de 0.0001.
 Por último se tienen  tres capas completamente conectadas, con tamaño de 500, 500 y 6 respectivamente. Con la función Sigmoid para las primeras dos capas, y Softmax.
