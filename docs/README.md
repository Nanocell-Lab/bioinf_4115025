# Bioinformatica y Estructura Macromolecular - 4115025
- **Profesor: Dr. Alexis Salas B.**
- **Mágister de Bioquímica y Bioinformática**
- **Universidad de Concepción - Chile**

# Instrucciones Iniciación
*Se recomienda encarecidamente instalar linux en su computador, para esto se puede instalar una versión de linux, realizar una partición (se requiere buen computador i7), habilitar la terminal linux en Mac o en Windows (sólo en 10). Esto lo veremos en la [primera clase](Linux.md/#Linux)*.

Este repositorio puede ser clonado en su computador con:
git clone https://github.com/labnanocell/bioinf_4115025.git
[¿Cómo instalar GIT en mi computador?](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalaci%C3%B3n-de-Git)


Las clases presenciales comenzarán el Miércoles 15 de Abril en la plataforma CANVAS de la UdeC.

# Syllabus

## Descripción del curso
Curso Teórico-Práctico que incorpora las competencias requeridas para poder realizar análisis bioinformáticos de datos experimentales desde: 

* Base de trabajo en entornos linux.
* Programación en lenguaje python.
* Análisis de secuencias biológicas. 
* Análisis de estructural bioinformático.

Los datos de origen biológico provenientes desde secuencias de ácidos nucleicos y proteínas son analizados por metodologías de la biología computacional con aplicaciones en bioquímica, biología molecular, ingeniería de proteínas y biotecnología. Las actividades semanales son programadas con una revisión bibliográfica desde revistas bioinformáticas y los talleres son realizados en la plataforma Jupyter con python para reforzar las habilidades de pensamiento crítico y de programación computacional, respectivamente.

Esta asignatura aporta a las siguientes competencias del perfil de egreso del Magíster en Bioquímica y Bioinformática:

1. Analizar y seleccionar en forma crítica información proveniente de fuentes diversas y validadas para fundamentar la investigación y formular argumentos sólidos que permitan tomar decisiones. 
2.	Comunicar resultados y hallazgos de la investigación, mediante el manejo responsable de la información en sus diferentes modalidades, ya sea en forma oral, escrita o a través de los medios y tecnologías de la información y comunicación.

## Motivación del Curriculum a Desarrollar
[Bioinformática](https://es.wikipedia.org/wiki/Bioinform%C3%A1tica) es la aplicación de tecnologías computacionales y la estadística a la gestión y análisis de datos biológicos. 

* 10 años de experiencia de encargado de curso.
* [A Quick Guide for Developing Effective Bioinformatics Programming Skills](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000589)
* [An Online Bioinformatics Curriculum](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1002632)
* [Bioinformatics core competencies for undergraduate life sciences education](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0196878)

## Competencias Generales.
1.	Amplio conocimiento de temas relacionados con la biología. No hace falta ser un experto en biología, pero sí es necesario saber qué tipo de información que se está trabajando. Es especialmente útil saber acerca de la biología molecular, celular y genética.
2.	Competencias de comunicación. Un bioinformático debe ser capaz de comunicar información compleja a profesionales con una formación  en el área de las biología o la informática. Esta incluye una excelente redacción y documentación del trabajo realizado. 
3.	Competencias de trabajo en equipo. Un bioinformático no puede trabajar independientemente, buenos trabajos necesitan de varios profesionales y aproximaciones interdisciplinarias.
4.	Competencia de trabajo bajo presión y con múltiples tareas. Esto puede ser un trabajo de alta presión con plazos que han de cumplirse. Debe poseer una alta capacidad de organización, planificación  y de asignación de prioridades.
5.	Competente en un lenguaje de programación. El comprender la lógica e implementación de algoritmos permitirá desarrollar pequeños códigos (scripts) que permitan optimizar o realizar nuevas tareas eficientemente.

## Resultados de Aprendizaje

1. Ejecución y monitoreo de trabajos en forma local y remota en entornos de terminal de sistemas operativos linux o analogos.
2. Programar código computacional en lenguaje de programación Python.
3. Analizar datos desde secuencias de nucleotidos y proteínas obtenidas desde bases de datos o experimentos, alinear secuencias, realizar análisis de conservación, reconstrucción de filogenia, identificación de patrones y diseñor de partidores.
4. Reaizar análisis de estructuras de proteínas desde la visualización hasta complejas simulaciones de dinámica molecular para establecer las relaciones estructura función.
5. Comunicar resultados de investigaciones relacionadas a la bioinformática.
Investigar un mecanismo molecular con herramientas bioinformáticas.

## Tipos de Actividades
* [Planificación de Contenido.](#curriculum) Entrega de contenidos en clases sincrónicas y asincrónicas con documento de lecturas que se irán revisando en reuniones sincrónicas los miércoles de 10:00 a 13:00 hrs.
* [Investigar y Analizar.](Journal.md) Presentación de artículos científicos desde un Journal asignado cada semana.
* [Proyecto.](Project.md) Se desarrollará un proyecto en el curso que será diseñado para tributar en un objetivo bioinformático de su tesis de magister.

## Curriculum

Este es el contenido que iremos revisando en el curso, donde se trabajará en un contexto general y revisión de 15-20 minutos por concepto con 30 minutos de una actividad. 

- [Mes 1: Entorno de Sistema Operativo](Linux.md#entorno-de-sistema-operativo)
  * [Linux.](Linux.md#linux)
  * [SSH.](Linux.md#ssh)
  * [Computación de alto rendimiento.](Linux.md#computaci-n-de-alto-rendimiento)
  * [Extras [Opcional]](Linux.md#extras--opcional-)
- [Mes 2: Programando en Python](Python.md#Programando-en-Python)
  * [Python-Conda-Jupyter.](Python.md#python-conda-jupyter)
  * [Variables](Python.md#variables)
  * [Contenedores](Python.md#contenedores)
  * [Controles de Flujo](Python.md#controles-de-flujo)
  * [Funciones](Python.md#funciones)
  * [Extras [Opcional]](Python.md#extras)
- [Mes 3: Análisis de Secuencias Biológicas](Sequences.md#An-lsis-de-Secuencias-Biol-gicas)
  * [Módulos Python Bioinformáticos](Sequences.md#m-dulos-python-bioinform-ticos)
  * [Descripción de secuencias](Sequences.md#descripci-n-de-secuencias)
  * [Evolución Similaridad](Sequences.md#evoluci-n-similaridad)
  * [Alineamiento](Sequences.md#alineamiento)
  * [Filogenia Molecular](Sequences.md#filogenia-molecular)
  * [Diseño de partidores](Sequences.md#dise-o-de-partidores)
  * [Extras [Opcional]](Sequences.md#extras)
- [Mes 4: Análisis de Estructura de Proteínas](Structures.md#estructura)
  * [PDB.](Structures.md#pdb)
  * [Modelling.](Structures.md#modelling)
  * [Docking.](Structures.md#docking)
  * [Dinámica Molecular.](Structures.md#din-mica-molecular)
  * [Extras.](Structures.md#extras)

## Modalidad de Clases Online
Las clase serán online (Escenario Pandemia Covid-19), para ello se utilizará la plataforma [Canvas](https://www.instructure.com/canvas/es), [Microsoft Team](https://www.microsoft.com/es-es/education/products/teams) y [Github](https://github.com/). Las presentaciones de evaluación de los artículos serán a través de estas plataformas.

## Actividades de Evaluación
* Presentación de búsqueda bibliográfica/seminario semanal (25%): Dado un journal específico cada estudiante deberá enviar un día antes del miércoles un resumen del artículo seleccionado de una hoja y una presentación de 4-6 diapositivas. Un estudiante por clase presentará en forma aleatoria.
* Presentación de las tareas (25%): Las tareas de los talleres serán revisadas por los alumnos ayudantes, el promedio de todos estos trabajos será esta nota.
* Proyecto integrador (30%): Este proyecto deberá desarrollarse durante el semestre e incluye una presentación de 20 minutos de un tema y la aplicación de un *script* en Python. El escrito ponderará un 10%, el script 10%, y la presentación un 10%
* Prueba final de conocimientos (20%): Examen electrónico de la asignatura.

## Bibliografía Recomendada
*	Antao, Tiago. Bioinformatics with Python Cookbook: Learn How to Use Modern Python Bioinformatics Libraries and Applications to Do Cutting-Edge Research in Computational Biology, 2nd Edition. Edición: 2. Packt Publishing, 2018. ISBN-13: 978-1789344691. [Google Book](https://books.google.cl/books?id=ii59DwAAQBAJ&printsec=frontcover) | [Amazon Book](https://www.amazon.com/-/es/Tiago-Antao-ebook/dp/B07FNYFS9V) | [Github](https://github.com/PacktPublishing/Bioinformatics-with-Python-Cookbook-Second-Edition) 
*	Bessant, Conrad, Darren Oakley, and Ian Shadforth. Building Bioinformatics Solutions 2nd Edition. Edición: 2. Oxford, United Kingdom ; New York, NY, United States of America: Oxford University Press, 2014. ISBN-13 978-0199658565. [Google Book](https://books.google.cl/books?id=vkueAgAAQBAJ&printsec=frontcover) | [Amazon Book](https://www.amazon.com/Building-Bioinformatics-Solutions-Conrad-Bessant/dp/0199658560)
*	Lesk. Introduction To Bioinformatics. Edición: 5. Oxford, United Kingdom: Oxford University Press, 2019. ISBN-13: 978-0198794141. [Google Book](https://books.google.cl/books?id=xYmcAQAAQBAJ&printsec=frontcover) | [Amazon Book](https://www.amazon.com/-/es/Lesk/dp/0198794142)
*	Rocha, Miguel ; Ferreira, Pedro G.: Bioinformatics Algorithms: Design and Implementation in Python. 1 edition. Aufl. Waltham, MA : Academic Press, 2018 — ISBN 978-0-12-812520-5. [Google Books](https://books.google.cl/books?id=rkc1DwAAQBAJ&printsec=frontcover) | [Amazon Book](https://www.amazon.com/-/es/Miguel-Rocha/dp/0128125209)
*	Stevens, Tim J. ; Boucher, Wayne: Python Programming for Biology: Bioinformatics and Beyond. 1 edition. Aufl. Cambridge, United Kingdom : Cambridge University Press, 2015 — ISBN 978-0-521-72009-0 [Google Book](https://books.google.cl/books?id=oQNoBgAAQBAJ&printsec=frontcover) | [Amazon Book](https://www.amazon.com/-/es/Tim-J-Stevens-ebook/dp/B00SYVZ3WC/ref=sr_1_1?__mk_es_US=%C3%85M%C3%85%C5%BD%C3%95%C3%91&dchild=1&keywords=Python+Programming+for+Biology%3A+Bioinformatics+and+Beyond&qid=1586376277&s=books&sr=1-1)
*	Loging, W. T. (Hrsg.): Bioinformatics and Computational Biology in Drug Discovery and Development. Reprint edition. Aufl. S.l. : Cambridge University Press, 2018 — ISBN 978-1-108-46115-3. [Google Book](https://books.google.cl/books?id=6Bd-CwAAQBAJ&printsec=frontcover) | [Amazon Book](https://www.amazon.com/-/es/William-T-Loging-ebook/dp/B01B1G83SM/ref=sr_1_1?__mk_es_US=%C3%85M%C3%85%C5%BD%C3%95%C3%91&dchild=1&keywords=Bioinformatics+and+Computational+Biology+in+Drug+Discovery+and+Development&qid=1586376386&s=books&sr=1-1)