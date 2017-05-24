Filesystem ext4

ext4 (fourth extended filesystem o «cuarto sistema de archivos extendido») es un sistema de archivos transaccional 
(en inglés journaling), anunciado el 10 de octubre de 2006 por Andrew Morton, como una mejora compatible de ext3. 
El 25 de diciembre de 2008 se publicó el kernel Linux 2.6.28, que elimina ya la etiqueta de "experimental" de código de ext4.

Las principales mejoras son:

Soporte de volúmenes de hasta 1024 PiB.
Soporte añadido de extent.
Menor uso del CPU.
Mejoras en la velocidad de lectura y escritura.

Desarolladores: Mingming Cao, Dave Kleikamp, Alex Tomas, Andrew Morton, y otros

En ext4 se introducen los exents, que se utilizan para reemplazar al tradicional esquema de bloques utilizado por 
ext2 y ext3. Los exents mejoran el rendimiento al trabajar con ficheros de gran tamaño.

Sistema de archivos de gran tamaño:
El sistema de archivos ext4 es capaz de trabajar con volúmenes de gran tamaño, hasta 1 exbibyte1 y ficheros de 
tamaño de hasta 16 TiB.

Límite de 32000 subdirectorios superado:
En ext3 el nivel de profundidad en subdirectorios permitido estaba limitado a 32000. 
Este límite ha sido aumentado a 64000 en ext4, permitiendo incluso ir más allá de este límite (haciendo uso de "dir_nlink"). 
Para permitir un rendimiento continuo, dada la posibilidad de directorios mucho más grandes, htree está activado por defecto 
en ext4. Esta función está implementada desde la versión 2.6.23. htree está también disponible en ext3 cuando la función dir_index 
está activada.
