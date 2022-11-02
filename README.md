# Proyecto-Sharks-Adri 🦈 <br />
## 👀 Exploración
• Importamos y leemos el archivo.<br />
• Convertimos en dataframe.<br />
• Observamos tipos de variables, nulos, cantidad de registros, valores extraños o inconsistentes, etc.

## 🔧 Correcciones iniciales
• Corregimos los nombres de las columnas (espacios, carácteres especiales...)<br />
• Eliminamos duplicados (19441 duplicados)<br />
• Eliminamos filas con muchos nulos (drop 10 filas)<br />
• Corregimos valores nulos (observamos nulos por columna)<br />
• Corregimos los valores "object" por "unknown")<br />
• Convertimos todos los valores a MAYÚSCULAS para evitar problemas.<br />
• Quitamos espacios iniciales y finales de todos los valores.<br />
• Seleccionamos columnas (variables) de interés (col_vip).<br />
• Creamos subset con esas columnas (¿duplicados? Solo 1, pero eliminamos)

Limpiamos las columnas importantes (Case_number [Fecha*], Type, Country, Area, Location, Activity, Sex, Age, Fatal(y/n), Species).

Renombramos "Case_Number" por "Fecha".

Pasamos a "Unknown" los paises con pocos casos (ruido, aportación residual).

Hacemos lo mismo con el "Area".

Decidimos quitar "Location" de las columnas importantes (aportación residual).

Creamos un nuevo subset con las columnas importantes.

Eliminamos filas con muchos valores "Unknown" (criterio >3, 1655 filas).

Eliminamos filas que supongan duplicados en el subset (49 filas).

Eliminamos datos anteriores al año 1900 por inconsistencia del dato (316 filas).

Exportamos a excel y analizamos. 
