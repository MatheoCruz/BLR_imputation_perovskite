### Implementación de un algoritmo de imputación de datos de síntesis de celdas solares de perovskita utilizando el criterio de Bayesian Linear Regression BLR.

# 📑 BLR_imputation_perovskite

Mediante este proyecto se implementa un algoritmo que realiza dos procesos de imputación, los modelos emplean el criterio BLR, primero se realiza imputación para las variables de entrada y salida, y coo segundo modelo se realiza imputación mediante estimación para las variables de rendimiento/salida: *Voc, Jsc, PCE y FF.*

Este proyecto se hizo con la intención de ser replicable y utilizable sin importar la base de datos a utilizar, aclarando que algunas etapas, como lo es la de preprocesamiento, son únicas en este proyecto, dado que solucionan problemas y extraen características únicas de las bases de datos de interés presentadas.

## 💻 Instrucciones para los scripts
Para el correcto funcionamiento de este proyecto es importante seguir las instrucciones y tener en cuenta las pautas mencionadas. Cada script se encuentra relacionado con una etapa en específico.
- **📄 Preprocesamiento:** Esta etapa se encuenta relacionada con los scripts "Preprocesamiento_base_datos_imputar" y "Preprocesamiento_base_datos_complementaria".
- **📑 Construcción y entrenamiento del modelo:** Esta etapa se encuentra relacionada con los scripts "Proyecto_de_grado_imputacion" y "Proyecto_de_grado_estimacion".
- **📋 Evaluación:** Esta etapa se encuentra relacionada con los scripts "Evaluacion_imputacion" y "Evaluacion_estimacion".

Además para el correcto funcionamiento de este proyecto es importante la importación o descarga de los datos relacionados a cada script, dado el tamaño de estos se opto por crear un archivo en la nube que permita su descarga [Archivos_proyecto](https://drive.google.com/file/d/1uO6PLJAuZieIEYLc4G-VI5P_VzyKSaOS/view?usp=sharing).


El archivo "Archivos_proyecto" cuenta con 3 carpeta:
- **📚 Bases_datos:** Corresponden a las bases de datos utilizadas sin preprocesar "base_datos_sintesis", "Perovskite_database_content_all_data" que fungen como entradas de los scripts "Preprocesamiento_base_datos_imputar" y "Preprocesamiento_base_datos_complentaria".
- **📓 Datos_preprocesados:** En esta se encuentran la base de datos preprocesada "datos_sintesis" que funge como base de datos de entrenamiento en los scripts "Proyecto_de_grado_imputacion" y "Proyecto_de_grado_estimacion", además se encuentran los archivos "priori_x_grids" y "priori_y_grids" que permiten la construcción de las funciones de densidad de probabilidad a priori, lo que quiere decir que fungen como entradas de informacion previa de los modelos a entrenar en los scripts anteriormente mencionados.
- **📊 Resultados:** esta carpeta cuenta con dos subcarpetas
  - *Imputación:* Que son los resultados de la construcción del modelo del script "Proyecto_de_grado_imputacion" y fungen como entradas de el script "Evaluacion_imputacion"
  - *Imputación por estimación:* Que son los resultados de la construccion del modelo del script "Proyecto_de_grado_estimacion" y fungen como entradas de el script "Evaluacion_estimacion".
