# Análisis de Secuencias Biológicas
El análisis de secuencias es una de las primera aplicaciones en bioinformática que aprenderemos, esta es la base para elucidar mecanismos biológicos y moleculares desde las propiedades evolutivas y de herencia que se aplican tanto para secuencias de ADN y secuencias de proteínas, estas bases son esenciales para poder trabajar como bioinformático en análisis genómicos y estructurales para comprender la relación secuencia-función.

RA: Realizar análisis de secuencias de origen biológico.
EV: Desarrollar una función en python en cuaderno de programación para realizar una tarea asignada de análisis de secuencias.

# Módulos Python para Bioinformáticos 
Para realizar análisis de secuencias primero debemos explorar algunas bibliotecas de Python que utilizaremos durante esta unidad. Biopython es una biblioteca que nos conecta con las principales tareas bioinformáticas que debemos realizar, así como nos permite trabajar con algunas bases de datos donde destaca Entrez (que incluye al National Centre for Biotechnology Information-NCBI), ExPASy (Expert Protein Analysis System), y RCSB (Research Collaboratory for Structural Bioinformatics PDB). 

## Conceptos:
* [Biopython](https://biopython.org)
* [PANDAS](https://pandas.pydata.org)
* [Seaborn](https://seaborn.pydata.org)

## Lecturas
* [Capítulo 1-2 Biopython](http://biopython.org/DIST/docs/tutorial/Tutorial.html)
* [Pandas en 10 minutos](https://pandas.pydata.org/pandas-docs/stable/getting_started/10min.html)
* [Relaciones estadísticas con seaborn](https://seaborn.pydata.org/tutorial/relational.html)

## Actividades
* Crear un cuaderno Jupyter con una secuencia de nucleotidos utilizando Biopython.
* Realizar operaciones con la secuencia de nucleotidos.
* Generar una DataFrame con Pandas de frecuencia de nucleotidos.
* Graficar la tabla con seaborn.

# Descripción de Secuencias Biológicas
Las secuencias biológicas son de dos tipos princiaples de nucleótidos y de proteínas, y cada una como objeto biológicoposee sus atributos que dependen de sus propiedades biológicas, operaciones como la transcripción y replicación, el formato son propias de estos elementos así como la conexión de las bases de datos.

## Conceptos
* ADN
* Proteínas
* Obtener desde base de datos
* Operaciones con secuencias

## Lecturas
* [La secuencia de ADN](https://en.wikipedia.org/wiki/DNA)
* [La secuencia de proteína](https://en.wikipedia.org/wiki/Protein)
* [Secuencias desde Entrez](https://www.ncbi.nlm.nih.gov/books/NBK44863)
* [Secuencias desde Uniprot](https://www.youtube.com/user/uniprotvideos)

## Actividades
* Crear un cuaderno Jupyter donde se obtenga una secuencia de proteínas con Biopython.
* Realizar operaciones con la secuencia de proteínas.
* Generar una DataFrame con Pandas de frecuencia de aminoácidos.
* Graficar la tabla con seaborn.

# Evolución Molecular
La evolución molecular se encarga de los cambios en la secuencia de genes y proteínas, preguntándose por la tasa de mutación y los mecanismos que estos cambios e el tiempo a nivel molecular. Este campo se entrelaza con la genética de poblaciones clásica y con la genómica comparativa (revisada a cabalidad en el curso del próximo semestre de Bioinformática 2).

Conceptos:
* Evolución Molecular
* Reloj Molecular
* Matrices de sustitución
* Alineamiento local
* Alineamiento global
* Similaridad de secuencias

## Lecturas
* [Evolución molecular](https://en.wikipedia.org/wiki/Molecular_evolution)
* [La evolución de familia de proteínas](https://doi.org/10.1016/B978-0-12-809633-8.20268-9)
* [Matrices de sustitución](https://es.wikipedia.org/wiki/Matriz_de_sustituci%C3%B3n)
* [Algoritmo de Needleman-Wunsch](https://es.wikipedia.org/wiki/Algoritmo_Needleman-Wunsch)
* [Algoritmo de Smith-Waterman](https://en.wikipedia.org/wiki/Smith%E2%80%93Waterman_algorithm)
* [BLAST](https://es.wikipedia.org/wiki/BLAST)

## Actividades
* Crear en Jupyter una matriz de similaridad
* Crear una función de scoring
* Realizar un BLAST con Biopython.

# Alineamiento de Secuencias
El alineamiento de secuencias es una de las herramientas básicas de un biuoinformático y se utiliza para extrapolar información desde organismos, genes y proteínas conocidas a otros. También, se utiliza para identificar patrones relacionados a una función y estudiar las variaciones de las secuencias en el tiempo. El alinemaiento de secuencias es una herramienta bases para las búsquedad por similaridad, los análisis de conservación, la reconstrucción de filogenia y el modelamiento comparativo de proteínas.

## Conceptos:
* [Alineamiento de pares](https://doi.org/10.1016/B978-0-12-809633-8.20317-8)
* [Alineamiento múltiple de secuencias](https://doi.org/10.1016/B978-0-12-809633-8.20318-X)
* Análisis de alineamientos

## Lecturas
* [MAFFT](https://mafft.cbrc.jp/alignment/software)
* [FASTA36](https://github.com/wrpearson/fasta36)
* [Alineamiento de pares en Bioython](https://biopython.org/docs/dev/api/Bio.Align.html)
* [Alineamiento múltiple de secuencias en Biopython](https://biopython.org/wiki/AlignIO) 

## Actividades
* Descargas secuencias de proteínas
* Reaizar un análisis de pares con Biopython
* Realizar un análisis de secuencias multiples con MAFFT.
* Leer el alineamiento y calcular la conservación por cada columna.
 
# Filogenia Molecular
La reconstrucción de filogenia e suna herramienta para explorar la historia evolutiva de un grupo de secuencias e inferir relevancia de los componentes en el alineamiento y lograr clasificar grupos de estudio para obtener mejores alineamientos, búsuqedas de patrones, análisis de conservación, entre otros. Una filogenia se puede representar en forma de árbol, el cual contiene nodos que conectan ramas entre sí. Estos nodos y ramas pueden representar diferentes eventos, procesos, o relaciones. Dependiendo del árbol filogenético, por ejemplo: los nodos podrían representar eventos de especiación, y las ramas, las relaciones entre los diferentes grupos.

## Conceptos
* Filogenia 
* Métodos de distancia
* Métodos de probabilidad
* Análisis filogenético

## Lecturas
* [Computacional Filogenia](https://en.wikipedia.org/wiki/Computational_phylogenetics)
* [Software RAxML](https://cme.h-its.org/exelixis/web/software/raxml/)|[Artículo](https://academic.oup.com/bioinformatics/article/30/9/1312/238053)
* [iTOL](https://itol.embl.de)

## Actividades
* Descargar un grupo de sequences desde BLAST.
* Alinear las secuencias
* Construir filogenia RAxML desde Jupyter.
* Visualizar en iTOL.

# Diseño de Partidores
El diseño de partidores es una herramienta fundamental en biología molecular, y los bioinformáticos pueden requerir diseñar partidores para realizar amplificaciones por reacción en cadena de la polimerasa (PCR) para identificar organismos, para realizar clonamiento de genes, para introducir mutaciones sitio dirigidas, para realizar editado de genes, cuantificar cantidad de transcritos y silenciar genes, entre otras aplicaciones basadas en la complementariedad del ADN y enzimas involucradas en su procesamiento. 

## Conceptos
* Reacción en cadena de la polimerasa
* Clonamiento
* Mutaciones sitio dirigidas

## Lecturas
* [Reacción en cadena de la polimerasa](https://es.wikipedia.org/wiki/Reacci%C3%B3n_en_cadena_de_la_polimerasa)
* [Clonamiento molecular](https://en.wikipedia.org/wiki/Molecular_cloning)
* [Mutagénesis sitio dirigida](https://en.wikipedia.org/wiki/Site-directed_mutagenesis)

## Actividades
* Diseñar una función para calcular un partidor de un gen.
* Diseñar una función para calcular la TM de un partidor.

# Extras [Opcional]

## Módulos Python: 
* [Scikit-Bio](http://scikit-bio.org) | [Scipy])(https://www.youtube.com/watch?v=ZpgkRQooGqo). Este módulo entrega herramientas para realizar analisis de secuencias.
* [Bio.Phylo](https://biopython.org/DIST/docs/api/Bio.Phylo-module.html)
* [DendroPy](https://dendropy.org)|[Referencia](https://academic.oup.com/bioinformatics/article/26/12/1569/287181) 
* [ETE Toolkit](http://etetoolkit.org)|[Referencia](https://academic.oup.com/mbe/article/33/6/1635/2579822)
* [TreeSwift](https://github.com/niemasd/TreeSwift)|[Referencia](https://www.sciencedirect.com/science/article/pii/S2352711019300767)
* [Primer3](https://libnano.github.io/primer3-py). Este módulo busca la automatización del diseño de partidores.

## Secuencias de membrana
Las proteínas de membrana se clasifican como receptores, transportadores y canales iónicos. Estas proteínas se forman principalmente empacando hélices transmembrana de 15-35 aminoácidos de largo en orientación perpendicular a la membrana lipídica. Estas restricciones impuestas por la membrana de caracter hidrofóbico permitieorn identificar proteínas de membrana desde sus seccuencias por los perfiles de hidrofobicida que estas generaban. Luego con las cristalización de proteínas de membrana y la obtención de la disposición tridimensional de sus átomos se refinaron estas herramientas, existiendo herramientas bioinformáticas especiales para secuencias de proteína de membrana.

* Predicción de proteínas transmebrana
* [Predicción de tologías de proteinas de membrana](https://doi.org/10.1016/B978-0-12-809633-8.20269-0)
* bases de datos de proteínas de membrana
[Topcons](http://topcons.cbr.su.se)|[Memsat3](http://bioinf.cs.ucl.ac.uk/software_downloads/memsat)|[TCDB](http://www.tcdb.org/)|[MPKS](https://blanco.biomol.uci.edu/mpstruc)

## Secuencias de sistema inmune
Las secuencias y estructuras presentes en el sistema inmune deben tener patrones de reconocimeinto que nos entregan la capacidad de reconocer lo que pertenece a nuestro organismo de lo extraño. Esta funcionalidad se basa en la capacidad de combinatoria que es posible de generar nuestro sistema inmune y las interacciones moleculares del reconocimiento entre proteínas y proteínas u otros agentes moleculares. El reconcimiento de epítopes para el diseño de vacunas, la desinmunización, el reconocimiento por MHC, TLR, anticuerpos, entre otros aspectos puede ser estudiado por métodos bioinformáticos. Incluse se ha denominado inmunoinformática a esta área que estudia estos mecanismo aplicando técnicas computacionales.

* [Bases de datos inmunoinformáticas](https://doi.org/10.1016/B978-0-12-809633-8.20469-X)
* [Predicción de epitopes](https://doi.org/10.1016/B978-0-12-809633-8.20248-3)|[Herramientas bioinformáticas](https://www.sciencedirect.com/science/article/pii/S1532046414002330)
* [Predicción de estructuras de TCR](https://www.blopig.com/blog/2020/03/tcrbuilder-multi-state-t-cell-receptor-structure-prediction)
* Diseño de anticuerpos [Referencia])(https://academic.oup.com/bioinformatics/article/36/7/2126/5645171)
* Estructura de regiones determinantes de la complemetariedad (CDR)
* Desinmunización