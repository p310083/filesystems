SWAP

La swap o espacio de intercambio, es un espacio reservado en el disco duro que puede usarse como una extensión de memoria virtual de 
un sistema (entendiéndose como memoria a la RAM). Es una técnica utilizada desde hace tiempo para hacer creer a los programas que hay 
más memoria de la que realmente existe. Siendo el propio sistema operativo el que se encarga de pasar datos a la swap cuando necesita 
más espació libre en la RAM y viceversa.

En Linux, la memoria total disponible por el sistema estará formada por la cantidad de memora RAM instalada + la swap disponible. 
Cabe aclarar que el acceso a la swap (disco duro) es más lento que el acceso a la memoria RAM (memoria de estado sólido), por lo que 
si nuestro ordenador está muy cargado de trabajo y hace uso intensivo de la swap, la velocidad del sistema disminuirá. Un uso muy 
intensivo y continuo de la swap es un indicativo de que necesitamos más memoria en nuestro sistema para que funcione desahogado con 
respecto al uso que le estamos dando.

Su uso en sistemas operativos

Actualmente todos los sistemas operativos cuentan con funciones de intercambio entre la memoria RAM y alguna sección de memoria virtual 
creada en disco. Por lo que diferentes versiones de swap pueden ser encontradas tanto en sistemas operativos Windows, como en GNU/Linux 
o Unix, en donde cada sistema operativo gestiona la memoria virtual de intercambio de forma distinta.

-	Microsoft Windows usa un fichero de intercambio desde su versión 3.1 (1992), la primer versión en usar memoria virtual. Lo cual 
implementa mediante un fichero situado en el directorio raíz (C:\) o en el directorio del sistema (C:\WINDOWS\), y puede tener 
diferentes nombres, pero a partir de su versión NT se le puede reconocer como “pagefile.sys”.
-	En GNU/Linux se suele usar con una partición de intercambio, aunque también permite usar ficheros de intercambio.

¿Cómo creo una swap?

El espacio swap o de intercambio será normalmente una partición de disco, pero como ya se mencionó, también puede ser un archivo. Por 
ejemplo en el caso de distribuciones basadas en Linux, se pueden crear un espacio de intercambio durante la instalación del sistema 
operativo o en cualquier momento posterior en caso de ser necesario.

¿Cuál es el tamaño apropiado de una swap?

A la hora de crear una swap se nos presenta la siguiente duda: ¿Cuántos megas/gigas debe de ocupar? Y un mito muy extendido afirma que 
debemos elegir el doble en relación con la memoria RAM que tenga el equipo, pero hoy en día con las enormes memorias disponibles esto 
no es solo falso sino que pierde mucho el sentido. Por lo que expertos en el tema y a manera general nos explican el tamaño ideal de 
una partición swap con respecto a la RAM disponible:

-	En equipos con memoria RAM de hasta 1 GB, la swap deberá de ser igual de grande que la RAM.
-	Entre 2 y 4 GB, la swap deberá ser la mitad de grande que la memoria RAM disponible en el equipo.
-	En casos con más de 4 GB, la swap no deberá de sobrepasar los 2 GB como mucho. Más allá de eso, difícilmente sería aprovechado por 
el sistema operativo como zona de intercambio.

Uno de los motivos por los que se establece un tamaño máximo de 2 GB es que son pocos los ficheros que puedan manejar esa cantidad de 
swap. Pero también hay que tener en cuenta que otro uso de la swap es permitir una hibernación completa del sistema, con lo que habría 
que volcar toda la RAM en esa partición. Por lo tanto si la eficiente hibernación del sistema operativo es una necesidad a cubrir, un 
tamaño de swap igual a la RAM  sería lo ideal.

Ventajas de utilizar swap

-	Permite correr una mayor cantidad de programas y de estar bien configurada, puede mejorar el rendimiento de los procesos ejecutados.

Desventajas de la swap

-	Un problema no menor del intercambio entre RAM y swap, reside en los tiempos necesarios para realizar las copias a la memoria de 
apoyo, ya que normalmente estaremos hablando de discos duros, lo cual en términos de tiempo son muy costosos al estar constantemente 
copiando y leyendo procesos. Cuando estos tiempos se hacen muy largos, pueden terminar haciendo más lenta la ejecución del programa en 
cuestión. Este problema es conocido como “thrashing” y la forma más simple de solucionarlo es agregar más memoria o bien, mejorar el 
diseño de las aplicaciones para que disminuya su consumo.

Elaboró: Ing. Emmanuel Zúñiga T. 
p310084@uach.mx

Referencias:
https://es.wikipedia.org/wiki/Espacio_de_intercambio
https://www.genbeta.com/linux/cual-es-el-tamano-optimo-para-la-swap-en-linux
