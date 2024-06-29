Proyecto de Programación de Servicios y Procesos: Sockets

Este proyecto contiene una serie de ejercicios que exploran la programación de servicios utilizando sockets en Java. Los ejercicios están organizados en dos boletines, cada uno con varios problemas que abarcan diferentes aspectos de la programación de sockets TCP y UDP.
Requisitos Previos

    Java Development Kit (JDK)
    IDE de Java (Eclipse, IntelliJ IDEA, NetBeans, etc.)
    Conocimientos básicos de programación en Java
    Conocimientos básicos de redes y sockets

Boletín 1: Sockets
Ejercicio 1: Información de Nombres de Máquinas o IPs

Descripción:
Este programa permite introducir desde la consola nombres de máquinas o direcciones IP y muestra información sobre ellas utilizando la clase InetAddress.
Ejercicio 2: Conexión a URL y Mostrar HTML

Descripción:
Este programa recoge una URL desde el teclado y abre una conexión al sitio web indicado, mostrando el código HTML de la página inicial.
Ejercicio 3: Servidor y Cliente TCP con Puertos

Descripción:
Implementa un servidor TCP que acepta conexiones de 2 clientes y muestra sus puertos locales y remotos. El cliente también muestra los puertos locales y remotos a los que se encuentra conectado, así como la IP de la máquina remota.
Ejercicio 4: Enviar Número y Recibir Cuadrado

Descripción:
El programa cliente introduce un número entero y se lo envía al servidor, el cual le devuelve el cuadrado del número.
Ejercicio 5: Servidor TCP para N Clientes

Descripción:
Este servidor puede atender hasta 3 clientes y les envía un mensaje indicando su número de cliente. El cliente muestra el mensaje recibido. La implementación se puede extender para atender a N clientes, siendo N un parámetro definido en el programa.
Ejercicio 6: Enviar Cadenas y Contar Caracteres

Descripción:
El cliente introduce cadenas de texto hasta introducir un asterisco (*). Las cadenas se envían a un servidor que devuelve el número de caracteres de cada cadena. El servidor finaliza al recibir un asterisco.
Boletín 2: Sockets
Ejercicio 1: Información de Profesores

Descripción:
Se definen clases para Asignatura, Especialidad y Profesor. El servidor inicializa un array de 5 objetos de tipo Profesor. Acepta conexiones de clientes en un bucle infinito, asignando un id incremental a cada cliente. El cliente introduce un idProfesor para consultar y recibe el objeto Profesor correspondiente.
Ejercicio 2: Sockets UDP y Cadena en Mayúsculas

Descripción:
El cliente envía texto escrito desde la entrada estándar al servidor, el cual lo devuelve en mayúsculas. El cliente finaliza al introducir un asterisco. Se establece un tiempo de espera con setSoTimeout y se maneja la excepción InterruptedIOException si no se reciben datos en 5000 ms.
Ejercicio 3: Enviar y Recibir Objetos Numeros

Descripción:
Se define una clase Numeros con atributos numero, cuadrado y cubo. El cliente introduce un número, inicializa un objeto Numeros y lo envía al servidor, el cual calcula el cuadrado y el cubo, y devuelve el objeto. El cliente muestra los resultados. El servidor finaliza si recibe un número <= 0.
Ejercicio 4: UDP y Objeto Persona

Descripción:
El cliente envía un objeto Persona inicializado al servidor, el cual modifica los datos del objeto y lo devuelve al cliente. Los datos se visualizan tanto en el cliente como en el servidor.
Ejercicio 5: UDP y Consultas de Alumnos

Descripción:
Se definen clases Curso y Alumno. El servidor inicializa un array de 5 objetos Alumno. El cliente solicita un idAlumno y recibe el objeto correspondiente. El cliente recoge datos hasta recibir un asterisco. Si el idAlumno no está registrado, el servidor devuelve un objeto Alumno con datos vacíos.
Ejercicio 6: Servidor Multihilo

Descripción:
El servidor escucha en el puerto 12345. Cada vez que se conecta un cliente, se crea un nuevo hilo para atenderlo. Se muestran en la consola del servidor la dirección IP y el puerto remoto del cliente. Se notifica cuando un cliente se desconecta. El hilo que atiende al cliente devuelve las cadenas recibidas en mayúsculas mientras no sean "*".
