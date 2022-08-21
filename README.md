# Proyecto-Sharks-Adri
En este repositorio se irán añadiendo los archivos del proyecto de limpieza del DataFrame "Sharks"

--------------------------------------------------------------------------------------------------

Leemos el archivo

Exploramos el archivo. Observamos tipos de variables, nulos, cantidad de registros...

Corregimos los nombres de las columnas (espacios, carácteres especiales...)

Eliminamos duplicados (19441 duplicados)

Eliminamos filas con muchos nulos (solo 10 filas)

Corregimos valores nulos (observamos nulos por columna. Todos los valores "object" por "unknown")

Convertimos todos los valores a MAYÚSCULAS para evitar problemas.

Quitamos espacios iniciales y finales de todos los valores.

Seleccionamos columnas (variables) de interés (col_vip).

Creamos subset con esas columnas (¿duplicados? Solo 1, pero eliminamos)

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
