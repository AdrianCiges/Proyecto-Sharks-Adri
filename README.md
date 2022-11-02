#  SHARKS DATA BASE 🦈 <br />
En este repositorio se encuentran los archivos utilizados y creados para el proyecto de limpieza de la base de datos de "Global Shark Attack" de la semana 2 del bootcamp de análisis de datos de IronHack (Madrid).<br />
URL: https://www.kaggle.com/datasets/teajay/global-shark-attacks

## Objetivo
🧹 Limpiar la base de datos lo más minuciosamente posible con un deadline de 3 días.<br />
📊 Realizar un pequeño análisis de los datos.<br />
🔊 Exponer las conclusiones obtenidas.

## Exploración 👀
⤵️ Importamos y leemos el archivo.<br />
📅 Convertimos en dataframe.<br />
🔎 Observamos tipos de variables, nulos, cantidad de registros, valores extraños o inconsistentes, etc.

## Correcciones iniciales 🔧
🪛 Corregimos los nombres de las columnas (espacios, carácteres especiales...)<br />
‼️ Eliminamos duplicados (19441 duplicados).<br />
⛔ Observamos columnas con muchos nulos -> No se nos permite eliminar columnas, pero eliminaríamos aquellas con +80% nulos.<br />
🚩 Eliminamos filas con muchos nulos (drop 10 filas). <br />
🔃 Corregimos valores nulos (observamos nulos por columna).<br />
🅰️ Convertimos todos los valores a MAYÚSCULAS para evitar problemas.<br />
🔘 Quitamos espacios iniciales y finales de todos los valores.<br />
🚨 Seleccionamos columnas (variables) de interés (col_vip).<br />
🔝 Creamos subset con esas columnas (¿duplicados? Solo 1, pero eliminamos).

## Limpieza 🧼
🧹 Limpiamos las columnas importantes (Case_number [Fecha*], Type, Country, Area, Location, Activity, Sex, Age, Fatal(y/n), Species).<br />
🗓️ Renombramos "Case_Number" por "Fecha".<br />
🌍 Pasamos a "Unknown" los Países y las Áreas con pocos casos (ruido, aportación residual).<br />
🔙 Decidimos quitar "Location" de las columnas importantes (aportación residual).<br />
🔝 Creamos un nuevo subset con las columnas importantes.<br />
🗑️ Eliminamos filas con muchos valores "Unknown" (criterio >3, 1655 filas).<br />
🗑️ Eliminamos filas que supongan duplicados en el subset (49 filas).<br />
🗑️ Eliminamos datos anteriores al año 1900 por inconsistencia del dato (316 filas).<br />
⤴️ Exportamos a excel y analizamos.<br />

## Análisis 📊
🚻 Ataques por Sexo: 88/12 % (H/M).<br />
👧 Ataques por Edad: Top -> Jóvenes y peso relativo Niñas y Ancianas vs Hombres.<br />
🦈 Ataques por Especie: Top -> Tiburón Blanco.<br />
💀 Letalidad por Especie: Top -> Tiburón Blanco.<br />
🏄 Ataques por Actividad: Top -> Surfeo.<br />
🏊 Letalidad por Actividad: Top -> Nado.<br />
🗺️ Ataques por País: Top -> EEUU.<br />
📈 Letalidad por País: Top -> Australia.
