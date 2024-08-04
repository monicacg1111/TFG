# TFG - Técnicas de Minería en bases de conocimiento
Repositorio dedicado a la realización de mi Trabajo de Fin de Grado en el Doble Grado de Ingeniería Informática y Matemáticas, titulado "**Técnicas de Minería en bases de conocimiento: Detección de *spam* en bases textuales mediante técnicas de aprendizaje supervisado**.

##  Resumen del proyecto

Este proyecto se centra en explorar técnicas tanto convencionales como no convencionales de Aprendizaje Automático. El objetivo es analizar el desempeño de los algoritmos de aprendizaje supervisado, junto con técnicas de Procesamiento del Lenguaje Natural, para combatir el problema de la detección de *spam*. 

El correo no deseado, comúnmente conocido como *spam*, constituye una forma de comunicación no solicitada que, normalmente está asociada al marketing y a la promoción de productos pero, a menudo, puede contener ofertas fraudulentas o intentos de phishing. Esta problemática se ha intensificado con la evolución de las tecnologías digitales, donde el envío masivo de correos electrónicos indeseados se realiza a un costo mínimo para los emisores, pero con consecuencias potencialmente severas para los receptores.

La memoria (`MemoriaTFG.pdf`) se divide en las siguientes secciones:

1. **Estudio del los conceptos de KDD (*Knowledge Discovery in Databases*) y del KDT (*Knowledge Discovery in Text*)**. Comparación de ambos enfoques y diferencias entre sus fases. Estudio de distintas técnicas de preprocesamiento y limpieza de datos, en su mayoría relacionadas con el Procesamiento del Lenguaje Natural. 

2. ***Spam***: estado del arte de las técnicas de filtrado de *spam*. 

3. **Fundamentos matemáticos**: por un lado, se ve el estudio de los fundamentos de la probabilidad, Teoría de grafos, redes bayesianas y las bases matemáticas del clasificador Naive Bayes. Por otro lado, se explican los fundamentos geométricos necesarios para comprender las Máquinas de Soporte Vectorial. 

4. **Experimentación**: se toman tres corpus de datos distintos, se realiza una visualización de los datos y se aplican distintas técnicas de preprocesado: *stemming*, lematización, eliminación de *stop words*, etc. A continuación, se aplican distintos clasificadores derivados de Naive Bayes y SVM y se comparan los resultados obtenidos. Además, se experimenta con nuevos enfoques relacionados con la Ingeniería de Conocimiento (uso de *synsets*).

   El lenguaje de programación utilizado fue Python y las bibliotecas empleadas incluyen `Pandas`, `Scikit-learn` y `NLTK`.

En el presente trabajo he tenido la oportunidad de desarrollar que a pesar de haber sido profundamente estudiado a lo largo de las últimas dos décadas, aún provoca grandes problemas a los usuarios. 

En particular, hemos conseguido confirmar la viabilidad de detectar correo electrónico basura mediante técnicas de Minería de Textos.  Por ejemplo, hemos visto que para cada categoría, el contenido de los textos es distinto. Los correos spam suelen contener palabras relacionadas con el marketing, las citas y las transacciones, mientras que en los correos ham aparecen términos más corporativos y académicos. 

A lo largo de la realización del proyecto, hemos encontrado distintas dificultades. Entre ellas, la extracción conocimiento a partir de texto en lenguaje natural no es un tarea trivial. A decir verdad, el texto no estructurado necesita de un tratamiento más preciso que por ejemplo los datos numéricos. Por ello hemos tenido que ajustar de forma muy concisa el preprocesamiento utilizado para no conseguir el efecto contrario y mermar la eficacia de los modelos entrenados. 

En cuanto a los resultados de la clasificación, destacamos el sobresaliente desempeño de
los algoritmos empleados. En general se han obtenido métricas de evaluación con valores
por encima del **95 %**, lo que indica una alta eficacia en la detección de spam. Ha resultado complicado hacer comparaciones detalladas entre los modelos, ya que todos exhiben un rendimiento casi inmejorable. No obstante, destacamos el buen desempeño del algoritmo **Naive Bayes Multinomial**, pues consigue entrenar un modelo mediante validación cruzada en apenas unos segundos, y sus resultados son tan buenos como los de otros modelos más lentos.

