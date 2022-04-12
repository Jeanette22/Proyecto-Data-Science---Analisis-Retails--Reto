# RETO: Proyecto final del reto de Data-Science - Caso: Analisis-Retails | Platzi
 
## ÍNDICE:
### Preguntas a responder: 
1) Preguntas del negocio: ¿Cuál es el promedio de ventas sin contar a la compañía dominante?
2) ¿Cuánto dinero en ventas generó la mayoría de las compañías?
3) ¿Cuántas tiendas tiene la mayoría de las compañías?
4) ¿La cantidad de tiendas está relacionada con la cantidad de ventas? Es decir, ¿si una empresa tiene más tiendas tendrá más dinero de ventas?
5) ¿Cuál es el rango que existe entre las ventas?
6) ¿Cuáles son las 5 empresas que más tiendas físicas tienen? ¿Cuáles de ellas están dentro de las 5 empresas que más ventas tuvieron?
7) ¿Qué categoría de compañía generó más ventas?
8) ¿Cuál es la compañía que en relación con su cantidad de tiendas físicas genera más ventas?
9) ¿Cuáles compañías venden de forma exclusivamente online? ¿Sus ventas destacan sobre las que también tienen tiendas físicas?
10) 10) ¿Cuáles son los outliers?

## Respuestas: 
### Análisis de los 25 retailers más grandes de Estados Unidos
- analisis de ventas, 
a) Usos de SLICES
- Promedio de ventas(media): interpretación
b) Ventas de las mayoria de las empresas: uso de la "mediana"
- gráfico con seaborn
c) Cantidad de tiendas de la mayoria de compañias: "mediana"
- gráfico con seaborn, para analizar detalles
d) Analisis de correlación entre cant de tiendas con sus ventas
- gráfico Scatter
e) Analisis del rango entre ventas: uso de formula
f) Analisis de las empresas con mas tiendas fisicas
- uso de señalador de colores con formato de Pandas
g) Analisis de las categoria con más ventas
- pandas: degrade de colores
h) Analisis de la Compañia en relacion a sus tiendas fisicas, con mas ventas.
- Grafico de barras
i) Analsis de empresas online y fisicas
j) Analisis de OUTLIERS 

### Cuestiones técnicas:
- Utilicé DeepNote
Python 3.7:
![image](https://user-images.githubusercontent.com/80054717/162942946-2481d33d-bb22-4a2d-8ce0-b1358b8df41f.png)

- Pandas
- Numpy
- Matplotlib.pyplot
- Seaborn

### Teoría y análisis estadísticos:
Durante el desarrollo de este proyecto apliqué la teória y prácticas sobre estadisticas vista durante el DataCamp y en cursos de la Ruta Data Science, bajo los siguientes conceptos: 
- Distribución de los datos:  
Discreta: cuando no puede tomar ningún valor entre dos consecutivos. 
Continua: cuando puede tomar cualquier valor dentro de un intervalo 
En este caso en el proyecto se pueden visualizar en las gráficas con ventas / ingresos de empresas superiores a otras, dónde utilicé graficos de barra, dónde a simple vista puede notarse las diferencias, y señalar su promedio. 

### MEDIDAS DE TENDENCIA CENTRAL
"no se puede predecir el comportamiento individual pero si el comportamiento promedio!"
La medida de tendencia central se usa para situar el que lugar esta el elemento promedio/ tipico del grupo. 
Un ejemplo desde este proyecto fue el analsis del promedio (media) y la mediana
- media (promedio): noción de centralidad de los datos, ubicación de ese conj de datos, es resumida
- ![image](https://user-images.githubusercontent.com/80054717/160477809-1c02862e-e03a-495f-b63e-9804a0d62927.png)

(es el valor promedio de un conjunto de datos numéricos, calculada como la suma del conjunto de valores dividida entre el número total de valores.)
- mediana (dato central) dato que está en la mitad, valor caracterizado, balanceado justo en la mitad, 
(es un estadístico de posición central que parte la distribución en dos, es decir, deja la misma cantidad de valores a un lado que a otro.)
- moda (dato que más se repite): el dato que más se repite, o valor de la variable que más se repite
- 
- Estas medidas tambien sirven para realizar comparaciones, e interpretar resultados: Ejemple; Analsis de retails y su cantidad de tiendas
- El uso de una misma variable para diferentes ocasiones, por ejemplo en casos donde el valor promedio no sea representativo y utilizamos la mediana. 
- permite comparar resultados entre grupos, usando la media 


Acotación: en la pregunta numero dos, justifico el uso de "la mediana" debido a que tenemos datos sesgados, esto porque si utilizamos todo el dataset 
hay una gran diferencia respecto a WallMart y eso afecta a todos los resultados, por eso para responder ¿Cuánto dinero en ventas generó la mayoría de las compañías? y en la siguiente pregunte, dado a que en ambas se solicitaba "la mayoria de..." y consideré que era mas próximo a datos reales este tipo de medida. 
Cualquier tipo de sugerencia es bienvenida! :)

### Otras medidas de tendencia central: 
- rango: distancia que abarca la distancia del valor min al max de un conj de datos 
- rango intercuartil: es la distancia entre cuartil q1 al q2 //cuartiles: define en cuatro subdivision homogenea,:// diagrama de caja, podemos verlo aca
- desviación estándar: La desviación estándar es la medida de dispersión más común, que indica qué tan dispersos están los datos con respecto a la media. Mientras mayor sea la desviación estándar, mayor será la dispersión de los datos.
- En estos último casos utilicé gráficos Scatter donde puede analizar la correlacion de variables, e interpretar los resultados para responder las preguntas solciitadas

### Por último sume un analisis de los quartiles 

Cuartil	Descripción
- 1er cuartil (Q1)	25% de los datos es menor que o igual a este valor.
- 2do cuartil (Q2)	La mediana. 50% de los datos es menor que o igual a este valor.
- 3er cuartil (Q3)	75% de los datos es menor que o igual a este valor.
- Rango intercuartil	La distancia entre el primer 1er cuartil y el 3er cuartil (Q3-Q1); de esta manera, abarca el 50% central de los datos.

### Para analizar dispersión y tendencia central, usando el diagrama de caja como vimos en clases.
