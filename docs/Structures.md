# Análisis de Estructura de Proteínas 
Los mecanismos moleculares y celulares que permiten el metabolismo de nuestras células esta regulado por la función de genes que se traducen en proteínas. Las proteínas estan formadas por aminoácidos que se pliegan en una estructura tridimensional dando forma y funcionalidad, que con la flexibilidad de estas estructuras inmersas en un medio acuoso y sales, en conjunto con la interacción de otras proteinas, le otorgan la dinámica a los procesos vivos y el funcionamiento de estos en condiciones normales y patológicas. La compresión de estos mecanismos, su dinámica, es fundamental tanto en procesos biotecnológicos como en la preservación de la salud humana, tanto de otros animales como las plantas.

RA: Realizar análisis de secuencias de origen biológico.
EV: Desarrollar una función en python en cuaderno de programación para realizar una tarea asignada de análisis de estructura.

Este es el contenido que iremos revisando en el curso, donde se trabajará en un contexto general y revisión de 15-20 minutos por concepto con 30 minutos de una actividad. 

# El Banco de Datos de Proteínas
Las coordenadas de las estructura de proteínas son depositadas en el Banco de Datos de Proteínas, [PDB](https://www.rcsb.org). Estas coordenadas provienen principalmente de la determinación de mapas de densidad electrónica desde experimentos de [cristalografía de rayos X](https://www.youtube.com/watch?v=-6j7_xS5FAI), [resonancia nuclear para determinación de estructura de proteínas](https://en.wikipedia.org/wiki/Nuclear_magnetic_resonance_spectroscopy_of_proteins), de [modelamiento comparativo](https://en.wikipedia.org/wiki/Homology_modeling), y finalmente desde [crio-microscopía electrónica](https://en.wikipedia.org/wiki/Transmission_electron_cryomicroscopy). Un bioinformático debe conocer la estructura de un archivo PDB y generar visualizaciones tridimensionales de estas estructuras para realizar un análisis de estructura-función.

## Conceptos
* PDB format
* Descargar PDB
* Pymol Visualizar 3D
* NGLView en Jupyter

## Lecturas
[Bases de datos de estructuras de proteínas](https://doi.org/10.1016/B978-0-12-809633-8.20280-X)
[Historia del PDB](https://www.rcsb.org/pages/about-us/history)
[Visualización de proteínas](https://doi.org/10.1016/B978-0-12-809633-8.20283-5)
[Formato de un archivo PDB](http://www.wwpdb.org/documentation/file-format-content/format33/v3.3.html)
[Visualizador molecular Pymol](https://pymol.org)|[Conda](https://anaconda.org/schrodinger/pymol)
[Visualizador molecular NGLView](https://academic.oup.com/bioinformatics/article/34/7/1241/4721781)|[Github](https://github.com/arose/nglview)

## Actividades
* [Elegir una molécula del mes](http://pdb101.rcsb.org/browse)
* Instalar Pymol
* Descargar un archivo PDB en Pymol
* Visualizar el formato de su archivo
* Generar una vista del sitio activo
* Inscrustar una vista de una molécula en Jupyter

# Modelamiento de Proteínas
La determinación de estructuras de proteínas es un proceso experimentalmente costoso en tiempo en dinero. Mientras desde análisi de filogenia y compararndo secuencias se pueden obtener secuencias con un alto porcentaje de identidad (>50%), usando la información de estos alineamiento se ha demostrado que es posible extrapolar esta estructura para reconstruir proteínas relacionadas. Esta técnica es muy utilizada por bioinformáticos, cuando se dispone de una estructura cristalizada y es homologa a nuestra proteína de interes. Muchas veces las proteínas cristalizados son de microorganismos y no humanas y con modelamiento comparativo se pueden calcular estas estructuras para realizar análisis de estructura-función. En los últimos años con el poder computacional que se dispone incluso se ha simulado con éxito el plegamiento de proteínas desde su secuencia primaria.    

## Conceptos
* [Algoritmos en modelamiento comparativo](https://doi.org/10.1016/B978-0-12-809633-8.20484-6)
* [Algoritmos es modelamiento *ab initio*](https://doi.org/10.1016/B978-0-12-809633-8.20321-X)
* [Evaluación del modelo](https://doi.org/10.1016/B978-0-12-809633-8.20282-3)

## Lecturas
[Modeller]([Modeller](https://salilab.org/modeller))
[Modelamiento básico con Modeller](https://salilab.org/modeller/tutorial/basic.html)
[ModFOLD](https://www.reading.ac.uk/bioinf/ModFOLD/index.html)

## Actividades
* Instalar Modeller
* Ejecutar modeler en Jupyter
* Realizar una búsqueda de moldes
* Construir un alineamiento en formato PIR
* Construir un modelo de proteína.
* Evaluar un modelo de una proteína.

# Cribado Molecular
La comunicación a nivel molecular y la transferencia de señales, fuerzas, e inclusive reconocimiento celular, esta gobernado por las fuerzas de interacción molecular, y el proceso de unión entre estas moléculas con una energía determinada se denomina cribado (*docking*) molecular. En biología estos procesos están involucrados en la transducción de señales, en el transporte de metabolitos, en el reconocimiento de sustratos, en la afinidad de anticuerpos, en la sinapsis, entre otrso; así como en la acción de practicamente todos los fármacos que modulan una respuesta biológica. El cribado molecular nos permite calcular mdoos de unión entre proteínas, seleccionar ligandos de una base de datos que se unirían a un receptor, evaluar la energía de unión.

## Conceptos
* Docking proteína-proteína
* Docking proteína-ligando
* Análisis de docking molecular

## Lecturas
* [Algoritmos de cribado molecular](https://doi.org/10.1016/B978-0-12-809633-8.20485-8)
* [Diseño de fármacos basado en estructura](https://doi.org/10.1016/B978-0-12-809633-8.20275-6)
* [Smina docking])(https://sourceforge.net/projects/smina/files)
* [Lightdock](https://lightdock.org)

## Actividades
* Realizar un docking molecular receptor-ligando con smina, analizar los resultados.
* Realizar un docking molecular proteína-proteína con lightdock, analizar los resultados.

# Simulaciones de Dinámica Molecular
Los procesos biológicos no son estáticos y la vida depende de la dinámica molecular al interior de la célula. Estos procesos respoden a las leyes de la mecánica estadística y la fisicoquímica, donde tempranamente se han desarrollado métodos para realizar simulaciones de ensambles termodinámicos que representan los componentes de la vida desde sus átomos y poder ver estos procesos en una resolución naométrica y en tiempos de femtosegundos. Con la potencia de cálculo computacional en sistemas distribuidos, tanto de cluster como en GPU, se ha logrado simular sistemas tan grandes como virus y ribosomas; mientras en sistemas más pequeños se han logrado simulaciones de milisengudos a segundos. Hoy estas simulaciones son parte de las herramientas que un bioinformático utiliza para analizar sistemas biológicos y nuevamente establecer relaciones de estructura-función.

* Simulaciones de dinámica molecular
* Campo de fuerza
* Ensambles
* Análisis de SDM
* [MDanalysis](https://www.mdanalysis.org)
* [Openmm](http://openmm.org)

## Lecturas
[Simulaciones de dinámica molecular (SDM)](https://doi.org/10.1016/B978-0-12-809633-8.20284-7)
[SDM y diseño de fármacos](https://www.sciencedirect.com/science/article/pii/B9780128096338201544)
[Algoritmo de simulaciones de dinámica molecular - Capítulo 3.4](https://ftp.gromacs.org/pub/manual/manual-5.0.4.pdf)
[Campos de fuerza - Capítulo 3.1](https://ambermd.org/doc12/Amber19.pdf)
[Premio Nobel de Química 2013](https://www.youtube.com/watch?v=NuaeD9xYBtY)

## Actividades
* Instala openmm y mdanalysis
* Crear un ensamble termodinámico con openmm-setup
* Ejecutar una simulacion de dinámica molecular con openmm: minimización, equilibración y producción.
* Analizar la trayectoria en cuaderno de Jupyter con MDanalysis.

# Extras [Opcional].

## Módulos python para análisis de estructuras
* [Prody](http://prody.csb.pitt.edu)
* [Biopandas](http://rasbt.github.io/biopandas)
* [Pytraj](https://amber-md.github.io/pytraj/latest/index.html)
* [MDTraj](http://mdtraj.org)
* [Bio3D](http://thegrantlab.org/bio3d)

## Bioinformático de refinado de datos cristalográficos
En cristalografía de rayos X, al obtener el mapa de densidad electrónica y con una fase se debe refinar el modelo para ellos se dispone de software que nos permite realiar esta tarea, desarrollando un modelo del sistema y definiendo parámetros de la resolución y de confiabilidad por regiones de la proteína. Un bioinformático puede desarrollar estas tareas. 

Software escrito o con interfaz en Python
* [Phenix](http://www.phenix-online.org)
* [General MacroMocelecular I/O (GEMMI)](https://gemmi.readthedocs.io)
* [CCP4](http://www.ccp4.ac.uk)

## Diseño de fármacos
El diseño de fármacos es una aplicación de la bioinformática donde la estructura de proteínas se entrelaza con la quimioinformática, principalmente en el manejo de base de datos de moléculas pequeñas, el estudio de sus propiedades y el desarrollo de experimentos de cribado molecular en conjunto con cálculos de energía libre que es indirectamente proporcional a la afinidad entre moléculas, en esta última se desarrollan cálculos termodinámicos que van desde la enegría libre desde el cálculo de nergías de solvatación, la integración termódinámica, perturbaciones de energía libre y energía libre calculada desde trabajo, entre otros.

* [PBSA and GBSA Capítulo 32-33](https://ambermd.org/doc12/Amber19.pdf) 
* Perturbaciones de Energía libre. [FEP v/s GBSA en PIP](https://doi.org/10.1016/j.jmb.2019.02.003)  
* [Integración termodinámica - Capítulo 21.1](https://ambermd.org/doc12/Amber19.pdf)
* Energía calculada desde trabajo. [Paprika](https://github.com/slochower/pAPRika)|[BLUEs](https://github.com/MobleyLab/blues)
* Quimiometría: [RDkit](https://www.rdkit.org)|[OpenBabel](http://openbabel.org)
* Base de datos: [ZINC](https://zinc.docking.org)

## Evaluación del efecto de mutaciones en proteínas
La bioinformática posee varias subdisciplinas donde destaca el análisis de estructuras de proteínas y la genómica, no obstante durante los últimos años ambas disciplinas se han solapado para poder estudiar el efecto de mutaciones en genes en la función de proteínas. Estas metodologías combinan un procesamiento para la identificación de las variantes del individuo con el genoma de referencia, la clínica del paciente y el estudio del efecto de estas mutaciones en la proteína.

* Automatizar la configuración y análisis de mutaciones en la unión de fármacos. [Referencia](https://doi.org/10.1186/s12859-019-2774-9)
* Evaluar el efecto de las mutaciones en el plegamiento. [Referencia](https://doi.org/10.1073/pnas.1715896115)
* Evaluar el efecto de mutaciones en la interfaz de proteína-proteína. [Referencia](https://doi.org/10.1371/journal.pone.0219935)

## Crio-miscropía electrónica
La criomiscropía electrónica es una técnica para obtener la disposición espacial de proteínas, en un princicpio se logran resoluciones de alrededor de los 10 Amstrong, no obstante con el avance de la técnica y del refinameinto mediante software hoy en día se pueden logar resolutiones cercanas a 3 Amstrong, lo que ha producido un desarrollo rápìdo de experimentos para observar sistemas más grandes, complejos y en condiciones naturales.

* [Premio Nobel de Química 2017](https://www.youtube.com/watch?v=026rzTXb1zw)
* [Software para resolver Criomicroscopía electrónica](https://dx.doi.org/10.1038%2Fs41592-019-0396-9)
* [Py-EM](https://git.embl.de/schorb/pyem)