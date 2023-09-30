# BLR_imputation_perovskite
Imputación de datos faltantes de parámetros de síntesis y rendimiento de celdas solares de perovskite, implementando una regresión lineal bayesiana (BLR).

Este proyecto se hizo con la intencion de ser replicable y utilizable sin importar la base de datos a utilizar, claro esta que algunas etapas como es la de preprocesamiento, son unicas en este proyecto, dado que solucionan problemas y extraen caracteristicas unicas de las bases de datos de interes presentadas.

## Instrucciones
Para el correcto funcionamiento de este proyecto es importante seguir las instruccione y tener en cuenta las pautas mencionadas. Cada script se encuentra relacionado con una etapa en especifico.
- Preprocesamiento: Esta etapa se encuenta relacionada con los scripts "Preprocesamiento_base_datos_imputar" y "Preprocesamiento_base_datos_complementaria".
- Construccion y entrenamiento del modelo: Esta etapa se encuentra relacionada con los scripts "Proyecto_de_grado_imputacion" y "Proyecto_de_grado_estimacion".
- Evaluacion: Esta etapa se encuentra relacionada con los scripts "Evaluacion_imputacion" y "Evaluacion_estimacion".

Ademas para el correcto funcionamiento de este proyecto es importante la importacion o descarga de los datos relacionados a cada script, dado el tamaño de estos se opto por crear un archivo en la nube que permita su descarga "https://drive.google.com/file/d/17lrKxfZ3qhqc4CE9S13kwbI4OAU11xb2/view?usp=drive_link".

El archivo "Archivos_proyecto" cuenta con 3 carpeta:
- Bases_datos: corresponden a las bases de datos utilizadas sin preprocesar "base_datos_sintesis", "Perovskite_database_content_all_data" que fungen como entradas de los scripts "Preprocesamiento_base_datos_imputar" y "Preprocesamiento_base_datos_complentaria".
- Datos_preprocesados: en esta se encuentran la base de dato preprocesada "datos_sintesis" que funge como base de datos de entrenamiento en los scripts "Proyecto_de_grado_imputacion" y "Proyecto_de_grado_estimacion", ademas se encuentran los archivos "priori_x_grids" y "priori_y_grids" que permiten la construccion de las funciones de densidad de probabilidad a priori, lo que quiere decir que fungen como entradas de informacion previa de los modelos a entrenar en los scripts anteriormente mencionados.
- Resultados: esta carpeta cuenta con dos subcarpetas
  - Imputacion: Que son los resultados de la construccion del modelo del script "Proyecto_de_grado_imputacion" y fungen como entradas de el script "Evaluacion_imputacion"
  - Imputacion por estimacion: Que son los resultados de la construccion del modelo del script "Proyecto_de_grado_estimacion" y fungen como entradas de el script "Evaluacion_estimacion".


