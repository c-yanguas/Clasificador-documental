# Clasificador-documental
El objetivo de este proyecto es crear un clasificador documental automático a través de textos etiquetados. <br />

Se recomiendo la lectura de Clasificador-documental.pdf para comprender con detalle los objetivos que abarca el código propuesto, así como su utilización y estructuración. <br />

El proyecto se divide de la siguiente manera:
- La carpeta Documentos contiene 6 carpetas, 3 con textos en formato .docx y otras 3 con textos en formato .txt, divididos en las temáticas deportes salud y política. En caso de querer llevar a cabo otro preprocesado de datos para abordar el problema, se recomienda utilizar las carpetas _plano, ya que son las que contienen los .txt
- El notebook Transformacion_inicial contiene el preprocesado  realizado, es decir, el paso de docx a txt así como el preprocesado realizado a nivel texto. En caso de no querer hacer un preprocesado, se recomienda utilizar directamente datos.csv
- Después tenemos la carpeta glosario, la cual contiene un glosario por temática extraído de manera automática mediante los 100 elementos con  mayor TF-IDF asociado para cada temática. También existen otros 3 csv con _revisado, esto es debido a que la librería de preprocesado nltk utilizada, no cuenta con recursos tan potentes como los de habla inglesa, por lo que existían stopwords como 'dos' o 'día'.
- Finalmente nos encontramos con 5 carpetas referentes a los resultados de cada una de las 5 aproximaciones utilizadas, expuestas en cada uno de los 5 notebooks:
  - Modelo Naïve Bayes: Se utiliza para su entrenamiento los glosarios revisados
  - SVM: Tiene dos aproximaciones, con glosario y con SVD
  - Red neuronal: Se utiliza para su entrenamiento SVD
  - Random forest: Se utiliza para su entrenamiento SVD
