## Nombre de este equipo: 

equipo-c24-10-n-data

## Vertical tecnológica del proyecto: 

Data - BI

## 👥 Integrantes

<div align="left">
  <table>
    <thead>
      <tr>
        <th>Integrante</th>
        <th>Rol</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><b>Jesús Joaquín Cerón Melgoza</b></td>
        <td>Analista de datos (Data analyst) </td>
      </tr>
      <tr>
        <td><b>Alondra Ferra Muñiz</b></td>
        <td>Analista de datos (Data analyst) </td>
      </tr>
    </tbody>
  </table>
</div>

## Team Leader:

<b>Brayan Córdova</b>

## Nombre del proyecto:

<b>Dashboard ENTCO</b>

## 📄Descripción del proyecto:

El dashboard ENTCO, desarrollado en Tableau Public, es una herramienta interactiva diseñada para monitorear indicadores clave relacionados con enfermedades no transmisibles, crónicas y oncológicas en América. Este proyecto busca apoyar a hospitales y clínicas, ofreciéndoles información estratégica basada en datos internos y externos para mejorar la calidad y efectividad de los servicios de salud.

Los datos externos juegan un papel esencial al identificar tendencias internacionales, segmentar poblaciones según factores demográficos y analizar la demanda de servicios y recursos. De esta forma, las instituciones de salud pueden anticiparse a las necesidades de los pacientes y optimizar sus procesos.

Este proyecto se basa en dos conjuntos de datos: uno se encuentra en Kaggle y el otro es de la Organización Panamericana de la Salud, asegurando una base sólida y confiable para la toma de decisiones.

## 📖Conjuntos de datos utilizados:

Fuente 1: 

El conjunto de datos de la Organización Panamericana de la Salud (PAHO por sus siglas en inglés) fue descargado el día 3 de marzo de 2025, y su última actualización fue el día 14 de enero de 2025. El archivo original contiene 27 columnas, sin embargo, se ha decidido delimitar el análisis de datos a 5 columnas de datos y a 150 indicadores.

Fuente 2: 

El conjunto de datos de "National Institute of Diabetes and Digestive and Kidney Diseases" fue descargado el día 04 de marzo de 2025, y su última actualización fue el día 08 de abril de 2022. El archivo original contiene 9 columnas, se ha decidido mantener la integridad del dataframe para su abordaje en el presente proyecto.

## 📖Archivos CSV usados en Google Colab

Los siguientes enlaces permiten descargar los archivos originales utilizados en Google Colab:

Archivo 1:
https://drive.google.com/file/d/1FeNg3pMyvOutFTSC6rJP3czoCFm_qPIo/view?usp=sharing

Archivo 2:
https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset


## ➡️Descripción de los pasos de exploración, preparación y selección de los datos (etapa previa a la visualización de datos)

Conjunto de datos 1

El primer paso fue escribir un bloque de código dentro de una celda en un archivo de Google Colab denominado “notebook”. El bloque de código correspondiente al primer paso contiene líneas de código para importar la librería pandas y permitir utilizar archivos, una función que permite subir archivos CSV a Google Colab, se utilizó el método df.info() para obtener un resumen del archivo CSV que permite mostrar la cantidad de valores no nulos de cada columna y se usó un ciclo con instrucciones que permitir ver los valores únicos y la cantidad de valores únicos de cada columna. El archivo original que se utilizó al ejecutar el bloque de código escrito en la celda se llama "PAHO-Core-Indicators-2024-20241126".

El segundo paso fue modificar el bloque de código de la celda del primer paso para que mediante instrucciones se seleccionaran 5 columnas relevantes para el análisis y la visualización de datos. El bloque de código del segundo paso además contiene instrucciones que permiten guardar el dataframe con las columnas seleccionadas. Cuando el bloque de código de la celda del segundo paso se terminó de ejecutar se obtuvo un archivo con el nombre "selected columns.csv".

El tercer paso fue desarrollar líneas de código que permitieran imprimir una lista de los valores únicos ordenados alfabéticamente de la columna 'spatial_dim_es' que contiene los países considerados en el conjunto de datos de la Organización Panamericana de la Salud. El bloque de código del tercer paso pide al usuario que suba el archivo "selected columns.csv" para poder imprimir la lista. Con este bloque de código observamos que la Organización Panamericana de la Salud obtuvo datos de 49 países del continente americano.

El cuarto paso fue reemplazar el valor 'Bolivia (Estado Plurinacional de)' de la columna 'spatial_dim_es' por Bolivia para que el software Tableau Public pudiera considerar a este país en una visualización de mapa. Cuando el bloque de código de la celda del cuarto paso se terminó de ejecutar se obtuvo un archivo con el nombre "corrected data.csv".

El quinto paso fue determinar las instrucciones para ordenar alfabéticamente los valores únicos de la columna 'nombre_indicador' y contar cuántos valores únicos hay en esa columna.

El sexto paso fue determinar el identificador (id) de cada uno de los valores únicos (indicadores) de la columna "nombre_indicador".

El séptimo paso fue modificar el formato de los identificadores del paso anterior para no demorarse en la definición repetitiva y manual del formato de la selección de indicadores.

El octavo paso fue la definición de la lista de IDs de los indicadores seleccionados a importar en un archivo CSV.

Finalmente se ejecutó un bloque de código para comprobar que el archivo con el nombre "indicadores seleccionados.csv" incluyera los indicadores elegidos.

Conjunto de datos 2

El primer paso fue escribir un bloque de código dentro de una celda en un archivo de Google Colab denominado “Diabetes equipo-c24-10-n-data.ipynb”. El bloque de código correspondiente al primer paso contiene líneas de código para importar la librería pandas, numpy, matplotlib, seaborn y permitir utilizar archivos con una función que permite subir archivos CSV a Google Colab, se utilizó el método df.info() para obtener un resumen del archivo CSV que permite mostrar la cantidad de valores no nulos de cada columna y se usó un ciclo con instrucciones que permitir ver los valores únicos y la cantidad de valores únicos de cada columna. El archivo original que se utilizó al ejecutar el bloque de código escrito en la celda se llama "diabetes_dataset".

El segundo paso fue seleccionar las 5 columnas iniciales para el análisis y la visualización de datos.

El tercer paso fue generar una lista de las columnas. Tambien se establecio un bucle que permite contar el número de valores únicos de cada columna.

El cuarto paso consiste en el calculo de la cantidad de duplicados del DataFrame usando el método df.duplicated().sum().

No se determino condiciones adicionales necesarias para la lectura de los datos.


## ➡️Explicación adicional de los pasos de exploración, preparación y selección de los datos

El archivo original del conjunto de datos 1 contiene 327401 filas y el peso del archivo es de 125,631 KB. Los 8 pasos descritos anteriormente permitieron obtener un archivo con 225130 filas y un peso de 17621 KB. 

El archivo original del conjunto de datos 2 contiene 9538 filas y el peso del archivo es de 23.87 KB. Los 4 pasos descritos anteriormente permitieron determinar mantener la integridad del dataset original para el abordaje de este proyecto.

## ➡️Agrupación de indicadores

Hemos agrupado los 150 indicadores elegidos para que el dashboard interactivo en Tableau cuente con un número reducido de secciones.

Las secciones con sus respectivos indicadores se encuentran en el siguiente documento:


## 🚀Enlace para acceder al dashboard interactivo en Tableau Public:

*

## 🚀Enlace para acceder a las diapositivas de presentación del dashboard interactivo (Nombre del proyecto):

*

## 📌Los siguientes enlaces contienen información en inglés sobre los indicadores que se encuentran en los conjuntos de datos:

https://opendata.paho.org/en/core-indicators/technical-specifications

https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset
