# PostulacionDatalized
Repositorio para los pedidos de postulacion de Datalized

------------------------------------------------------------------------------------------------------------------------

Se pide responder lo siguiente:
1- La pregunta que busca responder el panel
2- Las fuentes de datos utilizadas
3- El proceso de limpieza y transformación de los datos
4- Las decisiones de diseño del panel

------------------------------------------------------------------------------------------------------------------------

1- La pregunta que busca responder el panel:
La preguntan que busca responder el panel es que paises han tenido una mejoría o un empeoramiento entre los años 2010 y 2015,
se realizo a través de un .csv de explotación laboral infantil, en donde se mostraban varios paises con sus porcentajes y cantidades
por año, solo algunos paises poseían datos sólidos de 3 o más años, la mayoría mostraba 1 año como máximo.

Se puede observar en el panel que solo 1 país mejoró de forma radical sus numeros de explotación infantil, siendo este méxico
Paises como Malawi ha ido de mal en peor, aumentando cada año más el numero de explotación infantil
Brasil logró bajar sus numeros de explotación infantil desde 2011 hasta 2015, con una recaída en el aumento en 2014, pero en 2015 lograron un numero menor a que en 2011

------------------------------------------------------------------------------------------------------------------------

2- Fuente de datos utlizada:
Data set proveniente de kaggle:
https://www.kaggle.com/datasets

Fue usado principalmente el de estadísticas de explotación infantil:
https://www.kaggle.com/datasets/shaistashahid/child-labor-statistics?resource=download

------------------------------------------------------------------------------------------------------------------------

3- El proceso de limpieza y transformación de los datos:

Primero se realizo un poco de estudio de los datos con distintos paneles: 
Total por pais en mapa mundi (por año, especificamente 2011,2014,2015) 
Se realizó un gráfico de orden de explotacion infantil de los paises de mayor a menor (por año, especificamente 2013,2014,2015) 

Para la pregunta que se intenta resolver:
Se graficó la mejoría o el empeoramiento de paises que tengan data de 3 años o más (la mayoria poseia 1 año y algunos pocos 2 años)
Del total de paises se obtuvieron solo 4 paises que tuvieran 3 años o más de data de cuantos millones de niños eran explotados

Para el panel que busca responder la pregunta:
Ignorar si es niño o niña y solo considerar el total, ya que el csv de datos lo separa en niño, niña, masculino, femenino
Para el panel final se filtraron distintos elementos ya que Tableau consideraba en algunas ocasiones el pais como región/continente (Latin America and Caribbean, Asia and the Pacific, Middle East and North Africa, entre otros), por lo tanto se separaron en un nuevo campo eliminar 
Se aplicó un script de COUNTD([Año]) > 3 para que solo se consideraran paises que tengan 3 años o más de data
Se filtraron los campos de años para considerar desde el 2010 - 2015

------------------------------------------------------------------------------------------------------------------------
4- Las decisiones de diseño del panel
Se realizaron distintas pruebas hasta que saliera el más adecuado para representar los datos
