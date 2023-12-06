# Unidades de almacenamiento 

![Almacenamiento](https://i.blogs.es/7bcfa4/almacenamiento/650_1200.jpg)

Muchos dispositivos electronicos trabajan con estas unidades de almacenamiento dentro de las cuales encontramos:
   * Disco duro
   * CD
   * PENDRIVE
   * TARJETA SD

## Unidades de capacidad

La unidad minima o básica es el bit y se representa por la letra b, simplemente es un 0 o 1.

El Byte (B) es la primera unidad de almacenamiento que tiene sentido, un Byte es aproximadamente un caracter.

![Capacidad](https://img.genial.ly/5f342e64f358d40f98d151ba/9d8a8955-1a2c-4f7f-914b-4ea7b253e6a7.png)

# Jerarquía de memoria 

![Jerarquía](https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Jerarquia_memoria.png/450px-Jerarquia_memoria.png)

La jerarquía de memoria en un sistema computacional se refiere a la organización de diferentes niveles de almacenamiento, desde los más rápidos y cercanos al procesador hasta los más lentos pero de mayor capacidad. La idea es proporcionar un equilibrio entre la velocidad de acceso a los datos y la capacidad de almacenamiento.

## Tipos de memorias 

1. **Memoria RAM (Random Access Memory)**

   - **Tipo:**
     - Volátil (La información se pierde cuando se apaga la computadora)
   - **Características:**
     - Muy rápida, de acceso temporal, directamente accesible por la CPU.
   - **Propósito:**
     - Proporcionar acceso rápido y temporal a datos e instrucciones.
     - Facilitar la multitarea y mejorar el rendimiento general del sistema.

2. **Disco Duro (HDD) / Unidad de Estado Sólido (SSD)**

   - **Tipo:**
     - No volátil (La información se mantiene incluso cuando la computadora está apagada)
   - **Características:**
     - HDD: Utiliza platos magnéticos, más lento pero generalmente más barato y con mayor capacidad.
     - SSD: Utiliza memoria flash, más rápido, duradero y caro.
   - **Propósito:**
     - HDD: Almacenar grandes cantidades de datos de forma permanente.
     - SSD: Proporcionar acceso rápido y duradero al almacenamiento permanente.

3. **Memoria Caché**

   - **Tipo:**
     - Volátil
   - **Características:**
     - Muy rápida, ubicada cerca o dentro de la CPU, más pequeña que la RAM.
   - **Propósito:**
     - Almacenar temporalmente datos e instrucciones para acelerar el acceso y mejorar la eficiencia del sistema.

4. **Memoria Virtual**

   - **Tipo:**
     - Volátil y no volátil
   - **Características:**
     - Más lenta que la RAM, permite ejecutar más aplicaciones simultáneamente.
   - **Propósito:**
     - Ampliar la capacidad de la memoria RAM utilizando una parte del disco duro.

5. **Memoria de Registros**

   - **Tipo:**
     - Volátil
   - **Características:**
     - Muy rápidos, capacidad muy limitada, dentro de la CPU.
   - **Propósito:**
     - Almacenar temporalmente datos e instrucciones para operaciones inmediatas.

6. **Memoria ROM (Read-Only Memory)**

   - **Tipo:**
     - No volátil
   - **Características:**
     - Solo lectura o difícil de reescribir, persistente.
   - **Propósito:**
     - Almacenar firmware y software básico necesario para el arranque y funciones críticas del sistema.

7. **Memoria Flash**

   - **Tipo:**
     - No volátil
   - **Características:**
     - Rápida, portátil, regrabable.
   - **Propósito:**
     - Proporcionar almacenamiento regrabable, duradero y portátil.

8. **Tarjetas de Memoria (Ejemplo: SD, microSD)**

   - **Tipo:**
     - No volátil
   - **Características:**
     - Tamaño compacto, regrabable, portátil.
   - **Propósito:**
     - Ofrecer almacenamiento portátil y expansible para dispositivos móviles.

## ¿Por qué necesitamos una Jerarquía de Memoria?

- Si la memoria es muy rápida → Es pequeña y cara
- Si la memoria es muy grande → Barata y lenta
- Si la memoria tiene un coste razonable → Grande y lenta

# Virtualización del  CPU

La virtualización del CPU permite que un solo procesador físico ejecute múltiples sistemas operativos y aplicaciones simultáneamente. En lugar de dedicar un procesador completo a una tarea, la virtualización divide los recursos del procesador entre varias máquinas virtuales (VM). Cada máquina virtual actúa como un entorno independiente con su propio sistema operativo y aplicaciones.

## Ejemplo

Ejecutar varias instancias del programa cpu.c al mismo tiempo para ilustrar la virtualización de la CPU.

    ./cpu A & ./cpu B & ./cpu C & ./cpu D

# Virtualización de la Memoria

La virtualización de la memoria es un concepto que permite crear entornos virtuales para gestionar y optimizar el uso de la memoria en sistemas computacionales ,es decir, la virtualización de la memoria se enfoca en administrar el espacio de memoria disponible.

## Ejemplo

Demuestra cómo la virtualización de la memoria permite la ejecución simultánea de múltiples instancias de un programa sin interferencia directa en sus respectivos espacios de memoria.

    ./mi_programa & ./mi_programa & ./mi_programa & ./mi_programa

# Localidad temporal

![Temporal](data:image/png;base64,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)

# Localidad espacial

![Temporal](data:image/png;base64,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)

# Tipos de Sistemas de Archivos:

- FAT (File Allocation Table): Antiguo y simple, pero menos eficiente con archivos grandes. Utilizado en memorias USB y tarjetas SD.
- NTFS (New Technology File System): Utilizado por Windows, soporta grandes capacidades de almacenamiento.
- APFS (Apple File System): Más reciente, utilizado por dispositivos Apple, optimizado para SSD y tiene mejor rendimiento y seguridad.
- Btrfs (B-tree filesystem): Sistema de archivos de Linux diseñado para la gestión de los sistemas de almacenamiento de gran tamaño.

# Estructuras de Directorios:

- Jerárquica: Los archivos se organizan en una estructura de árbol, con directorios 
que pueden contener subdirectorios y archivos.
- Plana: Todos los archivos están en el mismo nivel, sin directorios o subdirectorios

# Concurrencia

La concurrencia permite ejecutar múltiples procesos o hilos simultáneamente, maximizando la utilización de recursos. Es esencial para sistemas multitarea, aunque introduce desafíos de sincronización.

**Ejemplo:**

- Sistema Operativo Multitarea: Permite ejecutar varias aplicaciones al mismo tiempo, mejorando la eficiencia y la experiencia del usuario.

# Persistencia

La persistencia conserva datos a lo largo del tiempo, incluso después de cerrar o reiniciar un sistema. Fundamental para aplicaciones que necesitan retener información.

**Ejemplo:**

- Cookies en Navegadores Web: Guardan información en el lado del cliente para mantener el estado entre sesiones.

# Pioneros en la Historia de los Sistemas Operativos

## Linus Torvalds

![Linus](https://i.blogs.es/7c0ad8/torvadls1/450_1000.jpg)

Linus Torvalds, nacido el 28 de diciembre de 1969 en Helsinki, Finlandia, es un ingeniero de software y programador reconocido por ser el creador del kernel de Linux. En 1991, mientras estudiaba en la Universidad de Helsinki, inició el desarrollo de Linux como un proyecto personal. La decisión de Torvalds de lanzar Linux como software de código abierto permitió que se convirtiera en una pieza fundamental de muchos sistemas operativos, desde distribuciones de servidores hasta sistemas integrados y dispositivos móviles.

### Contribuciones Destacadas:

- Desarrollo del kernel de Linux, un componente esencial de los sistemas operativos basados en Linux.
- Fomento del modelo de desarrollo de código abierto, promoviendo la colaboración y contribución de la comunidad.

## Denis Ritchie

![Ritchie](https://i0.wp.com/imgs.hipertextual.com/wp-content/uploads/2011/10/Dennis_Ritchie.jpg?fit=800%2C827&quality=50&strip=all&ssl=1)

Denis Ritchie (9 de septiembre de 1941 - 12 de octubre de 2011) fue un científico de la computación estadounidense y co-creador del sistema operativo Unix. Trabajando en los laboratorios Bell de AT&T en la década de 1970, Ritchie y Ken Thompson desarrollaron Unix, que se convirtió en un sistema operativo influyente en el mundo de la informática. Además, Ritchie desempeñó un papel clave en la creación del lenguaje de programación C, que se convirtió en un pilar en el desarrollo de software.

### Contribuciones Destacadas:

- Co-desarrollo del sistema operativo Unix, que influyó en muchos sistemas operativos modernos.
- Co-creación del lenguaje de programación C, fundamental en el desarrollo de software de sistemas.

## Guido van Rossum

![Rossum](https://gvanrossum.github.io/images/guido-headshot-2019.jpg)

Guido van Rossum, nacido el 31 de enero de 1956 en La Haya, Países Bajos, es un programador de computadoras y el creador del lenguaje de programación Python. Van Rossum inició el desarrollo de Python en la década de 1980, y el lenguaje se ha convertido en uno de los más populares y versátiles en la programación moderna.

### Contribuciones Destacadas:

- Creación del lenguaje de programación Python, conocido por su legibilidad y facilidad de uso.
- Liderazgo en la comunidad de Python y promoción de prácticas de desarrollo colaborativo.

# Instalación de Linux

![Rossum](https://upload.wikimedia.org/wikipedia/commons/d/dd/Linux_logo.jpg)

## Requisitos:

- Computadora compatible con Linux.
- USB de al menos 8 GB.
- Conexión a Internet.

## Pasos:

1. **Descargar Linux:**
   - Elija una distribución y descargue la imagen ISO.

2. **Crear USB de Arranque:**
   - Use Rufus (Windows) o dd (Linux) para crear un USB de arranque.

3. **Arrancar desde USB:**
   - Reinicie y seleccione el USB como dispositivo de inicio.

4. **Iniciar Instalación:**
   - Siga las instrucciones en pantalla para configurar.

5. **Particionar el Disco:**
   - Configure las particiones según sus necesidades.

6. **Crear Cuenta:**
   - Proporcione datos para la cuenta de usuario.

7. **Completar la Instalación:**
   - Reinicie y retire el USB.

8. **Actualizar y Personalizar:**
   - Actualice y personalice según sus preferencias.

# Instalación de macOS

![Rossum](https://cdn-icons-png.flaticon.com/512/2/2235.png)

## Requisitos:

- Mac compatible con la nueva versión.
- Respaldo de datos.

## Pasos:

1. **Verificar Compatibilidad:**
   - Asegúrese de que su Mac sea compatible.

2. **Realizar Respaldo:**
   - Use Time Machine para hacer un respaldo.

3. **Descargar Nueva Versión:**
   - Desde la App Store, descargue la nueva versión de macOS.

4. **Iniciar Instalación:**
   - Abra el instalador y siga las instrucciones.

5. **Configurar Preferencias:**
   - Elija idioma, zona horaria y preferencias.

6. **Seleccionar Disco:**
   - Especifique el disco de instalación.

7. **Esperar la Instalación:**
   - El proceso tomará tiempo.

8. **Configuración Inicial:**
   - Configure su cuenta y preferencias.

9. **Restaurar Datos:**
   - Use Time Machine para restaurar datos.