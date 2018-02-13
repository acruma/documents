# Compara diversos sistemas de archivos (NTFS, ext4, FAT) y analiza sus diferencias y ventajas.

#### *FAT32 (FILE ALLOCATION TABLE)*
FAT es un sistema de archivos desarrollado para MS-DOS. Es el sucesor de FAT16, que a su vez es sucesor de FAT12. El tamaño máximo soportado por este sistema es de 4 GB-1 Byte y se utiliza para el intercambio de datos entre distintos sistemas operativos de un mismo equipo. Además, también es utilizado en tarjetas de memoria y dispositivos similares.
Si intentamos meter en un pendrive de 16 GB en sistema FAT32 un archivo de 10 GB, no nos dejará, pues este archivo supera esos 4GB-1Byte.

#### *NTFS (NEW TECHNOLOGY FILE SYSTEM)*
Está incluido en las versionas de Windows 2000, Windows XP, Windows Server 2003, Windows Server 2008, Window Vista, Windos 7 y Windows 8. El tamaño mínimo recomendado para las particiones de este tipo de sistemas de archivos es de 10 GB, siendo posibles tamaños mayores. Además, a diferencia de FAT32, distingue entre mayúsculas y minúsculas.
En cuanto al rendimiento, NTFS es mucho más rápido en el acceso a los archivos que una partición tipo FAT. Esto se debe a que utiliza un árbol binario de alto rendimiento para localizar los archivos. El tamaño límite de una partición es de 17*10⁹ Bytes.
Por otra parte, los sistemas de archivos NTFS son más estables que los FAT. Además, NTFS cifra archivos, cosa que FAT no hace.

#### *EXT3 (THIRD EXTENDED FILESYSTEM)*
Es un sistema de archivos principalmente utilizado en distribuciones Linux con registro por diario (journaling). Está siendo reemplazado por su sucesor, ext4, aunque todavía se utiliza.

*¿Qué es el journaling?*

El journaling se basa en llevar un registro diario en el que se almacena la información necesaria para restrablecer los datos del sistema afectados por un cambio, en caso de que falle.
Con el sistema de archivos ext3 se obtiene una gran reducción del tiempo necesario para recuperar un sistema de ficheros después de una caída. Por tanto, podemos decir que sus principales objetivos son la disponibilidad y confiabilidad.
Imaginemos que apagamos nuestro equipo incorrectamente. Ext3 se encargará de que al encenderlo lo tengamos igual que lo dejamos antes de apagarlo.

#### *EXT4 (FOURTH EXTENDED FILESYSTEM)*
Es una mejora compatible de ext3 que utiliza menos CPU y mejora la velocidad de lectura y escritura. Además, soporta volúmenes de hasta 1024 PiB (PebiByte) ( 1 PiB = 2^50 Bytes ). Como acabo de decir, mejora la velocidad de lectura y escritura en comparación con ext3, pero es más lento en la eliminación de archivos.

En ext4 se introducen los exents, que se utilizan para reemplazar al tradicional esquema de bloques utilizado por ext2 y ext3. Los exents mejoran el rendimiento al trabajar con ficheros de gran tamaño.

[Volver](https://github.com/acruma/documents)|[Siguiente - B]()
--|--
