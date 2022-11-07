#  SHARKS DATA BASE 🦈 <br />
## CONTENIDO 📑
[1 - Objetivo 🎯](#O)<br />
[2 - Exploración 👀](#E) <br />
[3 - Correcciones Iniciales 🔧](#CI)<br />
[4 - Limpieza 🧼](#L)<br />
[5 - Análisis 📊](#A)<br />
[6 - Links y Recursos 💻](#LR)<br />

## OBJETIVO <a name="O"/> 
🧹 Limpiar la base de datos lo más minuciosamente posible con un deadline de 3 días.<br />

📊 Realizar un pequeño análisis de los datos.<br />

🔊 Exponer las conclusiones obtenidas.

## EXPLORACIÓN 👀 <a name="E"/> 
⤵️ Importamos y leemos el archivo.<br />

📅 Convertimos en dataframe.<br />

🔎 Observamos tipos de variables, nulos, cantidad de registros, valores extraños o inconsistentes, etc.

## CORRECCIONES INICIALES 🔧 <a name="CI"/> 
🪛 Corregimos los nombres de las columnas (espacios, carácteres especiales...)<br />

‼️ Eliminamos duplicados (19441 duplicados).<br />

⛔ Observamos columnas con muchos nulos -> No se nos permite eliminar columnas, pero eliminaríamos aquellas con +80% nulos.<br />

🚩 Eliminamos filas con muchos nulos (drop 10 filas). <br />

🔃 Corregimos valores nulos (observamos nulos por columna).<br />

🅰️ Convertimos todos los valores a MAYÚSCULAS para evitar problemas.<br />

🔘 Quitamos espacios iniciales y finales de todos los valores.<br />

🚨 Seleccionamos columnas (variables) de interés (col_vip).<br />

🔝 Creamos subset con esas columnas (¿duplicados? Solo 1, pero eliminamos).

## LIMPIEZA 🧼 <a name="L"/> 
🧹 Limpiamos las columnas importantes (Case_number [Fecha*], Type, Country, Area, Location, Activity, Sex, Age, Fatal(y/n), Species).<br />

🗓️ Renombramos "Case_Number" por "Fecha".<br />

🌍 Pasamos a "Unknown" los Países y las Áreas con pocos casos (ruido, aportación residual).<br />

🔙 Decidimos quitar "Location" de las columnas importantes (aportación residual).<br />

🔝 Creamos un nuevo subset con las columnas importantes.<br />

🗑️ Eliminamos filas con muchos valores "Unknown" (criterio >3, 1655 filas).<br />

🗑️ Eliminamos filas que supongan duplicados en el subset (49 filas).<br />

🗑️ Eliminamos datos anteriores al año 1900 por inconsistencia del dato (316 filas).<br />

⤴️ Exportamos a excel y analizamos.<br />

## ANÁLISIS 📊 <a name="A"/> 
🚻 Ataques por Sexo: 88/12 % (H/M).<br />

👧 Ataques por Edad: Top -> Jóvenes y peso relativo Niñas y Ancianas vs Hombres.<br />

🦈 Ataques por Especie: Top -> Tiburón Blanco.<br />

💀 Letalidad por Especie: Top -> Tiburón Blanco.<br />

🏄 Ataques por Actividad: Top -> Surf.<br />

🏊 Letalidad por Actividad: Top -> Nado.<br />

🗺️ Ataques por País: Top -> EEUU.<br />

📈 Letalidad por País: Top -> Australia.

## LINKS Y RECURSOS 💻 <a name="LR"/>
• https://www.kaggle.com/teajay/global-shark-attacks <br />
• https://numpy.org/doc/1.18/ <br />
• https://pandas.pydata.org/ <br />
• https://docs.python.org/3/library/functions.html <br />
• https://plotly.com/python/ <br />
• https://matplotlib.org/ <br />
• https://seaborn.pydata.org/ <br />
• https://pandas.pydata.org/docs/ <br />
• https://towardsdatascience.com/beware-of-storytelling-with-data-1710fea554b0?gi=537e0c10d89e
