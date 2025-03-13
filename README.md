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

Los datos externos juegan un papel esencial al identificar tendencias internacionales, segmentar poblaciones según factores demográficos y analizar la demanda de servicios y recursos. De esta forma, las instituciones de salud pueden anticiparse a las necesidades de los pacientes y optimizar sus procesos. Este proyecto se basa en el conjunto de datos:de la Organización Panamericana de la Salud.

## 📖Conjunto de datos utilizado:

El conjunto de datos de la Organización Panamericana de la Salud (PAHO por sus siglas en inglés) fue descargado el día 3 de marzo de 2025, y su última actualización fue el día 14 de enero de 2025. El archivo original contiene 27 columnas, sin embargo, se ha decidido delimitar el análisis de datos a 5 columnas de datos y a 150 indicadores.

## 📖Archivo CSV usado en Google Colab

El siguiente enlace permite descargar el archivo original utilizado en Google Colab:

https://drive.google.com/file/d/1FeNg3pMyvOutFTSC6rJP3czoCFm_qPIo/view?usp=sharing

## ➡️Descripción de los pasos de exploración, preparación y selección de los datos (etapa previa a la visualización de datos)

El primer paso fue escribir un bloque de código dentro de una celda en un archivo de Google Colab denominado “notebook”. El bloque de código correspondiente al primer paso contiene líneas de código para importar la librería pandas y permitir utilizar archivos, una función que permite subir archivos CSV a Google Colab, se utilizó el método df.info() para obtener un resumen del archivo CSV que permite mostrar la cantidad de valores no nulos de cada columna y se usó un ciclo con instrucciones que permitir ver los valores únicos y la cantidad de valores únicos de cada columna. El archivo original que se utilizó al ejecutar el bloque de código escrito en la celda se llama "PAHO-Core-Indicators-2024-20241126".

El segundo paso fue modificar el bloque de código de la celda del primer paso para que mediante instrucciones se seleccionaran 5 columnas relevantes para el análisis y la visualización de datos. El bloque de código del segundo paso además contiene instrucciones que permiten guardar el dataframe con las columnas seleccionadas. Cuando el bloque de código de la celda del segundo paso se terminó de ejecutar se obtuvo un archivo con el nombre "selected columns.csv".

El tercer paso fue desarrollar líneas de código que permitieran imprimir una lista de los valores únicos ordenados alfabéticamente de la columna 'spatial_dim_es' que contiene los países considerados en el conjunto de datos de la Organización Panamericana de la Salud. El bloque de código del tercer paso pide al usuario que suba el archivo "selected columns.csv" para poder imprimir la lista. Con este bloque de código observamos que la Organización Panamericana de la Salud obtuvo datos de 49 países del continente americano.

El cuarto paso fue reemplazar el valor 'Bolivia (Estado Plurinacional de)' de la columna 'spatial_dim_es' por Bolivia para que el software Tableau Public pudiera considerar a este país en una visualización de mapa. Cuando el bloque de código de la celda del cuarto paso se terminó de ejecutar se obtuvo un archivo con el nombre "corrected data.csv".

El quinto paso fue determinar las instrucciones para ordenar alfabéticamente los valores únicos de la columna 'nombre_indicador' y contar cuántos valores únicos hay en esa columna.

El sexto paso fue determinar el identificador (id) de cada uno de los valores únicos (indicadores) de la columna "nombre_indicador".

El séptimo paso fue modificar el formato de los identificadores del paso anterior para no demorarse en la definición repetitiva y manual del formato de la selección de indicadores.

El octavo paso fue la definición de la lista de IDs de los indicadores seleccionados a importar en un archivo CSV.

Finalmente se ejecutó un bloque de código para comprobar que el archivo con el nombre "indicadores seleccionados.csv" incluyera los indicadores elegidos.

## ➡️Explicación adicional de los pasos de exploración, preparación y selección de los datos

El archivo original del conjunto de datos contiene 327401 filas y el peso del archivo es de 125,631 KB. Los 8 pasos descritos anteriormente permitieron obtener un archivo con 225130 filas y un peso de 17621 KB. 

## ➡️Agrupación de indicadores

Hemos agrupado los 150 indicadores elegidos para que el dashboard interactivo en Tableau cuente con un número reducido de secciones.

Las secciones con sus respectivos indicadores se encuentran en el siguiente documento:
https://drive.google.com/file/d/1GQHTs_nRKksucmf07-p07jirAVuNjzzF/view?usp=sharing 

## 🚀Enlace para acceder al dashboard interactivo en Tableau Public:

*

## 🚀Enlace para acceder a las diapositivas de presentación del dashboard interactivo (ENTCO):

https://www.canva.com/design/DAGhjhhYrSo/7LJwIoqBtxRckQ4iI_0v-Q/view?utm_content=DAGhjhhYrSo&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=ha60e1d9b8f

## 📌El siguiente enlace contienen información en inglés sobre los indicadores que se encuentran en el conjunto de datos:

https://opendata.paho.org/en/core-indicators/technical-specifications
