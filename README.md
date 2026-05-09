# Proyecto_dashboard
# Conjunto de datos sobre productividad y comportamiento estudiantil

##  :star2: 1.	Contexto

    En la era digital actual, el rendimiento académico de los estudiantes se ve influenciado no solo por sus hábitos de estudio, sino también por su comportamiento digital y sus estilos de vida. El mayor uso de teléfonos inteligentes, la interacción en redes sociales, los videojuegos y las notificaciones constantes pueden afectar significativamente la concentración y la productividad. Asimismo, factores como la duración del sueño, los niveles de estrés y la actividad física también influyen en los resultados académicos generales. Este conjunto de datos se ha desarrollado para examinar la relación entre los patrones de comportamiento de los estudiantes, las distracciones digitales y el rendimiento académico, proporcionando información valiosa para investigadores, educadores y analistas de datos.
## :question:2.	Planteamiento del problema

Los estudiantes están cada vez más expuestos a distracciones digitales como los teléfonos inteligentes y las redes sociales.
El tiempo excesivo frente a las pantallas puede afectar negativamente la concentración y la productividad académica.
Los malos hábitos de sueño pueden reducir el rendimiento cognitivo y la eficacia del aprendizaje.
Los altos niveles de estrés pueden afectar el rendimiento académico y el bienestar general.
Las rutinas de estudio irregulares pueden provocar un rendimiento académico inconsistente.
La inactividad física puede influir en la agudeza mental y los niveles de concentración.
La falta de gestión del tiempo puede reducir los índices de finalización de las tareas.
El impacto combinado del estilo de vida y el comportamiento digital en las calificaciones no está claramente cuantificado.

## :dart:3. Objetivo
El objetivo es realizar un análisis basado en los datos, con la finalidad de desarrollar estrategias que mejoren los resultados de los estudiantes. Es necesario identificar los factores conductuales clave que influyen significativamente en la productividad de los estudiantes. Aunque predecir el rendimiento académico utilizando indicadores de comportamiento sigue siendo un reto.

## :building_construction:4.	Estructura del proyecto

### ├── Datos
>>>├──student_productivity_distraction_dataset_originales.csv

>>>├──student_productivity_distraction_transformados.csv

### ├── Archivos_análisis

>>>├── Exploración_transformación de datos.xlsx

>>>├── Análisis_datos.xlsx

>>>├── Dashboard.xlsx

### ├── README.md


## :label:5.	Atributos del conjunto de datos
El conjunto de datos de productividad y comportamiento estudiantil contiene 20000 registros estructurados de estudiantes que recopilan información en 18 columnas.

### Datos de los Estudiantes (3 columnas)
>➤ ID_estudiante: Identificador único asignado a cada estudiante

>➤ Edad: Edad del estudiante (en años)

>➤ Género: Género del estudiante      

### Hábitos de estudio y bienestar (5 columnas)
>➤ horas_estudio_día: Promedio de horas dedicadas al estudio por día

>➤ horas_sueño: Promedio de horas dormidas por noche

>➤ horas_descanso_día: Promedio de horas dedicadas al descanso por día

>➤ g_ingesta_café: Cantidad de café consumido por día

>➤ horas_ejercicio: Promedio de horas de actividad física que realiza

### Patrones de uso digital (4 columnas)
>➤ horas_uso_smartphone: Uso promedio diario del teléfono inteligente

>➤ horas_redes_sociales: Tiempo diario dedicado a las plataformas de redes sociales.

>➤ horas_youtube: Tiempo promedio diario dedicado a youtube

>➤ horas_videojuego: Tiempo promedio diario dedicado a jugar videojuegos

### Métricas de productividad y resultados académicos (6 columnas)
>➤ tareas_completadas: Cantidad de tareas completadas a tiempo

>➤ porcentaje_asistencia: Porcentaje de clases a las que se asiste

>➤ nivel_stress: Medido en un rango del 1 al 10

>➤ puntuación_enfoque: Puntuación del nivel de concentración medido

>➤ calificación_final: Calificación académica final obtenida

>➤ puntuación_productividad: Puntuación de rendimiento de productividad calculada

## :footprints: 6.	Pasos del proyecto
### Paso :one:
* Se crea repositorio con nombre “Proyecto_dashboard”.
* Se crea sistema de carpetas del repositorio
* Se añade archivo de datos originales “student_productivity_distraction_dataset_originales.csv”
### Paso :two:
* Para realizar la exploración de datos, se crea el primer Excel “Exploración_Transformación de datos.xlsx”.
* En excel creado se importan datos originales.
* Se crea nueva hoja “Datos_transformados” para generar tabla con copia de los datos originales.
* Se crea “Hoja_auxiliar” donde se realiza el conteo de filas, columnas y el conteo de datos en blanco en todas las categorías.
* Se traduce al español los encabezados de todas las columnas.
* Se genera nueva columna y se traduce al español las categorías de la columna “género”.
* Se genera nueva columna y se convierte valores de “mg_ingesta_café” a “g_ingesta_café”.
* Se genera nueva columna y se convierte valores de “minutos_ejercicio” a “horas_ejercicio”.
* Se ocultan columnas que fueron transformadas.
* Se genera y añade a repositorio el archivo de datos transformados “student_productivity_distraction_transformados.csv”
* Se añade a repositorio el archivo excel “Exploración_Transformación de datos.xlsx”.

### Paso :three:
* Se crea nuevo Excel para análisis de los datos “Análisis_datos.xlsx”.
* Se importa archivo csv de datos transformados “student_productivity_distraction_transformados.csv”.
* Se eliminan las columnas que fueron transformadas y no se usarán en análisis.
* Se inicia análisis categórico . Se identifica una sola columna categórica “género”.
* Se inicia análisis estadístico de todas las columnas numéricas.
* Se realiza un gráfico de correlación con las variables numéricas y con formato de escala de color identificamos cuáles son las variables fuertemente relacionadas.
* Se realiza el análisis binario tomando como variable de referencia “puntuación _productividad”.
* Se añade a repositorio el archivo excel “Análisis_datos.xlsx”.
### Paso :four:
* Se crea nuevo Excel “Dashboard.xlsx”.
* Se cargan los datos *.csv transformados.
* Se generan las tablas y gráficos a incluir en dashboard, siendo la variable de referencia “puntuación_productividad”.
* Se concluye con la elaboración de Dashboard en nueva hoja.
* Se añade a repositorio el archivo excel “Dashboard.xlsx”.

## :bulb:7.	Resultados y Conclusiones
### :white_check_mark: Conclusión General
El análisis realizado demuestra que la productividad no depende de un solo factor, sino de una interacción compleja entre hábitos de bienestar físico y hábitos académicos. 
Se concluye que una mayor puntuación de productividad está fuertemente correlacionada con un estilo de vida balanceado (sueño y bajo estrés) y una alta autodisciplina (estudio, enfoque y asistencia); mientras que la tecnología no bien gestionada (uso de Smartphone) es la de mayor impacto negativo en los resultados. 

### :white_check_mark: Conclusiones Específicas (Variables Positivas)
#### * Sueño y Estudio:
Se observó que un aumento en las horas de sueño y estudio potencian significativamente la productividad, sugiriendo que el descanso adecuado y la preparación técnica son pilares fundamentales.

#### * Asistencia y Enfoque: 
El alto porcentaje de asistencia, combinado con una mayor puntuación de enfoque, indica que la presencia activa y la atención sostenida son determinantes clave para maximizar los resultados

### :white_check_mark: Conclusiones Específicas (Variables Negativas)

#### * Uso de Smartphone: 
Se identificó una relación inversa clara: a mayor uso de smartphone, menor es la productividad, lo que probablemente se deba a la distracción y la fragmentación del tiempo.
#### * Nivel de Stress: 
El análisis confirma que el estrés alto actúa como un limitador directo de la productividad, lo que indica que el bienestar mental es esencial para el desempeño académico de los estudiantes.

## :loudspeaker:8.	Recomendaciones
Para neutralizar las variables negativas y potenciar las positivas, se podrían tener en cuenta las siguientes recomendaciones:
* Establecer zonas libres de dispositivos donde el smartphone permanezca fuera del alcance visual para reducir la carga cognitiva y la fragmentación de la atención.
* Establecer técnicas de priorización al estudiar (diferenciando lo urgente de lo importante) para evitar los picos de stress que afectan la productividad.
* Mantener una regularidad en las horas de sueño y horas de descanso, asumiendo que es una fase de recuperación necesaria para mantener la atención al día siguiente.
* Aplicar técnicas de gestión de la energía; es decir alternar bloques de tiempo de alta intensidad en el estudio, con tiempos de descansos breves, evitando el agotamiento y manteniendo el enfoque en niveles óptimos

## :writing_hand:9.	Autor
>>Martha Vergara
