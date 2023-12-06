##### Comandos básicos de la terminal Unix (terminal de Mac o Ubuntu)

###### Comandos básicos
cd: para navegar hacia un directorio 
history: muestra el historial de comandos escritos 
rm [filename]: elimina un archivo con dicho nombre
vim [filename]: abre un archivo con el nombre indicado del
ls: muestra los archivos que se encuentran en esa ruta
touch [filename]:crea un archivo 
git init: inicializa un repositorio de git
git add. : agrega todos los cambios nuevos en nuestra maquina local 
git commit -m [mensaje] : guarda un cambio en el repositorio para subirlo a la nube
git push: sube los cambios al cliente remoto

###### De administración de procesos para Ubuntu
ps -aux: muestra los procesos en ejecución
ps -U [usuario]: muestra los procesos asignados al usuario
pgrep VBoxClient: retorna el ID de los procesos cuyo nombre coincida con la expresion regular
pgrep -l VBoxClient: muestra el identificador del proceso y el nombre
top: top y htop listan los procesos en tiempo real con una serie de atributos
kill pid [identificador]: mata un proceso con un identificador que se le asigne 

##### Dispositivos de entrada y salida 
De entrada: dispositivos que permiten ingresar datos desde el exterior; teclado, mouse, micrófono, cámara, etc. 
De salida: dispositivos que dan como respuesta la información interior hacia el exterior; impresora, audífonos, bocinas, monitores, etc.

##### Procesos
Un proceso es la ejecución de un programa individual, siguiendo una serie de instrucciones a través del procesador. Un proceso cuenta con las siguientes características básicas: 
- Identificador: distintivo único de cada proceso
- Estado: indica si está en estado de ejecución (nuevo, listo, en ejecución, bloqueado, zombie, terminado )
- Prioridad: nivel relativo de prioridad en comparación a otros procesos

###### Criterios de planificación 
Tiempo de respuesta: tiempo transcurrido desde que se emite una solicitud hasta que se comienza a recibir respuesta
Tiempo de retorno: tiempo transcurrido desde que se lanza un proceso, hasta que se finaliza.
Plazos: plazos específicos de terminación para un proceso. 

##### Ejemplos de algoritmos de planeación
¿Que es la planificación de procesos? una herramienta para que un sistema operativo determine el orden en que un procesador va ejecutando diferentes procesos según sus propias políticas.

###### First Come First Serve (FCFS)
Algoritmo que da prioridad de ejecución al primer proceso en fila.
Tiempo de retorno = tiempo para completarse - tiempo de llegada
Burst time: tiempo que tomará completar el proceso (de manera individual)
Tiempo de espera = tiempo de retorno - burst time

###### Shortest Job First (SJF)
Algoritmo que da prioridad de ejecución al proceso con menor burst time en fila.
Tiempo de espera= tiempo de inicio - tiempo de llegada

###### Round Robin 
Algoritmo que designa un determinado tiempo de ejecución (llamado quantum) para llevar cada proceso en diferentes rondas (hasta que cada uno se termine de ejecutar).
Quantum total: suma de cada ejecución de proceso (contando todas las rondas hasta la finalización de los procesos)
