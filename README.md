# Ataques de Red #
Noviembre 2022
## Replay atack ##

### Definición ###

Un ataque de replay, también llamado ataque de reproducción o de reinyección, es un ciberataque en el cual una entidad maliciosa intercepta y a continuación repite una transmisión de datos válida a través de una red. Debido a la validez de los datos originales -que habitualmente provienen de un usuario autorizado-, los protocolos de seguridad de la red actúan frente al ataque como si se tratara de una transmisión de datos normal. Dado que los mensajes originales son interceptados y retransmitidos de forma literal, los hackers que ejecutan ataques de replay no se ven obligados a desencriptarlos.

### Ejemplos ###

Un ejemplo de ataque por replay es el robo de las de datos de las tarjetas crédito.

[ejemplo](https://www.youtube.com/watch?v=18O_Xn5CPvo)

### Parte de la red o del sistema que se ve comprometido ###

En un caso de ataque por replay la información del usuario es lo que se mas se ve comprometido y la transmisión de datos.

## Buffer Overflow Attack

### Definición
Es un error de software que se produce cuando un programa no controla adecuadamente la cantidad de datos que se copian sobre un área de memoria reservada a tal efecto (buffer): Si dicha cantidad es superior a la capacidad preasignada, los bytes sobrantes se almacenan en zonas de memoria adyacentes, sobrescribiendo su contenido original, que probablemente pertenecían a datos o código almacenados en memoria. Esto constituye un fallo de programación.

Una vulnerabilidad puede ser aprovechada por un usuario malintencionado para influir en el funcionamiento del sistema. En algunos casos el resultado es la capacidad de conseguir cierto nivel de control saltándose las limitaciones de seguridad habituales. Si el programa con el error en cuestión tiene privilegios especiales constituye en un fallo grave de seguridad.

Se denomina shellcode al código ejecutable especialmente preparado que se copia al host objeto del ataque para obtener los privilegios del programa vulnerable.

Hay varios tipos:

- Ataque de desbordamiento de pila: este es el tipo más común de ataque de desbordamiento de buffer e implica desbordar un buffer en la pila de llamadas.
- Ataque de desbordamiento de montón: este tipo de ataque apunta a datos en el grupo de memoria abierta conocido como el montón.
- Desbordamiento de enteros: en un desbordamiento de enteros, una operación aritmética da como resultado un entero (número entero) que es demasiado grande para el tipo de entero destinado a almacenarlo. Esto puede provocar un desbordamiento del buffer.
- Desbordamiento Unicode: un desbordamiento Unicode crea un desbordamiento de buffer insertando caracteres Unicode en una entrada que espera caracteres ASCII. ASCII y Unicode son estándares de codificación que permiten que las computadoras representen texto. Por ejemplo, la letra ‘a’ está representada por el número 97 en ASCII. Mientras que los códigos ASCII solo cubren caracteres de idiomas occidentales, Unicode puede crear caracteres para casi todos los idiomas escritos en la tierra debido a que hay muchos más caracteres disponibles, muchos caracteres Unicode son más grandes que el carácter ASCII más grande.

### Ejemplo

El atacante usaría un exploit de desbordamiento de búfer para aprovechar un programa que está esperando la entrada de un usuario.

[Ejemplo](https://youtu.be/f_NXlTfXaSQ)



### Parte de la red o del sistema que se ve comprometido

Los desbordamientos del buffer pueden ocurrir vulnerabilidades en cualquier software.
