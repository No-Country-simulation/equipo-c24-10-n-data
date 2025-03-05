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

Brayan Córdova

## Nombre del proyecto:



## 📄Descripción del proyecto:



## 📖Conjuntos de datos utilizados:

Fuente 1: 

El conjunto de datos de la Organización Panamericana de la Salud (PAHO por sus siglas en inglés) fue descargado el día 3 de marzo de 2025, y su última actualización fue el día 14 de enero de 2025. El archivo original contiene 27 columnas, sin embargo, se ha decidido delimitar el análisis de datos a 5 columnas de datos y a 158 indicadores.

Fuente 2: 

El conjunto de datos de - fue descargado el día -, y su última actualización fue el día -. El archivo original contiene - columnas, sin embargo, se ha decidido delimitar el análisis de datos a - columnas de datos y a - indicadores.

## 📖Archivos CSV usados en Google Colab

El siguiente enlace permite descargar el archivo original que se utilizó en Google Colab:
*

## ➡️Descripción de los pasos de exploración, preparación y selección de los datos (etapa previa a la visualización de datos)

El primer paso fue escribir un bloque de código dentro de una celda en un archivo de Google Colab denominado “notebook”. El bloque de código correspondiente al primer paso contiene líneas de código para importar la librería pandas y permitir utilizar archivos, una función que permite subir archivos CSV a Google Colab, se utilizó el método df.info() para obtener un resumen del archivo CSV que permite mostrar la cantidad de valores no nulos de cada columna y se usó un ciclo con instrucciones que permitir ver los valores únicos y la cantidad de valores únicos de cada columna. El archivo original que se utilizó al ejecutar el bloque de código escrito en la celda se llama "PAHO-Core-Indicators-2024-20241126".

El segundo paso fue modificar el bloque de código de la celda del primer paso para que mediante instrucciones se seleccionaran 5 columnas relevantes para el análisis y la visualización de datos. El bloque de código del segundo paso además contiene instrucciones que permiten guardar el dataframe con las columnas seleccionadas. Cuando el bloque de código de la celda del segundo paso se terminó de ejecutar se obtuvo un archivo con el nombre "selected columns.csv".

El tercer paso fue desarrollar líneas de código que permitieran imprimir una lista de los valores únicos ordenados alfabéticamente de la columna 'spatial_dim_es' que contiene los países considerados en el conjunto de datos de la Organización Panamericana de la Salud. El bloque de código del tercer paso pide al usuario que suba el archivo "selected columns.csv" para poder imprimir la lista. Con este bloque de código observamos que la Organización Panamericana de la Salud obtuvo datos de 49 países del continente americano.

El cuarto paso fue reemplazar el valor 'Bolivia (Estado Plurinacional de)' de la columna 'spatial_dim_es' por Bolivia para que el software Tableau Public pudiera considerar a este país en una visualización de mapa. Cuando el bloque de código de la celda del cuarto paso se terminó de ejecutar se obtuvo un archivo con el nombre "corrected data.csv".

...

Finalmente se ejecutó un bloque de código para comprobar que el archivo con el nombre "indicadores seleccionados.csv" incluyera los indicadores elegidos.

## ➡️Explicación adicional de los pasos de exploración, preparación y selección de los datos

El archivo original contiene 327401 filas y el peso del archivo es de 125,631 KB. Los 8 pasos descritos anteriormente permitieron obtener un archivo con 225402 filas y un peso de 17650 KB. 

## ➡️Agrupación de indicadores

Hemos agrupado los 158 indicadores elegidos para que el dashboard interactivo en Tableau cuente con un número reducido de secciones.

Las secciones con sus respectivos indicadores se encuentran en el siguiente documento:


## 🚀Enlace para acceder al dashboard interactivo en Tableau Public:

*

## 🚀Enlace para acceder a las diapositivas de presentación del dashboard interactivo (Nombre del proyecto):

*

## 📌Los siguientes enlaces contienen información en inglés sobre los indicadores que se encuentran en los conjunto de datos:

https://opendata.paho.org/en/core-indicators/technical-specifications
