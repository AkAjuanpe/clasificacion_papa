# clasificacion_papa
Codigo fuente de un modelo de clasificacion de cultivos basado en el sudeste de la provincia de Buenos Aires, Argentina. Desarrollado en Google Earth Engine, utilizando datos reales y un algoritmo de Random Forest para la clasificación.

En el codigo fuente "table 4" indica la region en la que se centra el proyecto, en este caso se utilizo un poligono que delimitaba ciertos partidos de la zona.

Por otro lado, "table 3" es el buffer de información sobre cultivos y diferentes superficies en la zona, solo la parte de entrenamiento, es decir, un 70%.
Este buffer presenta en la base de datos una columna que indica un codigo por cada tipo de cobertura que se queria identificar.
Este codigo fue el que distingio posteriormente las diferentes clases cuando se subio el archivo final a QGIS para poder analizarlo y evaluarlo.

En el codigo cuando se procesan las imagenes del Sentinel 2, hay una variable llamada "bandstoremove" donde se eliminan diferentes bandas de este satelite.
Esto no es necesario, ya que fueron eliminadas por alto contenido de nubes que daba error al momento de clasificar.
