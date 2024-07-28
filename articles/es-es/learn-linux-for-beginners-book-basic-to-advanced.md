---
title: "Aprende Linux para Principiantes: Desde lo Básico hasta Técnicas Avanzadas [Libro Completo]"
date: 2024-07-24T10:32:46.639Z
author: Zaira Hira
authorURL: https://www.freecodecamp.org/news/author/zaira/
OriginalURL: https://www.freecodecamp.org/news/learn-linux-for-beginners-book-basic-to-advanced/
Proofreader: ""

---

Aprender Linux es una de las habilidades más valiosas en la industria tecnológica. Puede ayudarte a hacer las cosas más rápido y de manera más eficiente. Muchos de los servidores y supercomputadoras más poderosos del mundo funcionan con Linux.

<!-- more -->

Además de empoderarte en tu rol actual, aprender Linux también puede ayudarte a hacer la transición a otras carreras tecnológicas como DevOps, Ciberseguridad y Computación en la Nube.

En este manual, aprenderás los conceptos básicos de la línea de comandos de Linux, y luego pasarás a temas más avanzados como la escritura de scripts en shell y la administración de sistemas. Ya sea que seas nuevo en Linux o lo hayas estado utilizando durante años, este libro tiene algo para ti.

Nota Importante: Todos los ejemplos en este libro se demuestran en Ubuntu 22.04.2 LTS (Jammy Jellyfish). La mayoría de las herramientas de línea de comandos son más o menos iguales en otras distribuciones. Sin embargo, algunas aplicaciones y comandos de interfaz gráfica pueden diferir si trabajas con otra distribución de Linux.

## Tabla de Contenidos

-   [Parte 1: Introducción a Linux][1]
    
    -   [1.1. Empezando con Linux][2]
-   [Parte 2: Introducción a Bash Shell y Comandos del Sistema][3]
    
    -   [2.1. Empezando con el shell Bash][4]
        
    -   [2.2. Estructura de Comandos][5]
        
    -   [2.3. Comandos de Bash y Atajos de Teclado][6]
        
    -   [2.4. Identificándote: El Comando `whoami`][7]
        
-   [Parte 3: Entendiendo tu Sistema Linux][8]
    
    -   [3.1. Descubriendo tu SO y Especificaciones][9]
-   [Parte 4: Gestionando Archivos desde la Línea de Comandos][10]
    
    -   [4.1. La Jerarquía del Sistema de Archivos de Linux][11]
        
    -   [4.2. Navegando el Sistema de Archivos de Linux][12]
        
    -   [4.3. Gestionando Archivos y Directorios][13]
        
    -   [4.5. Comandos Básicos para Ver Archivos][14]
        
-   [Parte 5: Lo Esencial de la Edición de Texto en Linux][15]
    
    -   [5.1. Dominando Vim: La Guía Completa][16]
        
    -   [5.2. Dominando Nano][17]
        
-   [Parte 6: Escritura de Scripts en Bash][18]
    
    -   [6.1. Definición de la Escritura de Scripts en Bash][19]
        
    -   [6.2. Ventajas de la Escritura de Scripts en Bash][20]
        
    -   [6.3. Resumen del Shell Bash y la Interfaz de Línea de Comandos][21]
        
    -   [6.4. Cómo Crear y Ejecutar Scripts en Bash][22]
        
    -   [6.5. Conceptos Básicos de la Escritura de Scripts en Bash][23]
        
-   [Parte 7: Gestionando Paquetes de Software en Linux][24]
    
    -   [7.1. Paquetes y Gestión de Paquetes][25]
        
    -   [7.2. Instalación de un Paquete vía Línea de Comandos][26]
        
    -   [7.3. Instalación de un Paquete vía Método Gráfico Avanzado – Synaptic][27]
        
    -   [7.4. Instalación de Paquetes Descargados de un Sitio Web][28]
        
-   [Parte 8: Temas Avanzados de Linux][29]
    
    -   [8.1. Gestión de Usuarios][30]
        
    -   [8.2. Conexión a Servidores Remotos vía SSH][31]
        
    -   [8.3. Análisis y Parsing Avanzado de Registros][32]
        
    -   [8.4. Gestionando Procesos de Linux vía Línea de Comandos][33]
        
    -   [8.5. Flujo de Entrada y Salida Estándar en Linux][34]
        
    -   [8.6. Automatización en Linux – Automatizar Tareas con Cron Jobs][35]
        
    -   [8.7. Fundamentos de Redes en Linux][36]
        
    -   [8.8. Solución de Problemas en Linux: Herramientas y Técnicas][37][8.9. Estrategia General de Solución de Problemas para Servidores][38]
        
-   [Conclusión][39]
    

## Parte 1: Introducción a Linux

### 1.1. Empezando con Linux

#### ¿Qué es Linux?

Linux es un sistema operativo de código abierto que está basado en el sistema operativo Unix. Fue creado por Linus Torvalds en 1991.

El código abierto significa que el código fuente del sistema operativo está disponible para el público. Esto permite que cualquiera pueda modificar el código original, personalizarlo y distribuir el nuevo sistema operativo a posibles usuarios.

#### ¿Por qué deberías aprender sobre Linux?

En el panorama actual de los centros de datos, Linux y Microsoft Windows destacan como los principales contendientes, con Linux teniendo una participación mayoritaria.

Aquí hay varias razones convincentes para aprender Linux:

-   Dada la prevalencia del alojamiento Linux, hay una alta probabilidad de que tu aplicación sea alojada en Linux. Así que aprender Linux como desarrollador se vuelve cada vez más valioso.
    
-   Con la computación en la nube convirtiéndose en la norma, las probabilidades son altas de que tus instancias en la nube dependerán de Linux.
    
-   Linux sirve como la base para muchos sistemas operativos para el Internet de las Cosas (IoT) y aplicaciones móviles.
    
-   En IT, hay muchas oportunidades para aquellos capacitados en Linux.
    

#### ¿Qué significa que Linux sea un sistema operativo de código abierto?

Primero, ¿qué es el código abierto? El software de código abierto es software cuyo código fuente es libremente accesible, permitiendo que cualquiera lo utilice, modifique y distribuya.

Siempre que se crea un código fuente, automáticamente se considera protegido por derechos de autor, y su distribución está gobernada por el titular de los derechos a través de licencias de software.

En contraste con el código abierto, el software propietario o de código cerrado restringe el acceso a su código fuente. Solo los creadores pueden verlo, modificarlo o distribuirlo.

Este enfoque colaborativo ha llevado a la adopción generalizada de Linux en servidores, escritorios, sistemas embebidos y dispositivos móviles.

El aspecto más interesante de Linux al ser de código abierto es que cualquiera puede adaptar el sistema operativo a sus necesidades específicas sin estar restringido por limitaciones propietarias.

Chrome OS utilizado por Chromebooks está basado en Linux. Android, que impulsa muchos teléfonos inteligentes a nivel mundial, también está basado en Linux.

**¿Qué es un kernel de Linux?**

El kernel es el componente central de un sistema operativo que gestiona la computadora y sus operaciones de hardware. Maneja operaciones de memoria y tiempo de CPU.

El kernel actúa como un puente entre aplicaciones y el procesamiento de datos a nivel de hardware utilizando comunicación entre procesos y llamadas al sistema.

El kernel se carga en la memoria primero cuando se inicia un sistema operativo y permanece allí hasta que el sistema se apaga. Es responsable de tareas como la gestión de discos, gestión de tareas y gestión de memoria.

![Diseño del Kernel de Linux mostrando la interacción del kernel con aplicaciones y el sistema operativo](https://cdn.hashnode.com/res/hashnode/image/upload/v1719844849011/f4bb226e-f319-4cb5-bfc9-c1a80401123e.png)

Si tienes curiosidad sobre cómo se ve el kernel de Linux, [aquí][40] está el enlace a GitHub.

#### ¿Qué es una distribución de Linux?

A este punto, sabes que puedes reutilizar el código del kernel de Linux, modificarlo y crear un nuevo kernel. Puedes combinar diferentes utilidades y software para crear un sistema operativo completamente nuevo.

Una distribución de Linux o distro es una versión del sistema operativo Linux que incluye el kernel de Linux, utilidades del sistema y otro software. Al ser de código abierto, una distribución de Linux es un esfuerzo colaborativo que involucra múltiples comunidades independientes de desarrollo de código abierto.

**¿Qué significa que una distribución sea derivada?** Cuando dices que una distribución es "derivada" de otra, la distro más nueva se basa en la base o el fundamento de la distro original. Esta derivación puede incluir el uso del mismo sistema de gestión de paquetes (más sobre esto más adelante), versión del kernel y, a veces, las mismas herramientas de configuración.

Hoy en día, existen miles de distribuciones de Linux para elegir, que ofrecen diferentes objetivos y criterios para seleccionar y soportar el software proporcionado por su distribución.

Las distribuciones varían de una a otra, pero en general tienen varias características comunes:

-   Una distribución consiste en un kernel de Linux.
    
-   Soporta programas en espacio de usuario.
    
-   Una distribución puede ser pequeña y de un solo propósito o incluir miles de programas de código abierto.
    
-   Se debe proporcionar algún medio para instalar y actualizar la distribución y sus componentes.
    

Si ves la [línea de tiempo de distribuciones de Linux][41], verás dos distros principales: Slackware y Debian. Varias distribuciones derivan de ellas. Por ejemplo, Ubuntu y Kali derivan de Debian.

**¿Cuáles son las ventajas de la derivación?** Hay varias ventajas de la derivación. Las distribuciones derivadas pueden aprovechar la estabilidad, seguridad y grandes repositorios de software de la distribución primaria.

Al construir sobre una base existente, los desarrolladores pueden enfocar su atención y esfuerzo completamente en las características especializadas de la nueva distribución. Los usuarios de distribuciones derivadas pueden beneficiarse de la documentación, soporte de la comunidad y recursos ya disponibles para la distribución primaria.

Algunas distribuciones populares de Linux son:

1.  **Ubuntu**: Una de las distribuciones de Linux más utilizadas y populares. Es fácil de usar y recomendada para principiantes. [Más información sobre Ubuntu aquí][42].
    
2.  **Linux Mint**: Basada en Ubuntu, Linux Mint proporciona una experiencia fácil de usar con un enfoque en el soporte multimedia. [Más información sobre Linux Mint aquí][43].
    
3.  **Arch Linux**: Popular entre usuarios experimentados, Arch es una distribución ligera y flexible destinada a usuarios que prefieren un enfoque DIY (hazlo tú mismo). [Más información sobre Arch Linux aquí][44].
    
4.  **Manjaro**: Basada en Arch Linux, Manjaro proporciona una experiencia fácil de usar con software preinstalado y herramientas de gestión del sistema fáciles de usar. [Más información sobre Manjaro aquí][45].
    
5.  **Kali Linux**: Kali Linux proporciona una suite completa de herramientas de seguridad y se enfoca principalmente en ciberseguridad y hacking. [Más información sobre Kali Linux aquí][46].
    

#### Cómo instalar y acceder a Linux

La mejor manera de aprender es aplicar los conceptos a medida que avanzas. En esta sección, aprenderemos cómo instalar Linux en tu máquina para que puedas seguir adelante. También aprenderás cómo acceder a Linux en una máquina con Windows.

Recomiendo que sigas cualquiera de los métodos mencionados en esta sección para obtener acceso a Linux para que puedas seguir adelante.

##### Instalar Linux como el sistema operativo principal

Instalar Linux como el sistema operativo principal es la forma más eficiente de usar Linux, ya que puedes aprovechar todo el poder de tu máquina.

En esta sección, aprenderás cómo instalar Ubuntu, que es una de las distribuciones de Linux más populares. He omitido otras distribuciones por ahora, ya que quiero mantener las cosas simples. Siempre puedes explorar otras distribuciones una vez que te sientas cómodo con Ubuntu.

¡Y ahí lo tienes! Ahora puedes instalar aplicaciones y personalizar tu escritorio.

![Pantalla del escritorio de Ubuntu 22.04.4 LTS](https://cdn.hashnode.com/res/hashnode/image/upload/v1719304547967/d150c6eb-d04e-47e0-8473-d1a837df45c4.png)

Para una instalación avanzada, puedes explorar los siguientes temas:

-   Particionamiento de disco.
    
-   Configuración de la memoria de intercambio (swap) para habilitar la hibernación.
    

**Acceder al terminal**

Una parte importante de este manual es aprender sobre el terminal donde ejecutarás todos los comandos y verás cómo sucede la magia. Puedes buscar el terminal presionando la tecla "Windows" y escribiendo "terminal". Puedes anclar el Terminal en el dock donde se encuentran otras aplicaciones para un acceso fácil.

![Resultados de búsqueda para "terminal"](https://cdn.hashnode.com/res/hashnode/image/upload/v1719305113272/4dd30c5e-da73-4cd4-86bb-7dcd8cd2084c.png)

> 💡 El atajo para abrir el terminal es `ctrl+alt+t`

También puedes abrir el terminal desde dentro de una carpeta. Haz clic derecho donde estés y selecciona "Abrir en el Terminal". Esto abrirá el terminal en la misma ruta.

![Abrir el terminal con el menú del clic derecho](https://cdn.hashnode.com/res/hashnode/image/upload/v1719305289021/284a4a53-2d1a-4eaa-925a-1002a32c1dce.png)

##### Cómo usar Linux en una máquina con Windows

A veces, podrías necesitar ejecutar tanto Linux como Windows uno al lado del otro. Afortunadamente, hay algunas maneras de obtener lo mejor de ambos mundos sin tener computadoras diferentes para cada sistema operativo.

En esta sección, explorarás algunas formas de usar Linux en una máquina con Windows. Algunas de ellas son basadas en navegador o en la nube y no necesitan ninguna instalación de SO antes de usarlas.

**Opción 1: "Arranque dual" Linux + Windows** Con el arranque dual, puedes instalar Linux junto con Windows en tu computadora, permitiéndote elegir qué sistema operativo usar al inicio.

Esto requiere particionar tu disco duro e instalar Linux en una partición separada. Con este enfoque, solo puedes usar un sistema operativo a la vez.

**Opción 2: Utilizar Windows Subsystem for Linux (WSL)** El Subsistema de Windows para Linux proporciona una capa de compatibilidad que te permite ejecutar ejecutables binarios de Linux de manera nativa en Windows.

Utilizar WSL tiene algunas ventajas. La configuración de WSL es simple y no consume mucho tiempo. Es ligero en comparación con las máquinas virtuales donde tienes que asignar recursos desde la máquina anfitriona. No necesitas instalar ninguna ISO o imagen de disco virtual para máquinas Linux, que tienden a ser archivos pesados. Puedes usar Windows y Linux uno al lado del otro.

**Cómo instalar WSL2**

Primero, habilita el Subsistema de Windows para Linux en la configuración.

-   Ve a Inicio. Busca "Activar o desactivar las características de Windows."
    
-   Marca la opción "Subsystem for Linux" si no está ya marcada.
    
    ![Seleccionar la opción "Subsystem for Linux" en las características de Windows](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306102095/84f23bae-faa5-4ece-a9b6-e40f8789a061.png)
    
-   Luego, abre tu símbolo del sistema y proporciona los comandos de instalación.
    
-   Abre el Símbolo del sistema como administrador:
    
    ![Ejecutando el símbolo del sistema como administrador, haciendo clic derecho en la app y eligiendo "ejecutar como administrador"](https://cdn.hashnode.com/res/hashnode/image/upload/v1720451480640/6052c9b4-cf07-47e0-ae89-18c3a2d3e385.png)
    
-   Ejecuta el siguiente comando:
    

```
wsl --install
```

Este es el resultado:

![Progreso de descarga de Ubuntu](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306131053/b7272031-ddb7-4e04-8d7b-bafc0911da04.png)

Nota: Por defecto, se instalará Ubuntu.

![Ubuntu instalado por defecto usando WSL](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306144861/a01f95df-1d95-4b79-bff9-08759be0d3dc.png)

-   Una vez que la instalación esté completa, necesitarás reiniciar tu máquina con Windows. Por lo tanto, reinicia tu máquina con Windows.

Después de reiniciar, podrías ver una ventana como esta:

![Ventana que se muestra después de un reinicio](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306157704/15620fbe-59d1-40da-9cd6-119a1fab0802.png)

Una vez que la instalación de Ubuntu esté completa, se te pedirá que ingreses tu nombre de usuario y contraseña.

![Usuario solicitando un nombre de usuario y una contraseña](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306167380/5e3058cd-b7a1-45b1-a16d-c23b5a451504.png)

¡Y eso es todo! Ya estás listo para usar Ubuntu.

Lanza Ubuntu buscándolo desde el menú de inicio.

![Lanzando Ubuntu desde el menú de inicio](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306185110/77c17856-08ac-4ec7-9380-5b06f93be095.png)

Y aquí tenemos tu instancia de Ubuntu lanzada.

![Instalación exitosa de Ubuntu usando WSL](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306196320/13be3a71-5b40-440c-a6bf-d742e5b5934b.png)

**Opción 3: Utilizar una Máquina Virtual (VM)**

Una máquina virtual (VM) es una emulación de software de un sistema informático físico. Te permite ejecutar múltiples sistemas operativos y aplicaciones en una sola máquina física simultáneamente.

Puedes usar software de virtualización como Oracle VirtualBox o VMware para crear una máquina virtual ejecutando Linux dentro de tu entorno Windows. Esto te permite ejecutar Linux como un sistema operativo invitado junto con Windows.

Aquí tienes la traducción del archivo al español manteniendo el formato y la disposición del archivo original en markdown:

Here are some of the common options available for virtualization:

-   [Oracle virtual box][49]
    
-   [Multipass][50]
    
-   [VMware workstation player][51]
    

**Opción 4: Usar una solución basada en el navegador**

Las soluciones basadas en el navegador son particularmente útiles para pruebas rápidas, aprendizaje o acceso a entornos Linux desde dispositivos que no tienen Linux instalado.

Puedes usar editores de código en línea o terminales basadas en la web para acceder a Linux. Ten en cuenta que generalmente no tienes privilegios de administración completos en estos casos.

#### **Editores de código en línea**

Los editores de código en línea ofrecen editores con terminales Linux integradas. Aunque su propósito principal es la codificación, también puedes utilizar la terminal de Linux para ejecutar comandos y realizar tareas.

[Replit][52] es un ejemplo de un editor de código en línea, donde puedes escribir tu código y acceder al shell de Linux al mismo tiempo.

![Ejecutando scripts y un shell bash en Replit](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306257260/d85d5541-b78f-4c8b-99a8-dbd8c097f661.gif)

#### **Terminales Linux basadas en la web:**

Las terminales Linux en línea te permiten acceder a una interfaz de línea de comandos de Linux directamente desde tu navegador. Estas terminales proporcionan una interfaz basada en la web a un shell de Linux, permitiéndote ejecutar comandos y trabajar con utilidades de Linux.

Un ejemplo es [JSLinux][53]. La captura de pantalla a continuación muestra un entorno Linux listo para usar:

![Usando JSLinux para acceder a la terminal de Linux](https://cdn.hashnode.com/res/hashnode/image/upload/v1719306276915/ddaabfc3-9a20-43b2-bedc-0af6875d2008.png)

**Opción 5: Usar una solución basada en la nube**

En lugar de ejecutar Linux directamente en tu máquina con Windows, puedes considerar usar entornos Linux basados en la nube o servidores privados virtuales (VPS) para acceder y trabajar con Linux de forma remota.

Servicios como Amazon EC2, Microsoft Azure o DigitalOcean proporcionan instancias de Linux a las que puedes conectarte desde tu computadora con Windows. Ten en cuenta que algunos de estos servicios ofrecen niveles gratuitos, pero generalmente no son gratuitos a largo plazo.

## Parte 2: Introducción al Bash Shell y Comandos del Sistema

### 2.1. Empezando con el Bash shell

#### Introducción al bash shell

La línea de comandos de Linux es proporcionada por un programa llamado el shell. Con el tiempo, el programa shell ha evolucionado para ofrecer varias opciones.

Diferentes usuarios pueden configurarse para usar diferentes shells. Pero, la mayoría de los usuarios prefieren quedarse con el shell predeterminado actual. El shell predeterminado para muchas distribuciones de Linux es el GNU Bourne-Again Shell (`bash`). Bash es el sucesor del Bourne shell (`sh`).

Para averiguar tu shell actual, abre tu terminal y escribe el siguiente comando:

```
echo $SHELL
```

Desglose del comando:

-   El comando `echo` se utiliza para imprimir en la terminal.
    
-   El `$SHELL` es una variable especial que contiene el nombre del shell actual.
    

En mi configuración, el resultado es `/bin/bash`. Esto significa que estoy usando el bash shell.

```
# salida
echo $SHELL
/bin/bash
```

Bash es muy poderoso ya que puede simplificar ciertas operaciones que son difíciles de lograr de manera eficiente con una GUI (o Interfaz Gráfica de Usuario). Recuerda que la mayoría de los servidores no tienen una GUI, y es mejor aprender a usar los poderes de una interfaz de línea de comandos (CLI).

**Terminal vs Shell**

Los términos "terminal" y "shell" a menudo se usan indistintamente, pero se refieren a diferentes partes de la interfaz de línea de comandos.

La terminal es la interfaz que usas para interactuar con el shell. El shell es el intérprete de comandos que procesa y ejecuta tus comandos. Aprenderás más sobre shells en la Parte 6 del manual.

#### ¿Qué es un prompt?

Cuando se usa un shell de forma interactiva, muestra un `$` cuando está esperando un comando del usuario. Esto se llama el prompt del shell.

`[usuario@host ~]$`

Si el shell se está ejecutando como `root` (aprenderás más sobre el usuario root más adelante), el prompt se cambia a `#`.

`[root@host ~]#`

### 2.2. Estructura de Comandos

Un comando es un programa que realiza una operación específica. Una vez que tengas acceso al shell, puedes introducir cualquier comando después del signo `$` y ver el resultado en la terminal.

Generalmente, los comandos de Linux siguen esta sintaxis:

```
comando [opciones] [argumentos]
```

Aquí está el desglose de la sintaxis anterior:

-   `comando`: Este es el nombre del comando que deseas ejecutar. `ls` (listar), `cp` (copiar) y `rm` (eliminar) son comandos comunes de Linux.
    
-   `[opciones]`: Las opciones, o banderas, a menudo precedidas por un guion (-) o doble guion (--), modifican el comportamiento del comando. Pueden cambiar cómo opera el comando. Por ejemplo, `ls -a` usa la opción `-a` para mostrar archivos ocultos en el directorio actual.
    
-   `[argumentos]`: Los argumentos son las entradas para los comandos que requieren uno. Estos podrían ser nombres de archivos, nombres de usuarios u otros datos sobre los que actuará el comando. Por ejemplo, en el comando `cat access.log`, `cat` es el comando y `access.log` es la entrada. Como resultado, el comando `cat` muestra el contenido del archivo `access.log`.
    

Las opciones y los argumentos no son necesarios para todos los comandos. Algunos comandos pueden ejecutarse sin opciones ni argumentos, mientras que otros pueden requerir uno o ambos para funcionar correctamente. Siempre puedes consultar el manual del comando para verificar las opciones y argumentos que admite.

Puedes acceder a la página del manual para `ls` con `man ls`, y se verá así:

![5b1232a6-8c0b-4a97-86f0-9f15f2e14ed7](https://cdn.hashnode.com/res/hashnode/image/upload/v1719312523336/5b1232a6-8c0b-4a97-86f0-9f15f2e14ed7.png)

Las páginas del manual son una forma excelente y rápida de acceder a la documentación. Recomiendo encarecidamente revisar las páginas del manual para los comandos que usas más frecuentemente.

### 2.3. Comandos de Bash y Atajos de Teclado

Cuando estás en la terminal, puedes acelerar tus tareas usando atajos.

Aquí tienes algunos de los atajos de terminal más comunes:

| Operación | Atajo |
| --- | --- |
| Buscar el comando anterior | Flecha Arriba |
| Saltar al principio de la palabra anterior | Ctrl+FlechaIzquierda |
| Borrar caracteres desde el cursor hasta el final de la línea de comando | Ctrl+K |
| Completar comandos, nombres de archivos y opciones | Presionando Tab |
| Saltar al principio de la línea de comando | Ctrl+A |
| Muestra la lista de comandos anteriores | history |

### 2.4. Identificándote: El Comando `whoami`

Puedes obtener el nombre de usuario con el que has iniciado sesión utilizando el comando `whoami`. Este comando es útil cuando estás cambiando entre diferentes usuarios y quieres confirmar el usuario actual.

Justo después del signo `$`, escribe `whoami` y presiona Enter.

```
whoami
```

Este es el resultado que obtuve.

```
zaira@zaira-ThinkPad:~$ whoami
zaira
```

## Parte 3: Entendiendo Tu Sistema Linux

### 3.1. Descubriendo Tu SO y Especificaciones

#### Imprimir información del sistema usando el Comando `uname`

Puedes obtener información detallada del sistema con el comando `uname`.

Cuando proporcionas la opción `-a`, imprime toda la información del sistema.

```
uname -a
# salida
Linux zaira 6.5.0-21-generic #21~22.04.1-Ubuntu SMP PREEMPT_DYNAMIC Fri Feb  9 13:32:52 UTC 2 x86_64 x86_64 x86_64 GNU/Linux
```

En la salida anterior,

-   `Linux`: Indica el sistema operativo.
    
-   `zaira`: Representa el nombre del host de la máquina.
    
-   `6.5.0-21-generic #21~22.04.1-Ubuntu SMP PREEMPT_DYNAMIC Fri Feb 9 13:32:52 UTC 2`: Proporciona información sobre la versión del núcleo, la fecha de compilación y algunos detalles adicionales.
    
-   `x86_64 x86_64 x86_64`: Indica la arquitectura del sistema.
    
-   `GNU/Linux`: Representa el tipo de sistema operativo.
    

#### Encontrar detalles de la arquitectura de la CPU usando el Comando `lscpu`

El comando `lscpu` en Linux se utiliza para mostrar información sobre la arquitectura de la CPU. Cuando ejecutas `lscpu` en la terminal, proporciona detalles como:

-   La arquitectura de la CPU (por ejemplo, x86_64)
    
-   Modos de operación de la CPU (por ejemplo, 32-bit, 64-bit)
    
-   Orden de bytes (por ejemplo, Little Endian)
    
-   CPU(s) (número de CPUs), y así sucesivamente
    
    Vamos a intentarlo:
    

```
lscpu
# salida
Architecture:            x86_64
  CPU op-mode(s):        32-bit, 64-bit
  Address sizes:         48 bits physical, 48 bits virtual
  Byte Order:            Little Endian
CPU(s):                  12
  On-line CPU(s) list:   0-11
Vendor ID:               AuthenticAMD
  Model name:            AMD Ryzen 5 5500U with Radeon Graphics
    Thread(s) per core:  2
    Core(s) per socket:  6
    Socket(s):           1
    Stepping:            1
    CPU max MHz:         4056.0000
    CPU min MHz:         400.0000
```

Eso fue mucha información, ¡pero también útil! Recuerda que siempre puedes revisar la información relevante utilizando banderas específicas. Consulta el manual del comando con `man lscpu`.

## Parte 4: Gestionando Archivos desde la Línea de Comandos

### 4.1. La Jerarquía del Sistema de Archivos en Linux

Todos los archivos en Linux están almacenados en un sistema de archivos. Sigue una estructura similar a un árbol invertido porque la raíz está en la parte más alta.

El `/` es el directorio raíz y el punto de inicio del sistema de archivos. El directorio raíz contiene todos los demás directorios y archivos en el sistema. El carácter `/` también sirve como separador de directorios entre nombres de ruta. Por ejemplo, `/home/alice` forma una ruta completa.

La imagen a continuación muestra la jerarquía completa del sistema de archivos. Cada directorio sirve para un propósito específico.

Ten en cuenta que esto no es una lista exhaustiva y que diferentes distribuciones pueden tener diferentes configuraciones.

![Jerarquía del sistema de archivos en Linux](https://cdn.hashnode.com/res/hashnode/image/upload/v1719322457140/02fdbf2c-f4fa-438b-af2f-c23f59f9ddf4.png)

Aquí hay una tabla que muestra el propósito de cada directorio:

| Ubicación | Propósito |
| --- | --- |
| /bin | Binarios de comandos esenciales |
| /boot | Archivos estáticos del gestor de arranque, necesarios para iniciar el proceso de arranque. |
| /etc | Configuración del sistema específica del host |
| /home | Directorios de inicio de los usuarios |
| /root | Directorio de inicio para el usuario administrador root |
| /lib | Bibliotecas compartidas esenciales y módulos del núcleo |
| /mnt | Punto de montaje para montar un sistema de archivos temporalmente |
| /opt | Paquetes de software adicionales |
| /usr | Software instalado y bibliotecas compartidas |
| /var | Datos variables que también son persistentes entre reinicios |
| /tmp | Archivos temporales que son accesibles para todos los usuarios |

💡 **Consejo:** Puedes aprender más sobre el sistema de archivos usando el comando `man hier`.

Puedes revisar tu sistema de archivos utilizando el comando `tree -d -L 1`. Puedes modificar la bandera `-L` para cambiar la profundidad del árbol.

```
tree -d -L 1
# salida
.
├── bin -> usr/bin
├── boot
├── cdrom
├── data
├── dev
├── etc
├── home
├── lib -> usr/lib
├── lib32 -> usr/lib32
├── lib64 -> usr/lib64
├── libx32 -> usr/libx32
├── lost+found
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin -> usr/sbin
├── snap
├── srv
├── sys
├── tmp
├── usr
└── var


Esta lista no es exhaustiva y diferentes distribuciones y sistemas pueden estar configurados de manera diferente.

### 4.2. Navegando el Sistema de Archivos de Linux

#### Ruta absoluta vs ruta relativa

La ruta absoluta es la ruta completa desde el directorio raíz hasta el archivo o directorio. Siempre comienza con un `/`. Por ejemplo, `/home/john/documents`.

La ruta relativa, por otro lado, es la ruta desde el directorio actual hasta el archivo o directorio de destino. No comienza con un `/`. Por ejemplo, `documents/work/project`.

#### Localizando tu directorio actual usando el comando `pwd`

Es fácil perderse en el sistema de archivos de Linux, especialmente si eres nuevo en la línea de comandos. Puedes localizar tu directorio actual usando el comando `pwd`.

Aquí hay un ejemplo:

```
pwd
# salida
/home/zaira/scripts/python/free-mem.py
```

#### Cambiando de directorios usando el comando `cd`

El comando para cambiar de directorios es `cd` y significa "cambiar de directorio". Puedes usar el comando `cd` para navegar hacia un directorio diferente.

Puedes usar una ruta relativa o una ruta absoluta.

Por ejemplo, si quieres navegar en la siguiente estructura de archivos (siguiendo las líneas rojas):

![Ejemplo de estructura de archivos](https://cdn.hashnode.com/res/hashnode/image/upload/v1719389950079/640cce46-6c52-4f38-9787-581747fb9798.png)

y estás en "home", el comando sería así:

```
cd home/bob/documents/work/project
```

Algunos otros atajos de `cd` comúnmente usados son:

| Comando | Descripción |
| --- | --- |
| `cd ..` | Regresar un directorio |
| `cd ../..` | Regresar dos directorios |
| `cd` o `cd ~` | Ir al directorio de inicio |
| `cd -` | Ir a la ruta anterior |

### 4.3. Gestionando Archivos y Directorios

Cuando trabajas con archivos y directorios, puede que quieras copiar, mover, eliminar y crear nuevos archivos y directorios. Aquí hay algunos comandos que pueden ayudarte con eso.

💡**Consejo:** Puedes diferenciar entre un archivo y una carpeta mirando la primera letra en la salida de `ls -l`. Un `'-'` representa un archivo y una `'d'` representa una carpeta.

!["d" representa una carpeta](https://cdn.hashnode.com/res/hashnode/image/upload/v1719390306244/4f1688cd-ded5-43fe-b13a-9ca44ac7c4ad.png)

#### Creando nuevos directorios usando el comando `mkdir`

Puedes crear un directorio vacío usando el comando `mkdir`.

```
# crea un directorio vacío llamado "foo" en la carpeta actual
mkdir foo
```

También puedes crear directorios recursivamente usando la opción `-p`.

```
mkdir -p tools/index/helper-scripts
# salida del árbol
.
└── tools
    └── index
        └── helper-scripts

3 directorios, 0 archivos
```

#### Creando nuevos archivos usando el comando `touch`

El comando `touch` crea un archivo vacío. Puedes usarlo así:

```
# crea el archivo vacío "file.txt" en la carpeta actual
touch file.txt
```

Los nombres de los archivos pueden encadenarse juntos si deseas crear múltiples archivos en un solo comando.

```
# crea los archivos vacíos "file1.txt", "file2.txt", y "file3.txt" en la carpeta actual

touch file1.txt file2.txt file3.txt
```

#### Eliminando archivos y directorios usando los comandos `rm` y `rmdir`

Puedes usar el comando `rm` para eliminar tanto archivos como directorios no vacíos.

| Comando | Descripción |
| --- | --- |
| `rm file.txt` | Elimina el archivo `file.txt` |
| `rm -r directory` | Elimina el directorio `directory` y su contenido |
| `rm -f file.txt` | Elimina el archivo `file.txt` sin pedir confirmación |
| `rmdir directory` | Elimina un directorio vacío |

🛑 Nota que debes usar la opción `-f` con precaución ya que no se te pedirá confirmación antes de eliminar un archivo. También, ten cuidado al ejecutar comandos `rm` en el directorio `root` ya que podría resultar en la eliminación de archivos importantes del sistema.

#### Copiando archivos usando el comando `cp`

Para copiar archivos en Linux, usa el comando `cp`.

-   **Sintaxis para copiar archivos:**`cp archivo_origen destino_archivo`

Este comando copia un archivo llamado `file1.txt` a una nueva ubicación de archivo `/home/adam/logs`.

```
cp file1.txt /home/adam/logs
```

El comando `cp` también crea una copia de un archivo con el nombre proporcionado.

Este comando copia un archivo llamado `file1.txt` a otro archivo llamado `file2.txt` en la misma carpeta.

```
cp file1.txt file2.txt
```

#### Moviendo y renombrando archivos y carpetas usando el comando `mv`

El comando `mv` se utiliza para mover archivos y carpetas de un directorio a otro.

**Sintaxis para mover archivos:**`mv archivo_origen directorio_destino`

**Ejemplo:** Mover un archivo llamado `file1.txt` a un directorio llamado `backup`:

```
mv file1.txt backup/
```

Para mover un directorio y su contenido:

```
mv dir1/ backup/
```

Renombrar archivos y carpetas en Linux también se hace con el comando `mv`.

**Sintaxis para renombrar archivos:**`mv nombre_viejo nombre_nuevo`

**Ejemplo:** Renombrar un archivo de `file1.txt` a `file2.txt`:

```
mv file1.txt file2.txt
```

Renombrar un directorio de `dir1` a `dir2`:

```
mv dir1 dir2
```

### 4.4. Localizando Archivos y Carpetas Usando el Comando `find`

El comando `find` te permite buscar de manera eficiente archivos, carpetas y dispositivos de caracteres y bloques.

A continuación se muestra la sintaxis básica del comando `find`:

```
find /ruta/ -type f -name archivo-a-buscar
```

Donde,

-   `/ruta` es la ruta donde se espera encontrar el archivo. Este es el punto de inicio para buscar archivos. La ruta también puede ser `/` o `.` que representan el directorio raíz y el directorio actual, respectivamente.
    
-   `-type` representa los descriptores de archivo. Pueden ser cualquiera de los siguientes:  
    `f` – **Archivo regular** como archivos de texto, imágenes y archivos ocultos.  
    `d` – **Directorio**. Estos son los directorios bajo consideración.  
    `l` – **Enlace simbólico**. Los enlaces simbólicos apuntan a archivos y son similares a los accesos directos.  
    `c` – **Dispositivos de caracteres**. Los archivos que se utilizan para acceder a dispositivos de caracteres se llaman archivos de dispositivos de caracteres. Los controladores se comunican con dispositivos de caracteres enviando y recibiendo caracteres individuales (bytes, octetos). Ejemplos incluyen teclados, tarjetas de sonido y el ratón.  
    `b` – **Dispositivos de bloques**. Los archivos que se utilizan para acceder a dispositivos de bloques se llaman archivos de dispositivos de bloques. Los controladores se comunican con dispositivos de bloques enviando y recibiendo bloques completos de datos. Ejemplos incluyen USB y CD-ROM
    
-   `-name` es el nombre del tipo de archivo que deseas buscar.

Supongamos que necesitamos encontrar archivos que contengan "style" en su nombre. Usaremos este comando:

```
find . -type f -name "style*"
#output
./style.css
./styles.css
```

Ahora, digamos que queremos encontrar archivos con una extensión particular como `.html`. Modificaremos el comando de esta manera:

```
find . -type f -name "*.html"
# output
./services.html
./blob.html
./index.html
```

#### Cómo buscar archivos ocultos

Un punto al principio del nombre del archivo representa archivos ocultos. Normalmente están ocultos, pero se pueden ver con `ls -a` en el directorio actual.

Podemos modificar el comando `find` como se muestra a continuación para buscar archivos ocultos:

```
find . -type f -name ".*"
```

**Listar y encontrar archivos ocultos**

```
ls -la
# contenido de la carpeta
total 5
drwxrwxr-x  2 zaira zaira 4096 Mar 26 14:17 .
drwxr-x--- 61 zaira zaira 4096 Mar 26 14:12 ..
-rw-rw-r--  1 zaira zaira    0 Mar 26 14:17 .bash_history
-rw-rw-r--  1 zaira zaira    0 Mar 26 14:17 .bash_logout
-rw-rw-r--  1 zaira zaira    0 Mar 26 14:17 .bashrc

find . -type f -name ".*"
# resultado del find
./.bash_logout
./.bashrc
./.bash_history
```

Arriba puedes ver una lista de archivos ocultos en mi directorio personal.

#### Cómo buscar archivos de registro y archivos de configuración

Los archivos de registro generalmente tienen la extensión `.log`, y podemos encontrarlos de esta manera:

```
 find . -type f -name "*.log"
```

De manera similar, podemos buscar archivos de configuración así:

```
 find . -type f -name "*.conf"
```

#### Cómo buscar otros archivos por tipo

Podemos buscar archivos de bloques de caracteres proporcionando `c` a `-type`:

```
find / -type c
```

De manera similar, podemos encontrar archivos de bloques de dispositivos usando `b`:

```
find / -type b
```

#### Cómo buscar directorios

En el ejemplo a continuación, estamos encontrando las carpetas usando la bandera `-type d`.

```
ls -l
# lista contenido de la carpeta
drwxrwxr-x 2 zaira zaira 4096 Mar 26 14:22 hosts
-rw-rw-r-- 1 zaira zaira    0 Mar 26 14:23 hosts.txt
drwxrwxr-x 2 zaira zaira 4096 Mar 26 14:22 images
drwxrwxr-x 2 zaira zaira 4096 Mar 26 14:23 style
drwxrwxr-x 2 zaira zaira 4096 Mar 26 14:22 webp 

find . -type d 
# resultado del find de directorios
.
./webp
./images
./style
./hosts
```

#### Cómo buscar archivos por tamaño

Un uso increíblemente útil del comando `find` es listar archivos basados en un tamaño particular.

```
find / -size +250M
```

Aquí, estamos listando archivos cuyo tamaño excede `250MB`.

Otras unidades incluyen:

-   `G`: GigaBytes.
    
-   `M`: MegaBytes.
    
-   `K`: KiloBytes
    
-   `c` : bytes.
    

Simplemente reemplaza con la unidad relevante.

```
find <directorio> -type f -size +N<Tipo de Unidad>
```

#### Cómo buscar archivos por tiempo de modificación

Usando la bandera `-mtime`, puedes filtrar archivos y carpetas basados en el tiempo de modificación.

```
find /path -name "*.txt" -mtime -10
```

Por ejemplo,

-   **\-mtime +10** significa que estás buscando un archivo modificado hace 10 días.
    
-   **\-mtime -10** significa menos de 10 días.
    
-   **\-mtime 10** Si omites + o – significa exactamente 10 días.
    

### 4.5. Comandos Básicos para Ver Archivos

#### Concatenar y mostrar archivos usando el comando `cat`

El comando `cat` en Linux se usa para mostrar el contenido de un archivo. También se puede usar para concatenar archivos y crear nuevos archivos.

Aquí está la sintaxis básica del comando `cat`:

```
cat [opciones] [archivo]
```

La forma más simple de usar `cat` es sin opciones ni argumentos. Esto mostrará el contenido del archivo en la terminal.

Por ejemplo, si quieres ver el contenido de un archivo llamado `file.txt`, puedes usar el siguiente comando:

```
cat file.txt
```

Esto mostrará todo el contenido del archivo en la terminal de una vez.

#### Ver archivos de texto interactivamente usando `less` y `more`

Mientras que `cat` muestra el archivo completo de una vez, `less` y `more` te permiten ver el contenido de un archivo interactivamente. Esto es útil cuando quieres desplazarte por un archivo grande o buscar contenido específico.

La sintaxis del comando `less` es:

```
less [opciones] [archivo]
```

El comando `more` es similar a `less` pero tiene menos características. Se usa para mostrar el contenido de un archivo una pantalla a la vez.

La sintaxis del comando `more` es:

```
more [opciones] [archivo]
```

Para ambos comandos, puedes usar la `barra espaciadora` para desplazarte una página hacia abajo, la tecla `Enter` para desplazarte una línea hacia abajo y la tecla `q` para salir del visor.

Para moverte hacia atrás, puedes usar la tecla `b`, y para moverte hacia adelante, puedes usar la tecla `f`.

#### Mostrar la última parte de los archivos usando `tail`

A veces podrías necesitar ver solo las últimas líneas de un archivo en lugar del archivo completo. El comando `tail` en Linux se usa para mostrar la última parte de un archivo.

Por ejemplo, `tail file.txt` mostrará las últimas 10 líneas del archivo `file.txt` por defecto.

Si quieres mostrar un número diferente de líneas, puedes usar la opción `-n` seguida del número de líneas que quieres mostrar.

```
# Mostrar las últimas 50 líneas del archivo file.txt
tail -n 50 file.txt
```

💡**Consejo:** Otro uso del `tail` es su opción de seguimiento (`-f`). Esta opción te permite ver el contenido de un archivo a medida que se escriben. Esta es una utilidad útil para ver y monitorear archivos de registro en tiempo real.

#### Mostrar el principio de los archivos usando `head`



Por ejemplo, `head file.txt` mostrará las primeras 10 líneas del archivo `file.txt` por defecto.

Para cambiar el número de líneas mostradas, puedes usar la opción `-n` seguida del número de líneas que deseas mostrar.

#### Contando palabras, líneas y caracteres usando `wc`

Puedes contar palabras, líneas y caracteres en un archivo utilizando el comando `wc`.

Por ejemplo, ejecutar `wc syslog.log` me dio el siguiente resultado:

```
1669 9623 64367 syslog.log
```

En el resultado anterior,

-   `1669` representa el número de líneas en el archivo `syslog.log`.
    
-   `9623` representa el número de palabras en el archivo `syslog.log`.
    
-   `64367` representa el número de caracteres en el archivo `syslog.log`.
    

Así que, el comando `wc syslog.log` contó `1669` líneas, `9623` palabras, y `64367` caracteres en el archivo `syslog.log`.

#### Comparando archivos línea por línea usando `diff`

Comparar y encontrar diferencias entre dos archivos es una tarea común en Linux. Puedes comparar dos archivos directamente en la línea de comandos usando el comando `diff`.

La sintaxis básica del comando `diff` es:

```
diff [opciones] archivo1 archivo2
```

Aquí hay dos archivos, `hello.py` y `also-hello.py`, que compararemos utilizando el comando `diff`:

```
# contenido de hello.py

def greet(name):
    return f"Hello, {name}!"

user = input("Enter your name: ")
print(greet(user))
```

```
# contenido de also-hello.py

more also-hello.py
def greet(name):
    return fHello, {name}!

user = input(Enter your name: )
print(greet(user))
print("Nice to meet you")
```

1.  Comprobar si los archivos son iguales o no

```
diff -q hello.py also-hello.py
# Salida
Files hello.py and also-hello.py differ
```

2.  Ver cómo difieren los archivos. Para eso, puedes usar la opción `-u` para ver un resultado unificado:

```
diff -u hello.py also-hello.py
--- hello.py    2024-05-24 18:31:29.891690478 +0500
+++ also-hello.py    2024-05-24 18:32:17.207921795 +0500
@@ -3,4 +3,5 @@

 user = input(Enter your name: )
 print(greet(user))
+print("Nice to meet you")
```

En el resultado anterior:

-   `--- hello.py 2024-05-24 18:31:29.891690478 +0500` indica el archivo que se está comparando y su marca temporal.
    
-   `+++ also-hello.py 2024-05-24 18:32:17.207921795 +0500` indica el otro archivo que se está comparando y su marca temporal.
    
-   `@@ -3,4 +3,5 @@` muestra los números de línea donde ocurren los cambios. En este caso, indica que las líneas 3 a 4 en el archivo original han cambiado a las líneas 3 a 5 en el archivo modificado.
    
-   `user = input(Enter your name: )` es una línea del archivo original.
    
-   `print(greet(user))` es otra línea del archivo original.
    
-   `+print("Nice to meet you")` es la línea adicional en el archivo modificado.
    

3.  Para ver la diferencia en un formato lado a lado, puedes usar la opción `-y`:

```
diff -y hello.py also-hello.py
# Salida
def greet(name):                        def greet(name):
    return fHello, {name}!                        return fHello, {name}!

user = input(Enter your name: )                    user = input(Enter your name: )
print(greet(user))                                print(greet(user))
                                        >    print("Nice to meet you")
```

En el resultado:

-   Las líneas que son iguales en ambos archivos se muestran lado a lado.
    
-   Las líneas que son diferentes se muestran con un símbolo `>` indicando que la línea está presente solo en uno de los archivos.
    

## Parte 5: Lo Esencial de la Edición de Texto en Linux

Las habilidades de edición de texto usando la línea de comandos son una de las habilidades más cruciales en Linux. En esta sección, aprenderás cómo usar dos editores de texto populares en Linux: Vim y Nano.

Te sugiero que domines alguno de los editores de texto de tu elección y te apegues a él. Te ahorrará tiempo y te hará más productivo. Vim y nano son opciones seguras ya que están presentes en la mayoría de las distribuciones de Linux.

### 5.1. Dominar Vim: La Guía Completa

#### Introducción a Vim

Vim es una popular herramienta de edición de texto para la línea de comandos. Vim tiene sus ventajas: es poderoso, personalizable y rápido. Aquí hay algunas razones por las que deberías considerar aprender Vim:

-   La mayoría de los servidores se acceden a través de una CLI, así que en la administración de sistemas, no necesariamente tienes el lujo de una GUI. Pero Vim está a tu disposición – siempre estará ahí.
    
-   Vim usa un enfoque centrado en el teclado, ya que está diseñado para ser usado sin un mouse, lo que puede acelerar significativamente las tareas de edición una vez que has aprendido los atajos de teclado. Esto también lo hace más rápido que las herramientas GUI.
    
-   Algunas utilidades de Linux, por ejemplo, la edición de trabajos cron, funcionan en el mismo formato de edición que Vim.
    
-   Vim es adecuado para todos – principiantes y usuarios avanzados. Vim soporta búsquedas de cadena complejas, resaltado de búsquedas, y mucho más. A través de complementos, Vim proporciona capacidades extendidas a los desarrolladores y administradores de sistemas que incluyen autocompletado de código, resaltado de sintaxis, gestión de archivos, control de versiones, y más.
    

Vim tiene dos variaciones: Vim (`vim`) y Vim tiny (`vi`). Vim tiny es una versión más pequeña de Vim que carece de algunas características de Vim.

#### Cómo comenzar a usar `vim`

Comienza a usar Vim con este comando:

```
vim your-file.txt
```

`your-file.txt` puede ser un archivo nuevo o un archivo existente que quieras editar.

En los primeros días de la CLI, los teclados no tenían teclas de flecha. Por lo tanto, la navegación se realizaba utilizando el conjunto de teclas disponibles, `hjkl` siendo uno de ellos.

Siendo centrado en el teclado, utilizar las teclas `hjkl` puede acelerar en gran medida las tareas de edición de texto.

Nota: Aunque las teclas de flecha funcionarían perfectamente, aún puedes experimentar con las teclas `hjkl` para navegar. Algunas personas encuentran eficiente esta forma de navegación.

💡**Consejo:** Para recordar la secuencia `hjkl`, usa esto: **h**az atrás, **j**ump (salta) hacia abajo, **k**ick (patea) hacia arriba, **l**anzarse hacia adelante.

![Guía de navegación hjkl](https://cdn.hashnode.com/res/hashnode/image/upload/v1719392462442/1a667ede-5f03-4acb-b40f-b10cefc64de3.png)

#### Los tres modos de Vim

Necesitas conocer los 3 modos operativos de Vim y cómo cambiar entre ellos. Las pulsaciones de teclas se comportan de manera diferente en cada modo de comando. Los tres modos son los siguientes:

1.  Modo de comando.
    
2.  Modo de edición.
    
3.  Modo visual.
    

**Modo de Comando.** Cuando inicias Vim, aterrizas en el modo de comando por defecto. Este modo te permite acceder a otros modos.

⚠ Para cambiar a otros modos, primero debes estar en el modo de comando

**Modo de Edición**

Este modo te permite hacer cambios en el archivo. Para entrar en el modo de edición, presiona `I` mientras estás en el modo de comando. Nota el interruptor `'-- INSERT'` al final de la pantalla.

![Modo de inserción en Vim](https://cdn.hashnode.com/res/hashnode/image/upload/v1719392526710/d44cecd7-64be-4c89-9a31-dbf395b77fcb.png)

**Modo Visual**

Este modo te permite trabajar en un solo carácter, un bloque de texto o líneas de texto. Vamos a desglosarlo en pasos simples. Recuerda, usa las siguientes combinaciones cuando estés en el modo de comando.

-   `Shift + V` → Selecciona múltiples líneas.
    
-   `Ctrl + V` → Modo de bloque
    
-   `V` → Modo de carácter
    

El modo visual es muy útil cuando necesitas copiar y pegar o editar líneas en masa.

![Seleccionando texto usando el modo visual](https://cdn.hashnode.com/res/hashnode/image/upload/v1719392557097/b61a1515-cac0-4470-856b-b2c15de581e8.gif)

**Modo de comando extendido.**

El modo de comando extendido te permite realizar operaciones avanzadas como buscar, configurar números de línea y resaltar texto. Cubriremos el modo extendido en la siguiente sección.

¿Cómo mantenerse en el camino? Si olvidas tu modo actual, solo presiona `ESC` dos veces y volverás al Modo de Comando.

#### Editando Eficientemente en Vim: Copiar/pegar y buscar

**1\. Cómo copiar y pegar en Vim**

Copiar y pegar se conoce como 'yank' y 'put' en términos de Linux. Para copiar y pegar, sigue estos pasos:

-   Selecciona texto en el modo visual.
    
-   Presiona `'y'` para copiar/yank.
    
-   Mueve tu cursor a la posición requerida y presiona `'p'`.
    

**2\. Cómo buscar texto en Vim**

Cualquier serie de cadenas puede ser buscada con Vim usando el `/` en modo de comando. Para buscar, usa `/cadena-a-coincidir`.

En el modo de comando, escribe `:set hls` y presiona `enter`. Busca usando `/cadena-a-coincidir`. Esto resaltará las búsquedas.

Vamos a buscar algunas cadenas:

![Resaltando búsquedas en Vim](https://cdn.hashnode.com/res/hashnode/image/upload/v1719392684097/11c4a45e-0698-4fb7-bef7-f193684ea21a.gif)

**3\. Cómo salir de Vim**

Primero, muévete al modo de comando (presionando escape dos veces) y luego usa estas banderas:

-   Salir sin guardar → `:q!`
    
-   Salir y guardar → `:wq!`
    

#### Atajos en Vim: Haciendo la Edición Más Rápida

Nota: Todos estos atajos funcionan solo en el modo de comando.

-   **Navegación Básica**
    
    -   `h`: Moverse a la izquierda
        
    -   `j`: Moverse hacia abajo
        
    -   `k`: Moverse hacia arriba
        
    -   `l`: Moverse a la derecha
        
    -   `0`: Moverse al comienzo de la línea
        
    -   `$`: Moverse al final de la línea
        
    -   `gg`: Moverse al comienzo del archivo
        
    -   `G`: Moverse al final del archivo
        
    -   `Ctrl+d`: Moverse media página hacia abajo
        
    -   `Ctrl+u`: Moverse media página hacia arriba
        
-   **Edición**
    
    -   `i`: Entrar en modo de inserción antes del cursor
        
    -   `I`: Entrar en modo de inserción al comienzo de la línea
        
    -   `a`: Entrar en modo de inserción después del cursor
        
    -   `A`: Entrar en modo de inserción al final de la línea
        
    -   `o`: Abrir una nueva línea debajo de la línea actual y entrar en modo de inserción
        
    -   `O`: Abrir una nueva línea encima de la línea actual y entrar en modo de inserción
        
    -   `x`: Borrar el carácter debajo del cursor
        
    -   `dd`: Borrar la línea actual
        
    -   `yy`: Yank (copiar) la línea actual (usa esto en el modo visual)
        
    -   `p`: Pegar debajo del cursor
        
    -   `P`: Pegar encima del cursor
        
-   **Buscar y Reemplazar**
    
    -   `/`: Buscar un patrón que te llevará a su siguiente ocurrencia
        
    -   `?`: Buscar un patrón que te llevará a su ocurrencia anterior
        
    -   `n`: Repetir la última búsqueda en la misma dirección
        
    -   `N`: Repetir la última búsqueda en la dirección opuesta
        
    -   `:%s/viejo/nuevo/g`: Reemplazar todas las ocurrencias de `viejo` con `nuevo` en el archivo
        
-   **Salir**
    
    -   `:w`: Guardar el archivo pero no salir
        
    -   `:q`: Salir de Vim (falla si hay cambios no guardados)
        
    -   `:wq` o `:x`: Guardar y salir
        
    -   `:q!`: Salir sin guardar
        
-   **Múltiples Ventanas**
    
    -   `:split` o `:sp`: Dividir la ventana horizontalmente
        
    -   `:vsplit` o `:vsp`: Dividir la ventana verticalmente
        
    -   `Ctrl+w seguido de h/j/k/l`: Navegar entre las ventanas divididas

#### Comenzando con Nano: El editor de texto amigable para el usuario

Nano es un editor de texto amigable para el usuario que es fácil de usar y perfecto para principiantes. Está preinstalado en la mayoría de las distribuciones de Linux.

Para crear un nuevo archivo usando Nano, use el siguiente comando:

```
nano
```

Para comenzar a editar un archivo existente con Nano, use el siguiente comando:

```
nano nombre_del_archivo
```

#### Lista de atajos de teclado en Nano

Vamos a estudiar los atajos de teclado más importantes en Nano. Usarás los atajos de teclado para realizar varias operaciones como guardar, salir, copiar, pegar y más.

**Escribir en un archivo y guardar**

Una vez que abra Nano usando el comando `nano`, puede comenzar a escribir texto. Para guardar el archivo, presione `Ctrl+O`. Se le pedirá que ingrese el nombre del archivo. Presione `Enter` para guardar el archivo.

**Salir de nano**

Puede salir de Nano presionando `Ctrl+X`. Si tiene cambios no guardados, Nano le pedirá que guarde los cambios antes de salir.

**Copiar y pegar**

Para seleccionar una región, use `ALT+A`. Aparecerá un marcador. Use las flechas para seleccionar el texto. Una vez seleccionado, salga del marcador con `ALT+^`.

Para copiar el texto seleccionado, presione `Ctrl+K`. Para pegar el texto copiado, presione `Ctrl+U`.

**Cortar y pegar**

Seleccione la región con `ALT+A`. Una vez seleccionada, corte el texto con `Ctrl+K`. Para pegar el texto cortado, presione `Ctrl+U`.

**Navegación**

Use `Alt \` para moverse al principio del archivo.

Use `Alt /` para moverse al final del archivo.

**Ver números de línea**

Cuando abra un archivo con `nano -l nombre_del_archivo`, puede ver los números de línea en el lado izquierdo del archivo.

**Búsqueda**

Puede buscar un número de línea específico con `ALt + G`. Ingrese el número de línea en el cuadro de diálogo y presione `Enter`.

También puede iniciar una búsqueda para una cadena con `CTRL + W` y presione Enter. Si desea buscar hacia atrás, puede presionar `Alt+W` después de iniciar la búsqueda con `Ctrl+W`.

#### Resumen de atajos de teclado en Nano

-   **General**

    -   `Ctrl+X`: Salir de Nano (solicitando guardar si se hicieron cambios)
        
    -   `Ctrl+O`: Guardar el archivo
        
    -   `Ctrl+R`: Leer un archivo en el archivo actual
        
    -   `Ctrl+G`: Mostrar el texto de ayuda
        
-   **Edición**
    
    -   `Ctrl+K`: Cortar la línea actual y almacenarla en el búfer de corte
        
    -   `Ctrl+U`: Pegar el contenido del búfer de corte en la línea actual
        
    -   `Alt+6`: Copiar la línea actual y almacenarla en el búfer de corte
        
    -   `Ctrl+J`: Justificar el párrafo actual
        
-   **Navegación**
    
    -   `Ctrl+A`: Moverse al principio de la línea
        
    -   `Ctrl+E`: Moverse al final de la línea
        
    -   `Ctrl+C`: Mostrar el número de línea actual y la información del archivo
        
    -   `Ctrl+_` (`Ctrl+Shift+-`): Ir a un número de línea específico (y opcionalmente, número de columna)
        
    -   `Ctrl+Y`: Desplazarse una página hacia arriba
        
    -   `Ctrl+V`: Desplazarse una página hacia abajo
        
-   **Buscar y Reemplazar**
    
    -   `Ctrl+W`: Buscar una cadena (luego `Enter` para buscar de nuevo)
        
    -   `Alt+W`: Repetir la última búsqueda, pero en la dirección opuesta
        
    -   `Ctrl+\`: Buscar y reemplazar
        
-   **Misceláneo**
    
    -   `Ctrl+T`: Invocar el corrector ortográfico, si está disponible
        
    -   `Ctrl+D`: Eliminar el carácter bajo el cursor (no lo corta)
        
    -   `Ctrl+L`: Refrescar (redibujar) la pantalla actual
        
    -   `Alt+U`: Deshacer la última operación
        
    -   `Alt+E`: Rehacer la última operación deshecha
        

## Parte 6: Scripting en Bash

### 6.1. Definición de scripting en Bash

Un script de bash es un archivo que contiene una secuencia de comandos que son ejecutados por el programa bash línea por línea. Le permite realizar una serie de acciones, como navegar a un directorio específico, crear una carpeta y lanzar un proceso usando la línea de comandos.

Al guardar comandos en un script, puede repetir la misma secuencia de pasos múltiples veces y ejecutarlos al correr el script.

### 6.2. Ventajas del Scripting en Bash

El scripting en bash es una herramienta poderosa y versátil para automatizar tareas de administración del sistema, gestionar recursos del sistema y realizar otras tareas rutinarias en sistemas Unix/Linux.

Algunas ventajas del scripting en shell son:

-   **Automatización**: Los scripts de shell le permiten automatizar tareas y procesos repetitivos, ahorrando tiempo y reduciendo el riesgo de errores que pueden ocurrir con la ejecución manual.
    
-   **Portabilidad**: Los scripts de shell pueden ejecutarse en varias plataformas y sistemas operativos, incluidos Unix, Linux, macOS e incluso Windows mediante el uso de emuladores o máquinas virtuales.
    
-   **Flexibilidad**: Los scripts de shell son altamente personalizables y pueden modificarse fácilmente para adaptarse a requisitos específicos. También pueden combinarse con otros lenguajes de programación o utilidades para crear scripts más poderosos.
    
-   **Accesibilidad**: Los scripts de shell son fáciles de escribir y no requieren herramientas o software especiales. Se pueden editar con cualquier editor de texto, y la mayoría de los sistemas operativos tienen un intérprete de shell incorporado.
    
-   **Integración**: Los scripts de shell pueden integrarse con otras herramientas y aplicaciones, como bases de datos, servidores web y servicios en la nube, permitiendo tareas de automatización y administración de sistemas más complejas.
    
-   **Depuración**: Los scripts de shell son fáciles de depurar, y la mayoría de los shells tienen herramientas de depuración y reporte de errores incorporadas que pueden ayudar a identificar y solucionar problemas rápidamente.
    


Los términos "shell" y "bash" a menudo se utilizan indistintamente. Pero hay una sutil diferencia entre los dos.

El término "shell" se refiere a un programa que proporciona una interfaz de línea de comandos para interactuar con un sistema operativo. Bash (Bourne-Again SHell) es una de las shells de Unix/Linux más comúnmente usadas y es la shell predeterminada en muchas distribuciones de Linux.

Hasta ahora, los comandos que has estado introduciendo básicamente se han estado introduciendo en una "shell".

Aunque Bash es un tipo de shell, también hay otras shells disponibles, como Korn shell (ksh), C shell (csh) y Z shell (zsh). Cada shell tiene su propia sintaxis y conjunto de características, pero todas comparten el propósito común de proporcionar una interfaz de línea de comandos para interactuar con el sistema operativo.

Puedes determinar tu tipo de shell usando el comando `ps`:

```
ps
# salida:

    PID TTY          TIME CMD
  20506 pts/0    00:00:00 bash <--- el tipo de shell
  20931 pts/0    00:00:00 ps
```

En resumen, mientras que "shell" es un término amplio que se refiere a cualquier programa que proporciona una interfaz de línea de comandos, "Bash" es un tipo específico de shell que se usa ampliamente en sistemas Unix/Linux.

Nota: En esta sección, utilizaremos la shell "bash".

### 6.4. Cómo Crear y Ejecutar Scripts Bash

**Convenciones de nomenclatura de scripts**

Por convención de nomenclatura, los scripts bash terminan con `.sh`. Sin embargo, los scripts bash pueden ejecutarse perfectamente sin la extensión `sh`.

**Agregando el Shebang**

Los scripts bash comienzan con un `shebang`. Shebang es una combinación de `bash #` y `bang !` seguida de la ruta de la shell bash. Esta es la primera línea del script. Shebang le dice a la shell que lo ejecute a través de la shell bash. Shebang es simplemente una ruta absoluta al intérprete bash.

A continuación hay un ejemplo de la declaración shebang.

```
#!/bin/bash
```

Puedes encontrar tu ruta de shell bash (que puede variar de lo anterior) usando el comando:

```
which bash
```

**Creando tu primer script bash**

Nuestro primer script solicita al usuario que ingrese una ruta. A cambio, se listarán sus contenidos.

Crea un archivo llamado `run_all.sh` usando cualquier editor de tu elección.

```
vim run_all.sh
```

Agrega los siguientes comandos en tu archivo y guárdalo:

```
#!/bin/bash
echo "Hoy es " `date`

echo -e "\ningresa la ruta del directorio"
read the_path

echo -e "\ntu ruta tiene los siguientes archivos y carpetas: "
ls $the_path
```

Veamos el script más detalladamente, línea por línea. Estoy mostrando el mismo script nuevamente, pero esta vez con números de línea.

```
  1 #!/bin/bash
  2 echo "Hoy es " `date`
  3
  4 echo -e "\ningresa la ruta del directorio"
  5 read the_path
  6
  7 echo -e "\ntu ruta tiene los siguientes archivos y carpetas: "
  8 ls $the_path
```

-   Línea #1: El shebang (`#!/bin/bash`) apunta hacia la ruta de la shell bash.
    
-   Línea #2: El comando `echo` muestra la fecha y hora actuales en el terminal. Nota que la `date` está entre comillas invertidas.
    
-   Línea #4: Queremos que el usuario ingrese una ruta válida.
    
-   Línea #5: El comando `read` lee la entrada y la guarda en la variable `the_path`.
    
-   Línea #8: El comando `ls` toma la variable con la ruta guardada y muestra los archivos y carpetas actuales.
    

**Ejecutando el script bash**

Para hacer el script ejecutable, asigna derechos de ejecución a tu usuario usando este comando:

```
chmod u+x run_all.sh
```

Aquí,

-   `chmod` modifica la propiedad de un archivo para el usuario actual :`u`.
    
-   `+x` agrega los derechos de ejecución al usuario actual. Esto significa que el usuario que es el propietario ahora puede ejecutar el script.
    
-   `run_all.sh` es el archivo que deseamos ejecutar.
    

Puedes ejecutar el script usando cualquiera de los métodos mencionados:

-   `sh run_all.sh`
    
-   `bash run_all.sh`
    
-   `./run_all.sh`
    

Veámoslo en acción 🚀

![Ejecutando un script bash](https://www.freecodecamp.org/news/content/images/2023/03/run-script-bash-2.gif)

### 6.5. Conceptos Básicos de la Programación Bash

#### Comentarios en la programación bash

Los comentarios comienzan con un `#` en la programación bash. Esto significa que cualquier línea que comience con un `#` es un comentario y será ignorado por el intérprete.

Los comentarios son muy útiles para documentar el código, y es una buena práctica agregarlos para ayudar a otros a entender el código.

Estos son ejemplos de comentarios:

```
# Este es un comentario de ejemplo
# Ambas líneas serán ignoradas por el intérprete
```

#### Variables y tipos de datos en Bash

Las variables te permiten almacenar datos. Puedes usar variables para leer, acceder y manipular datos a lo largo de tu script.

No hay tipos de datos en Bash. En Bash, una variable es capaz de almacenar valores numéricos, caracteres individuales o cadenas de caracteres.

En Bash, puedes usar y establecer los valores de las variables de las siguientes maneras:

1.  Asignar el valor directamente:

```
pais=Países Bajos
```

2\. Asignar el valor basado en la salida obtenida de un programa o comando, usando la sustitución de comandos. Nota que `$` es necesario para acceder al valor de una variable existente.

```
mismo_pais=$pais
```

Esto asigna el valor de `pais` a la nueva variable `mismo_pais`.

Para acceder al valor de la variable, agrega `$` al nombre de la variable.

```
pais=Países Bajos
echo $pais
# salida
Países Bajos
nuevo_pais=$pais
echo $nuevo_pais
# salida
Países Bajos
```

#### Convenciones para nombrar variables

En la programación de scripts en Bash, las siguientes son las convenciones para nombrar variables:

1. Los nombres de las variables deben comenzar con una letra o un guion bajo (`_`).

2. Los nombres de las variables pueden contener letras, números y guiones bajos (`_`).

3. Los nombres de las variables son sensibles a mayúsculas y minúsculas.

4. Los nombres de las variables no deben contener espacios ni caracteres especiales.

5. Use nombres descriptivos que reflejen el propósito de la variable.

6. Evite usar palabras reservadas, como `if`, `then`, `else`, `fi`, y otras como nombres de variables.

Aquí hay algunos ejemplos de nombres de variables válidos en Bash:

```
name
count
_var
myVar
MY_VAR
```

Y aquí hay algunos ejemplos de nombres de variables inválidos:

```
# nombres de variables inválidos

2ndvar (el nombre de la variable comienza con un número)
my var (el nombre de la variable contiene un espacio)
my-var (el nombre de la variable contiene un guion)
```

Seguir estas convenciones de nomenclatura ayuda a que los scripts de Bash sean más legibles y fáciles de mantener.

#### Entrada y salida en scripts de Bash

#### Obtener entrada

En esta sección, discutiremos algunos métodos para proporcionar entrada a nuestros scripts.

1. Leer la entrada del usuario y almacenarla en una variable

Podemos leer la entrada del usuario utilizando el comando `read`.

```
#!/bin/bash
echo "¿Cuál es tu nombre?"
read entered_name
echo -e "\nBienvenido al tutorial de Bash" $entered_name
```

![Leer el nombre desde un script](https://www.freecodecamp.org/news/content/images/2023/03/name-sh.gif)

2. Leer desde un archivo

Este código lee cada línea de un archivo llamado `input.txt` y la imprime en la terminal. Estudiaremos los bucles while más adelante en esta sección.

```
while read line
do
  echo $line
done < input.txt
```

3. Argumentos de línea de comandos

En un script o función de Bash, `$1` denota el primer argumento pasado, `$2` denota el segundo argumento pasado, y así sucesivamente.

Este script toma un nombre como argumento de línea de comandos e imprime un saludo personalizado.

```
#!/bin/bash
echo "¡Hola, $1!"
```

Hemos proporcionado `Zaira` como nuestro argumento al script.

**Salida:**

![Proporcionando argumentos al script de Bash](https://www.freecodecamp.org/news/content/images/2023/03/name-sh-1.gif)

#### Mostrar salida

Aquí discutiremos algunos métodos para recibir salida de los scripts.

1. Imprimir en la terminal:

```
echo "¡Hola, Mundo!"
```

Esto imprime el texto "¡Hola, Mundo!" en la terminal.

2. Escribir en un archivo:

```
echo "Este es un texto." > output.txt
```

Esto escribe el texto "Este es un texto." en un archivo llamado `output.txt`. Tenga en cuenta que el operador `>` sobrescribe un archivo si ya tiene algún contenido.

3. Añadir a un archivo:

```
echo "Más texto." >> output.txt
```

Esto añade el texto "Más texto." al final del archivo `output.txt`.

4. Redirigir salida:

```
ls > files.txt
```

Esto lista los archivos en el directorio actual y escribe la salida en un archivo llamado `files.txt`. Puede redirigir la salida de cualquier comando a un archivo de esta manera.

Aprenderá sobre la redirección de salida en detalle en la sección 8.5.

#### Declaraciones condicionales (if/else)

Las expresiones que producen un resultado booleano, ya sea verdadero o falso, se llaman condiciones. Hay varias formas de evaluar condiciones, incluyendo `if`, `if-else`, `if-elif-else` y condicionales anidados.

**Sintaxis**:

```
if [[ condición ]];
then
    sentencia
elif [[ condición ]]; then
    sentencia 
else
    hacer esto por defecto
fi
```

#### Sintaxis de declaraciones condicionales en Bash

Podemos usar operadores lógicos como AND `-a` y OR `-o` para hacer comparaciones que tengan más significado.

```
if [ $a -gt 60 -a $b -lt 100 ]
```

Esta declaración verifica si ambas condiciones son `verdaderas`: `a` es mayor que `60` Y `b` es menor que `100`.

Veamos un ejemplo de un script de Bash que usa declaraciones `if`, `if-else` y `if-elif-else` para determinar si un número ingresado por el usuario es positivo, negativo o cero:

```
#!/bin/bash

# Script para determinar si un número es positivo, negativo o cero

echo "Por favor, ingrese un número: "
read num

if [ $num -gt 0 ]; then
  echo "$num es positivo"
elif [ $num -lt 0 ]; then
  echo "$num es negativo"
else
  echo "$num es cero"
fi
```

El script primero pide al usuario que ingrese un número. Luego, usa una declaración `if` para verificar si el número es mayor que `0`. Si lo es, el script indica que el número es positivo. Si el número no es mayor que `0`, el script pasa a la siguiente declaración, que es una declaración `if-elif`.

Aquí, el script verifica si el número es menor que `0`. Si lo es, el script indica que el número es negativo.

Finalmente, si el número no es ni mayor que `0` ni menor que `0`, el script usa una declaración `else` para indicar que el número es cero.

Viéndolo en acción 🚀

![Verificando si un número es par o impar](https://www.freecodecamp.org/news/content/images/2023/03/test-odd.gif)

#### Bucles y bifurcaciones en Bash

**Bucle While**

Los bucles while verifican una condición y repiten el bucle hasta que la condición siga siendo `verdadera`. Necesitamos proporcionar una declaración de contador que incremente el contador para controlar la ejecución del bucle.

En el ejemplo a continuación, `(( i += 1 ))` es la declaración de contador que incrementa el valor de `i`. El bucle se ejecutará exactamente 10 veces.

```
#!/bin/bash
i=1
while [[ $i -le 10 ]] ; do
   echo "$i"
  (( i += 1 ))
done
```

**Bucle `for`**

El bucle `for`, al igual que el bucle `while`, te permite ejecutar declaraciones un número específico de veces. Cada bucle difiere en su sintaxis y uso.

En el ejemplo a continuación, el bucle iterará 5 veces.

```
#!/bin/bash

for i in {1..5}
do
    echo $i
done
```

![Bucle de 1 a 10 usando ](https://www.freecodecamp.org/news/content/images/2023/03/image-186.png)

**Declaraciones `case`**

En Bash, las declaraciones `case` se utilizan para comparar un valor dado contra una lista de patrones y ejecutar un bloque de código basado en el primer patrón que coincida. La sintaxis para una declaración `case` en Bash es la siguiente:

```
case expresión in
    patrón1)
        # código a ejecutar si la expresión coincide con patrón1
        ;;
    patrón2)
        # código a ejecutar si la expresión coincide con patrón2
        ;;
    patrón3)
        # código a ejecutar si la expresión coincide con patrón3
        ;;
    *)
        # código a ejecutar si ninguno de los patrones anteriores coincide con la expresión
        ;;
esac
```

Aquí, "expresión" es el valor que queremos comparar, y "patrón1", "patrón2", "patrón3", y así sucesivamente son los patrones contra los que queremos compararlo.

El doble punto y coma ";;" separa cada bloque de código a ejecutar para cada patrón. El asterisco "\*" representa el caso por defecto, que se ejecuta si ninguno de los patrones especificados coincide con la expresión.

Veamos un ejemplo:

```
fruta="manzana"

case $fruta in
    "manzana")
        echo "Esta es una fruta roja."
        ;;
    "banana")
        echo "Esta es una fruta amarilla."
        ;;
    "naranja")
        echo "Esta es una fruta naranja."
        ;;
    *)
        echo "Fruta desconocida."
        ;;
esac
```

En este ejemplo, dado que el valor de `fruta` es `manzana`, el primer patrón coincide, y se ejecuta el bloque de código que imprime `Esta es una fruta roja.` Si el valor de `fruta` fuera `banana`, el segundo patrón coincidiría y se ejecutaría el bloque de código que imprime `Esta es una fruta amarilla.`, y así sucesivamente.

Si el valor de `fruta` no coincide con ninguno de los patrones especificados, se ejecuta el caso por defecto, que imprime `Fruta desconocida.`

## Parte 7: Gestión de Paquetes de Software en Linux

Linux viene con varios programas incorporados. Pero podrías necesitar instalar nuevos programas según tus necesidades. También podrías necesitar actualizar las aplicaciones existentes.

### 7.1. Paquetes y Gestión de Paquetes

#### ¿Qué es un paquete?

Un paquete es una colección de archivos que se agrupan. Estos archivos son esenciales para que un programa particular se ejecute. Estos archivos contienen archivos ejecutables del programa, bibliotecas y otros recursos.

Además de los archivos requeridos para que el programa se ejecute, los paquetes también contienen scripts de instalación, que copian los archivos donde se necesitan. Un programa puede contener muchos archivos y dependencias. Con paquetes, es más fácil gestionar todos los archivos y dependencias a la vez.

#### ¿Cuál es la diferencia entre fuente y binario?

Los programadores escriben código fuente en un lenguaje de programación. Este código fuente se compila en código máquina que la computadora puede entender. El código compilado se llama código binario.

Cuando descargas un paquete, puedes obtener el _código fuente_ o el _código binario._ El código fuente es el código legible por humanos que se puede compilar en código binario. El código binario es el código compilado que la computadora puede entender.

Los paquetes de código fuente se pueden usar con cualquier tipo de máquina si el código fuente se compila correctamente. El binario, por otro lado, es el código compilado que es específico de un tipo particular de máquina o arquitectura.

Puedes encontrar la arquitectura de tu máquina usando el comando `uname -m`.

```
uname -m
# resultado
x86_64
```

#### Dependencias de paquetes

Los programas a menudo comparten archivos. En lugar de incluir estos archivos en cada paquete, un paquete separado puede proporcionarles estos archivos a todos los programas.

Para instalar un programa que necesita estos archivos, también debes instalar el paquete que los contiene. Esto se llama dependencia de paquetes. Especificar dependencias hace que los paquetes sean más pequeños y simples al reducir duplicados.

Cuando instalas un programa, sus dependencias también deben ser instaladas. La mayoría de las dependencias requeridas generalmente ya están instaladas, pero podrían necesitarse algunas adicionales. Así que, no te sorprendas si varios otros paquetes se instalan junto con el paquete que has elegido. Estas son las dependencias necesarias.

#### Gestores de paquetes

Linux ofrece un sistema de gestión de paquetes completo para instalar, actualizar, configurar y eliminar software.

Con la gestión de paquetes, puedes acceder a una base organizada de miles de paquetes de software, además de tener la capacidad de resolver dependencias y verificar actualizaciones de software.

Los paquetes se pueden gestionar usando utilidades de línea de comandos que pueden ser fácilmente automatizadas por administradores del sistema o a través de una interfaz gráfica.

#### Canales/repositorios de software

⚠️ La gestión de paquetes es diferente para distintas distribuciones. Aquí, estamos usando Ubuntu.

Instalar software es un poco diferente en Linux en comparación con Windows y Mac.

Linux utiliza repositorios para almacenar paquetes de software. Un repositorio es una colección de paquetes de software que están disponibles para instalación a través de un gestor de paquetes.

El proceso genérico de descargar software desde un repositorio se ve algo así:

![Proceso de descarga de software desde un repositorio remoto](https://cdn.hashnode.com/res/hashnode/image/upload/v1719313472889/f4961606-b9c4-4ed7-8edc-61e0fc6908e4.png)

Si hablamos específicamente de Ubuntu,

1.  El índice se obtiene usando `apt update`. (`apt` se explica en la siguiente sección).
    
2.  Se solicitan los archivos / dependencias necesarios según el índice usando `apt install`
    
3.  Los paquetes y dependencias se instalan localmente.
    
4.  Actualiza las dependencias y paquetes cuando sea necesario usando `apt update` y `apt upgrade`
    

En distros basadas en Debian, puedes encontrar la lista de repositorios en `/etc/apt/sources.list`.

### 7.2. Instalación de un paquete vía línea de comandos

El comando `apt` es una poderosa herramienta de línea de comandos, que trabaja con la "Herramienta Avanzada de Empaquetado (APT)" de Ubuntu.

`apt`, junto con los comandos que lo acompañan, proporciona los medios para instalar nuevos paquetes de software, actualizar los paquetes de software existentes, actualizar el índice de la lista de paquetes e incluso actualizar todo el sistema Ubuntu.

Para ver los registros de la instalación utilizando `apt`, puedes ver el archivo `/var/log/dpkg.log`.

A continuación se indican los usos del comando `apt`:

#### Instalación de paquetes

Por ejemplo, para instalar el paquete `htop`, puedes usar el siguiente comando:

```
sudo apt install htop
```

#### Actualización del índice de la lista de paquetes

El índice de la lista de paquetes es una lista de todos los paquetes disponibles en los repositorios. Para actualizar el índice de la lista de paquetes local, puedes usar el siguiente comando:

```
sudo apt update
```

#### Actualización de los paquetes

Los paquetes instalados en tu sistema pueden recibir actualizaciones que contienen correcciones de errores, parches de seguridad y nuevas características.

Para actualizar los paquetes, puedes usar el siguiente comando:

```
sudo apt upgrade
```

#### Eliminación de paquetes

Para eliminar un paquete, como `htop`, puedes usar el siguiente comando:

```
sudo apt remove htop
```

### 7.3. Instalación de un paquete vía un método gráfico avanzado – Synaptic

Si no te sientes cómodo con la línea de comandos, puedes usar una aplicación GUI para instalar paquetes. Puedes lograr los mismos resultados que con la línea de comandos, pero con una interfaz gráfica.

Synaptic es una aplicación de gestión de paquetes GUI que ayuda a listar los paquetes instalados, su estado, las actualizaciones pendientes, etc. Ofrece filtros personalizados para ayudarte a reducir los resultados de búsqueda.

![0f362ed7-c371-4a58-96c2-c359178cdbd9](https://cdn.hashnode.com/res/hashnode/image/upload/v1719313599636/0f362ed7-c371-4a58-96c2-c359178cdbd9.png)

También puedes hacer clic derecho sobre un paquete y ver más detalles como las dependencias, el mantenedor, el tamaño y los archivos instalados.

![Ver los detalles de un paquete](https://cdn.hashnode.com/res/hashnode/image/upload/v1719313607397/33b7ad76-2492-4805-8133-35c8cd3c4a0a.png)

### 7.4. Instalación de paquetes descargados de un sitio web

Puedes querer instalar un paquete que hayas descargado de un sitio web, en lugar de desde un repositorio de software. Estos paquetes se llaman archivos `.deb`.

**Usando**`dpkg`**para instalar paquetes:**`dpkg` es una herramienta de línea de comandos utilizada para instalar paquetes. Para instalar un paquete con **dpkg**, abre la Terminal y escribe lo siguiente:

```
cd directorio
sudo dpkg -i nombre_paquete.deb
```

Nota: Reemplaza "directorio" con el directorio donde está almacenado el paquete y "nombre_paquete" con el nombre del archivo del paquete.

Alternativamente, puedes hacer clic derecho, seleccionar "Abrir con otra aplicación" y elegir una aplicación GUI de tu elección.

![Instalando un software usando una aplicación](https://cdn.hashnode.com/res/hashnode/image/upload/v1719322161581/f16d83ac-ca9a-4502-a80c-e6a25dee5c68.png)

💡 **Consejo:** En Ubuntu, puedes ver una lista de los paquetes instalados con `dpkg --list`.

## Parte 8: Temas avanzados de Linux

### 8.1. Gestión de usuarios

Puede haber múltiples usuarios con diferentes niveles de acceso en un sistema. En Linux, el usuario root tiene el nivel de acceso más alto y puede realizar cualquier operación en el sistema. Los usuarios regulares tienen acceso limitado y solo pueden realizar operaciones para las que se les haya concedido permiso.

#### ¿Qué es un usuario?

Una cuenta de usuario proporciona separación entre diferentes personas y programas que pueden ejecutar comandos.

Los humanos identifican a los usuarios por un nombre, ya que los nombres son fáciles de manejar. Pero el sistema identifica a los usuarios por un número único llamado ID de usuario (UID).

Cuando los usuarios humanos inician sesión usando el nombre de usuario proporcionado, tienen que usar una contraseña para autorizarse.

Las cuentas de usuario forman las bases de la seguridad del sistema. La propiedad de los archivos también está asociada con las cuentas de usuario y refuerza el control de acceso a los archivos. Cada proceso tiene una cuenta de usuario asociada que proporciona una capa de control para los administradores.

Hay tres tipos principales de cuentas de usuario:

1.  **Superusuario**: El superusuario tiene acceso completo al sistema. El nombre del superusuario es `root`. Tiene un `UID` de 0.
    
2.  **Usuario del sistema**: El usuario del sistema tiene cuentas de usuario que se utilizan para ejecutar servicios del sistema. Estas cuentas se utilizan para ejecutar servicios del sistema y no están destinadas a la interacción humana.
    
3.  **Usuario regular**: Los usuarios regulares son usuarios humanos que tienen acceso al sistema.
    

```
id
uid=1000(john) gid=1000(john) groups=1000(john),4(adm),24(cdrom),27(sudo),30(dip)... salida truncada
```

Para ver la información básica de otro usuario, pasa el nombre de usuario como un argumento al comando `id`.

```
id nombredeusuario
```

Para ver información relacionada con el usuario para procesos, usa el comando `ps` con el flag `-u`.

```
ps -u
# Salida
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root         1  0.0  0.1  16968  3920 ?        Ss   18:45   0:00 /sbin/init splash
root         2  0.0  0.0      0     0 ?        S    18:45   0:00 [kthreadd]
```

Por defecto, los sistemas usan el archivo `/etc/passwd` para almacenar la información del usuario.

Aquí hay una línea del archivo `/etc/passwd`:

```
root:x:0:0:root:/root:/bin/bash
```

El archivo `/etc/passwd` contiene la siguiente información sobre cada usuario:

1.  Nombre de usuario: `root` – El nombre de usuario de la cuenta.
    
2.  Contraseña: `x` – La contraseña en formato cifrado para la cuenta de usuario que se almacena en el archivo `/etc/shadow` por razones de seguridad.
    
3.  ID de usuario (UID): `0` – El identificador numérico único para la cuenta de usuario.
    
4.  ID de grupo (GID): `0` – El identificador principal del grupo para la cuenta de usuario.
    
5.  Información del usuario: `root` – El nombre real para la cuenta de usuario.
    
6.  Directorio home: `/root` – El directorio home para la cuenta de usuario.
    
7.  Shell: `/bin/bash` – El shell predeterminado para la cuenta de usuario. Un usuario del sistema podría usar `/sbin/nologin` si no se permiten inicios de sesión interactivos para ese usuario.
    

#### ¿Qué es un grupo?

Un grupo es una colección de cuentas de usuario que comparten acceso y recursos. Los grupos tienen nombres que los identifican. El sistema identifica a los grupos por un número único llamado ID de grupo (GID).

Por defecto, la información sobre los grupos se almacena en el archivo `/etc/group`.

Aquí hay una entrada del archivo `/etc/group`:

```
adm:x:4:syslog,john
```

Aquí está el desglose de los campos en la entrada dada:

1.  Nombre del grupo: `adm` – El nombre del grupo.
    
2.  Contraseña: `x` – La contraseña para el grupo se almacena en el archivo `/etc/gshadow` por razones de seguridad. La contraseña es opcional y aparece vacía si no está configurada.
    
3.  ID de grupo (GID): `4` – El identificador numérico único para el grupo.
    
4.  Miembros del grupo: `syslog,john` – La lista de nombres de usuarios que son miembros del grupo. En este caso, el grupo `adm` tiene dos miembros: `syslog` y `john`.
    

En esta entrada específica, el nombre del grupo es `adm`, el ID del grupo es `4`, y el grupo tiene dos miembros: `syslog` y `john`. El campo de la contraseña normalmente se establece en `x` para indicar que la contraseña del grupo se almacena en el archivo `/etc/gshadow`.

Los grupos se dividen además en grupos '_primarios'_ y '_suplementarios_'.

-   Grupo Primario: A cada usuario se le asigna un grupo primario por defecto. Este grupo usualmente tiene el mismo nombre que el usuario y se crea cuando se hace la cuenta de usuario. Los archivos y directorios creados por el usuario generalmente son propiedad de este grupo primario.
    
-   Grupos Suplementarios: Estos son grupos adicionales a los que un usuario puede pertenecer además de su grupo primario. Los usuarios pueden ser miembros de múltiples grupos suplementarios. Estos grupos permiten a un usuario tener permisos para recursos compartidos entre esos grupos. Ayudan a proporcionar acceso a recursos compartidos sin afectar los permisos de los archivos del sistema y manteniendo la seguridad intacta. Mientras que un usuario debe pertenecer a un grupo primario, pertenecer a grupos suplementarios es opcional.
    

#### Control de acceso: encontrando y entendiendo los permisos de archivos

La propiedad de los archivos se puede ver usando el comando `ls -l`. La primera columna en la salida del comando `ls -l` muestra los permisos del archivo. Otras columnas muestran al propietario del archivo y al grupo al que pertenece el archivo.

![Salida detallada de ls -l](https://www.freecodecamp.org/news/content/images/2022/04/image-146.png)

Echemos un vistazo más de cerca a la columna `mode`:

![Clases de permisos y tipos de archivo](https://www.freecodecamp.org/news/content/images/2022/04/image-147.png)

**Modo** define dos cosas:

-   **Tipo de archivo:** El tipo de archivo define el tipo de archivo. Para archivos regulares que contienen datos simples es en blanco `-`. Para otros tipos de archivo especiales el símbolo es diferente. Para un directorio que es un archivo especial, es `d`. Los archivos especiales son tratados de forma diferente por el SO.
    
-   **Clases de permisos:** El siguiente conjunto de caracteres define los permisos para usuario, grupo, y otros, respectivamente.  
    – **Usuario**: Este es el propietario de un archivo y el propietario del archivo pertenece a esta clase.  
    – **Grupo**: Los miembros del grupo del archivo pertenecen a esta clase  
    – **Otros**: Cualquier usuario que no sea parte de las clases de usuario o grupo pertenece a esta clase.
    

💡**Consejo:** La propiedad del directorio se puede ver usando el comando `ls -ld`.

##### Cómo leer permisos simbólicos o los permisos `rwx`

La representación `rwx` se conoce como la representación simbólica de los permisos. En el conjunto de permisos,

-   `r` significa **lectura**. Se indica en el primer carácter de la tríada.
    
-   `w` significa **escritura**. Se indica en el segundo carácter de la tríada.
    
-   `x` significa **ejecución**. Se indica en el tercer carácter de la tríada.
    
```

Para archivos regulares, los permisos de lectura permiten que el archivo se abra y lea únicamente. Los usuarios no pueden modificar el archivo.

De manera similar, los permisos de lectura en directorios permiten listar el contenido del directorio sin ninguna modificación en el directorio.

**Escribir:**

Cuando los archivos tienen permisos de escritura, el usuario puede modificar (editar, eliminar) el archivo y guardarlo.

Para carpetas, los permisos de escritura permiten a un usuario modificar su contenido (crear, eliminar y renombrar archivos dentro de ella) y modificar el contenido de los archivos a los que el usuario tiene permisos de escritura.

**Ejemplos de permisos en Linux**

Ahora que sabemos cómo leer los permisos, veamos algunos ejemplos.

-   `-rwx------`: Un archivo que solo es accesible y ejecutable por su propietario.
    
    `-rw-rw-r--`: Un archivo que está abierto a modificaciones por su propietario y grupo, pero no por otros.
    
-   `drwxrwx---`: Un directorio que puede ser modificado por su propietario y grupo.
    

**Ejecutar:**

Para archivos, los permisos de ejecución permiten al usuario ejecutar un script ejecutable. Para directorios, el usuario puede acceder a ellos y acceder a detalles sobre los archivos en el directorio.

##### Cómo cambiar permisos y propiedades de archivos en Linux usando `chmod` y `chown`

Ahora que conocemos lo básico sobre propiedades y permisos, veamos cómo podemos modificar permisos usando el comando `chmod`.

**Sintaxis de**`chmod`:

```
chmod permisos nombre-de-archivo
```

Donde,

-   `permisos` pueden ser lectura, escritura, ejecución o una combinación de estos.
    
-   `nombre-de-archivo` es el nombre del archivo cuyo permisos necesitan cambiarse. Este parámetro también puede ser una lista si se quieren cambiar permisos de archivos en masa.
    

Podemos cambiar permisos usando dos modos:

1.  **Modo simbólico**: este método usa símbolos como `u`, `g`, `o` para representar usuarios, grupos y otros. Los permisos se representan como `r, w, x` para lectura, escritura y ejecución, respectivamente. Se pueden modificar permisos usando +, - y =.
    
2.  **Modo absoluto**: este método representa los permisos como números octales de 3 dígitos que van del 0 al 7.
    

Ahora, veámoslos en detalle.

##### Cómo cambiar permisos usando el modo simbólico

La tabla a continuación resume la representación de usuarios:

| **REPRESENTACIÓN DE USUARIOS** | **DESCRIPCIÓN** |
| --- | --- |
| u | usuario/propietario |
| g | grupo |
| o | otros |

Podemos usar operadores matemáticos para agregar, eliminar y asignar permisos. La tabla a continuación muestra el resumen:

| **OPERADOR** | **DESCRIPCIÓN** |
| --- | --- |
| + | Agrega un permiso a un archivo o directorio |
| – | Elimina el permiso |
| \\= | Establece el permiso si no estaba presente antes. También anula los permisos establecidos anteriormente. |

**Ejemplo:**

Supongamos que tengo un script y quiero hacerlo ejecutable para el propietario del archivo `zaira`.

Los permisos actuales del archivo son los siguientes:

![image-161](https://www.freecodecamp.org/news/content/images/2022/04/image-161.png)

Dividamos los permisos de esta manera:

![División de permisos de archivos](https://www.freecodecamp.org/news/content/images/2022/04/image-160.png)

Para agregar derechos de ejecución (`x`) al propietario (`u`) usando el modo simbólico, podemos usar el siguiente comando:

```
chmod u+x mymotd.sh
```

**Salida:**

Ahora, podemos ver que los permisos de ejecución se han agregado para el propietario `zaira`.

![Permiso actualizado](https://www.freecodecamp.org/news/content/images/2022/04/image-162.png)

**Ejemplos adicionales para cambiar permisos vía método simbólico:**

-   Eliminar permisos de `lectura` y `escritura` para `grupo` y `otros`: `chmod go-rw`.
    
-   Eliminar permisos de `lectura` para `otros`: `chmod o-r`.
    
-   Asignar permiso de `escritura` al `grupo` y anular permisos existentes: `chmod g=w`.
    

##### Cómo cambiar permisos usando el modo absoluto

El modo absoluto usa números para representar permisos y operadores matemáticos para modificarlos.

La siguiente tabla muestra cómo podemos asignar los permisos relevantes:

| **PERMISO** | **ASIGNAR PERMISO** |
| --- | --- |
| lectura | agregar 4 |
| escritura | agregar 2 |
| ejecución | agregar 1 |

Los permisos pueden ser revocados usando la resta. La siguiente tabla muestra cómo puedes eliminar los permisos relevantes.

| **PERMISO** | **REVOCAR PERMISO** |
| --- | --- |
| lectura | restar 4 |
| escritura | restar 2 |
| ejecución | restar 1 |

**Ejemplo**:

-   Establecer `lectura` (agregar 4) para `usuario`, `lectura` (agregar 4) y `ejecución` (agregar 1) para grupo, y solo `ejecución` (agregar 1) para otros.

`chmod 451 nombre-del-archivo`

Así es como realizamos el cálculo:

![Desglose del cálculo para agregar permisos](https://www.freecodecamp.org/news/content/images/2022/04/image-163.png)

Tenga en cuenta que esto es lo mismo que `r--r-x--x`.

-   Eliminar derechos de `ejecución` de `otros` y `grupo`.

Para eliminar la ejecución de `otros` y `grupo`, resta 1 de la parte de ejecución de los últimos 2 octetos.

![Desglose del cálculo para eliminar permisos](https://www.freecodecamp.org/news/content/images/2022/04/image-164.png)

-   Asignar `lectura`, `escritura` y `ejecución` a `usuario`, `lectura` y `ejecución` a `grupo` y solo `lectura` a otros.

Esto sería lo mismo que `rwxr-xr--`.

![Desglose del cálculo para agregar permisos](https://www.freecodecamp.org/news/content/images/2022/04/image-165.png)

##### Cómo cambiar la propiedad usando el comando `chown`

Sintaxis de `chown`:

```
chown usuario nombre_archivo
```

##### Cómo cambiar la propiedad de usuario con `chown`

Vamos a transferir la propiedad del usuario `zaira` al usuario `news`.

`chown news mymotd.sh`

![ver propietario actual](https://www.freecodecamp.org/news/content/images/2022/04/image-167.png)

Comando para cambiar la propiedad: `sudo chown news mymotd.sh`.

**Salida:**

![Propiedad cambiada](https://www.freecodecamp.org/news/content/images/2022/04/image-168.png)

##### Cómo cambiar simultáneamente la propiedad de usuario y grupo

También podemos usar `chown` para cambiar el usuario y el grupo simultáneamente.

```
chown usuario:grupo nombre_archivo
```

##### Cómo cambiar la propiedad de un directorio

Puede cambiar la propiedad de manera recursiva para los contenidos en un directorio. El ejemplo a continuación cambia la propiedad de la carpeta `/opt/script` para permitir al usuario `admin`.

```
chown -R admin /opt/script
```

##### Cómo cambiar la propiedad del grupo

En caso de que solo necesitemos cambiar el propietario del grupo, podemos usar `chown` precediendo el nombre del grupo con dos puntos `:`

```
chown :admins /opt/script
```

##### Cómo cambiar entre usuarios

Puede cambiar entre usuarios usando el comando `su`.

```
[user01@host ~]$ su user02
Contraseña:
[user02@host ~]$
```

##### Cómo obtener acceso de superusuario

El superusuario o el usuario root tiene el nivel más alto de acceso en un sistema Linux. El usuario root puede realizar cualquier operación en el sistema. El usuario root puede acceder a todos los archivos y directorios, instalar y eliminar software, y modificar o sobrescribir configuraciones del sistema.

Con gran poder viene gran responsabilidad. Si el usuario root se ve comprometido, alguien puede ganar control completo sobre el sistema. Se aconseja usar la cuenta del usuario root solo cuando sea necesario.

Si omite el nombre de usuario, el comando `su` cambia a la cuenta del usuario root por defecto.

```
[user01@host ~]$ su
Contraseña:
[root@host ~]#
```

Otra variación del comando `su` es `su -`. El comando `su` cambia a la cuenta del usuario root pero no cambia las variables de entorno. El comando `su -` cambia a la cuenta del usuario root y cambia las variables de entorno a las del usuario objetivo.

##### Ejecución de comandos con sudo

Para ejecutar comandos como el usuario `root` sin cambiar a la cuenta del usuario `root`, puede usar el comando `sudo`. El comando `sudo` permite ejecutar comandos con privilegios elevados.

Ejecutar comandos con `sudo` es una opción más segura en lugar de ejecutar los comandos como el usuario `root`. Esto se debe a que solo un conjunto específico de usuarios puede tener permiso para ejecutar comandos con `sudo`. Esto está definido en el archivo `/etc/sudoers`.

Además, `sudo` registra todos los comandos que se ejecutan con él, proporcionando una pista de auditoría de quién ejecutó qué comandos y cuándo.

En Ubuntu, puede encontrar los registros de auditoría aquí:

```
cat /var/log/auth.log | grep sudo
```

Para un usuario que no tiene acceso a `sudo`, se señala en los registros y muestra un mensaje como este:

```
user01 no está en el archivo sudoers. Este incidente será reportado.
```

#### Gestión de cuentas de usuario locales

##### Creación de usuarios desde la línea de comandos

El comando utilizado para agregar un nuevo usuario es:

```
sudo useradd nombre_de_usuario
```

Este comando configura el directorio personal del usuario y crea un grupo privado designado por el nombre de usuario del usuario. Actualmente, la cuenta carece de una contraseña válida, lo que impide que el usuario inicie sesión hasta que se cree una contraseña.

##### Modificación de usuarios existentes

El comando `usermod` se utiliza para modificar usuarios existentes. Aquí hay algunas de las opciones más comunes usadas con el comando `usermod`:

Aquí hay algunos ejemplos del comando `usermod` en Linux:

1.  **Cambiar el nombre de inicio de sesión de un usuario:**
    
    ```
    sudo usermod -l nuevonombre antiguo_nombre_de_usuario
    ```
    
2.  **Cambiar el directorio personal de un usuario:**
    
    ```
    sudo usermod -d /nuevo/directorio/personal -m nombre_de_usuario
    ```
    
3.  **Agregar un usuario a un grupo complementario:**
    
    ```
    sudo usermod -aG nombre_del_grupo nombre_de_usuario
    ```
    
4.  **Cambiar el shell de un usuario:**
    
    ```
    sudo usermod -s /bin/bash nombre_de_usuario
    ```
    
5.  **Bloquear la cuenta de un usuario:**
    
    ```
    sudo usermod -L nombre_de_usuario
    ```
    
6.  **Desbloquear la cuenta de un usuario:**
    
    ```
    sudo usermod -U nombre_de_usuario
    ```
    
7.  **Establecer una fecha de expiración para una cuenta de usuario:**
    
    ```
    sudo usermod -e AAAA-MM-DD nombre_de_usuario
    ```
    
8.  **Cambiar el ID de usuario (UID) de un usuario:**
    
    ```
    sudo usermod -u nuevoUID nombre_de_usuario
    ```
    
9.  **Cambiar el grupo principal de un usuario:**
    
    ```
    sudo usermod -g nuevogrupo nombre_de_usuario
    ```
    
10.  **Eliminar a un usuario de un grupo complementario:**
    
    ```
    sudo gpasswd -d nombre_de_usuario nombre_del_grupo
    ```
    

##### Eliminación de usuarios

El comando `userdel` se utiliza para eliminar una cuenta de usuario y archivos relacionados del sistema.

-   `sudo userdel nombre_de_usuario`: elimina los detalles del usuario de `/etc/passwd` pero mantiene el directorio personal del usuario.
    
-   El comando `sudo userdel -r nombre_de_usuario` elimina los detalles del usuario de `/etc/passwd` y también elimina el directorio personal del usuario.
    

##### Cambio de contraseñas de usuario

El comando `passwd` se utiliza para cambiar la contraseña de un usuario.

-   `sudo passwd nombre_de_usuario`: establece la contraseña inicial o cambia la existente de nombre_de_usuario. También se utiliza para cambiar la contraseña del usuario actualmente conectado.

El acceso a servidores remotos es una de las tareas esenciales para los administradores de sistemas. Puedes conectarte a diferentes servidores o acceder a bases de datos a través de tu máquina local y ejecutar comandos, todo utilizando SSH.

**¿Qué es el protocolo SSH?**

SSH significa Secure Shell. Es un protocolo de red criptográfico que permite una comunicación segura entre dos sistemas.

El puerto predeterminado para SSH es `22`.

Los dos participantes durante la comunicación vía SSH son:

-   El servidor: la máquina a la que quieres acceder.
    
-   El cliente: el sistema desde el que estás accediendo al servidor.
    

La conexión a un servidor sigue estos pasos:

1.  Iniciar Conexión: El cliente envía una solicitud de conexión al servidor.
    
2.  Intercambio de Llaves: El servidor envía su llave pública al cliente. Ambos acuerdan los métodos de encriptación a usar.
    
3.  Generación de Llave de Sesión: El cliente y el servidor usan el intercambio de llaves Diffie-Hellman para crear una llave de sesión compartida.
    
4.  Autenticación del Cliente: El cliente inicia sesión en el servidor usando una contraseña, llave privada, u otro método.
    
5.  Comunicación Segura: Después de la autenticación, el cliente y el servidor se comunican de forma segura con encriptación.
    

**¿Cómo conectarse a un servidor remoto usando SSH?**

El comando `ssh` es una utilidad incorporada en Linux y también la predeterminada. Hace que el acceso a servidores sea bastante fácil y seguro.

Aquí, estamos hablando de cómo el cliente establecería una conexión con el servidor.

Antes de conectarte a un servidor, necesitas tener la siguiente información:

-   La dirección IP o el nombre de dominio del servidor.
    
-   El nombre de usuario y la contraseña del servidor.
    
-   El número de puerto al que tienes acceso en el servidor.
    

La sintaxis básica del comando `ssh` es:

```
ssh usuario@ip_servidor
```

Por ejemplo, si tu nombre de usuario es `john` y la IP del servidor es `192.168.1.10`, el comando sería:

```
ssh john@192.168.1.10
```

Después de eso, se te pedirá que ingreses la contraseña secreta. Tu pantalla se verá similar a esto:

```
john@192.168.1.10's password: 
Welcome to Ubuntu 20.04.2 LTS (GNU/Linux 5.4.0-70-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Fri Jun  5 10:17:32 UTC 2024

  System load:  0.08               Processes:           122
  Usage of /:   12.3% of 19.56GB   Users logged in:     1
  Memory usage: 53%                IP address for eth0: 192.168.1.10
  Swap usage:   0%

Last login: Fri Jun  5 09:34:56 2024 from 192.168.1.2
john@hostname:~$ # empieza a ingresar comandos
```

Ahora puedes ejecutar los comandos pertinentes en el servidor `192.168.1.10`.

⚠️ El puerto predeterminado para ssh es `22`, pero también es vulnerable, ya que los hackers probablemente intentarán aquí primero. Tu servidor puede exponer otro puerto y compartir el acceso contigo. Para conectarse a un puerto diferente, usa el indicador `-p`.

```
ssh -p número_de_puerto usuario@ip_servidor
```

### 8.3. Análisis y Parsing Avanzado de Logs

Los archivos de log, cuando están configurados, son generados por tu sistema por varias razones útiles. Pueden ser usados para rastrear eventos del sistema, monitorizar el rendimiento del sistema, y solucionar problemas. Son específicamente útiles para los administradores de sistemas donde pueden rastrear errores de aplicaciones, eventos de red, y actividad de usuarios.

Aquí hay un ejemplo de un archivo de log:

```
# archivo de log de muestra
2024-04-25 09:00:00 INFO Inicio: Aplicación iniciando
2024-04-25 09:01:00 INFO Configuración: Configuración cargada exitosamente
2024-04-25 09:02:00 DEBUG Base de Datos: Conexión a la base de datos establecida
2024-04-25 09:03:00 INFO Usuario: Nuevo usuario registrado (ID de Usuario: 1001)
2024-04-25 09:04:00 WARN Seguridad: Intento de inicio de sesión con credenciales incorrectas (ID de Usuario: 1001)
2024-04-25 09:05:00 ERROR Red: Tiempo de espera de red agotado en la solicitud (ID de Solicitud: 456)
2024-04-25 09:06:00 INFO Email: Correo de notificación enviado (ID de Usuario: 1001)
2024-04-25 09:07:00 DEBUG API: Llamada API con tiempo de respuesta sobre el umbral (Duración: 350ms)
2024-04-25 09:08:00 INFO Sesión: Sesión de usuario finalizada (ID de Usuario: 1001)
2024-04-25 09:09:00 INFO Apagado: Apagado de la aplicación iniciado
```

Un archivo de log usualmente contiene las siguientes columnas:

-   Timestamp: La fecha y la hora cuando ocurrió el evento.
    
-   Nivel de Log: La gravedad del evento (INFO, DEBUG, WARN, ERROR).
    
-   Componente: El componente del sistema que generó el evento (Inicio, Configuración, Base de Datos, Usuario, Seguridad, Red, Email, API, Sesión, Apagado).
    
-   Mensaje: Una descripción del evento que ocurrió.
    
-   Información Adicional: Información adicional relacionada con el evento.
    

En sistemas en tiempo real, los archivos de log tienden a ser de miles de líneas de largo y se generan cada segundo. Pueden ser muy verbosos dependiendo de la configuración. Cada columna en un archivo de log es una pieza de información que puede ser usada para rastrear problemas. Esto hace que los archivos de log sean difíciles de leer y entender manualmente.

Aquí es donde entra el parsing de logs. El parsing de logs es el proceso de extraer información útil de los archivos de log. Involucra descomponer los archivos de log en piezas más pequeñas y manejables, y extraer la información relevante.

En esta sección, explorarás algunas técnicas para analizar archivos de registro en Linux.

#### Extracción de texto usando `grep`

Grep es una utilidad integrada en bash. Significa "global regular expression print". Grep se utiliza para coincidir cadenas en archivos.

Aquí hay algunos usos comunes de `grep`:

1.  **Buscar una cadena específica en un archivo:**
    
    ```
     grep "cadena_buscar" nombre_archivo
    ```
    
    Este comando busca "cadena\_buscar" en el archivo llamado `nombre_archivo`.
    
2.  **Buscar recursivamente en directorios:**
    
    ```
     grep -r "cadena_buscar" /ruta/del/directorio
    ```
    
    Este comando busca "cadena_buscar" en todos los archivos dentro del directorio especificado y sus subdirectorios.
    
3.  **Ignorar mayúsculas y minúsculas al buscar:**
    
    ```
     grep -i "cadena_buscar" nombre_archivo
    ```
    
    Este comando realiza una búsqueda insensible a mayúsculas y minúsculas de "cadena\_buscar" en el archivo llamado `nombre_archivo`.
    
4.  **Mostrar números de línea con líneas coincidentes:**
    
    ```
     grep -n "cadena_buscar" nombre_archivo
    ```
    
    Este comando muestra los números de línea junto con las líneas coincidentes en el archivo llamado `nombre_archivo`.
    
5.  **Contar el número de líneas coincidentes:**
    
    ```
     grep -c "cadena_buscar" nombre_archivo
    ```
    
    Este comando cuenta el número de líneas que contienen "cadena\_buscar" en el archivo llamado `nombre_archivo`.
    
6.  **Invertir coincidencias para mostrar líneas que no coinciden:**
    
    ```
     grep -v "cadena_buscar" nombre_archivo
    ```
    
    Este comando muestra todas las líneas que no contienen "cadena\_buscar" en el archivo llamado `nombre_archivo`.
    
7.  **Buscar una palabra completa:**
    
    ```
     grep -w "palabra" nombre_archivo
    ```
    
    Este comando busca la palabra completa "palabra" en el archivo llamado `nombre_archivo`.
    
8.  **Usar expresiones regulares extendidas:**
    
    ```
     grep -E "patrón" nombre_archivo
    ```
    
    Este comando permite el uso de expresiones regulares extendidas para una coincidencia de patrones más compleja en el archivo llamado `nombre_archivo`.
    

**💡 Consejo:** Si hay múltiples archivos en una carpeta, puedes usar el siguiente comando para encontrar la lista de archivos que contienen las cadenas deseadas.

```
# encuentra la lista de archivos que contienen las cadenas deseadas
grep -l "Cadena a Coincidir" /ruta/del/directorio
```

#### Extracción de texto usando `sed`

`sed` significa "stream editor" (editor de flujo). Procesa datos de forma secuencial, lo que significa que lee los datos una línea a la vez. `sed` te permite buscar patrones y realizar acciones en las líneas que coinciden con esos patrones.

**Sintaxis básica de** `sed`:

La sintaxis básica de `sed` es la siguiente:

```
sed [opciones] 'comando' nombre_archivo
```

Aquí, `comando` se usa para realizar operaciones como sustitución, eliminación, inserción, etc., en los datos de texto. El nombre del archivo es el nombre del archivo que deseas procesar.

**Uso de `sed`:**

**1\. Sustitución:**

La bandera `s` se utiliza para reemplazar texto. El `texto_viejo` se reemplaza con `texto_nuevo`:

```
sed 's/texto_viejo/texto_nuevo/' nombre_archivo
```

Por ejemplo, para cambiar todas las instancias de "error" a "advertencia" en el archivo de registro `system.log`:

```
sed 's/error/advertencia/' system.log
```

**2\. Imprimir líneas que contienen un patrón específico:**

Usar `sed` para filtrar y mostrar líneas que coinciden con un patrón específico:

```
sed -n '/patrón/p' nombre_archivo
```

Por ejemplo, para encontrar todas las líneas que contienen "ERROR":

```
sed -n '/ERROR/p' system.log
```

**3\. Eliminar líneas que contienen un patrón específico:**

Puedes eliminar líneas de la salida que coinciden con un patrón específico:

```
sed '/patrón/d' nombre_archivo
```

Por ejemplo, para eliminar todas las líneas que contienen "DEBUG":

```
sed '/DEBUG/d' system.log
```

**4\. Extraer campos específicos de una línea de registro:**

Puedes usar expresiones regulares para extraer partes de líneas. Supongamos que cada línea de registro comienza con una fecha en el formato "YYYY-MM-DD". Podrías extraer solo la fecha de cada línea:

```
sed -n 's/^\([0-9]\{4\}-[0-9]\{2\}-[0-9]\{2\}\).*/\1/p' system.log
```

#### Análisis de texto con `awk`

`awk` tiene la capacidad de dividir fácilmente cada línea en campos. Está bien diseñado para procesar texto estructurado como archivos de registro.

**Sintaxis básica de** `awk`

La sintaxis básica de `awk` es:

```
awk 'patrón { acción }' nombre_archivo
```

Aquí, `patrón` es una condición que debe cumplirse para que la `acción` sea ejecutada. Si se omite el patrón, la acción se realiza en cada línea.

En los ejemplos siguientes, utilizarás este archivo de registro como ejemplo:

```
2024-04-25 09:00:00 INFO Inicio: Aplicación iniciando
2024-04-25 09:01:00 INFO Configuración: Configuración cargada correctamente
2024-04-25 09:02:00 INFO Base de datos: Conexión a la base de datos establecida
2024-04-25 09:03:00 INFO Usuario: Nuevo usuario registrado (UserID: 1001)
2024-04-25 09:04:00 INFO Seguridad: Intento de inicio de sesión con credenciales incorrectas (UserID: 1001)
2024-04-25 09:05:00 INFO Red: Tiempo de espera de red en solicitud (ReqID: 456)
2024-04-25 09:06:00 INFO Correo: Correo de notificación enviado (UserID: 1001)
2024-04-25 09:07:00 INFO API: Llamada a la API con tiempo de respuesta superior al umbral (Duración: 350ms)
2024-04-25 09:08:00 INFO Sesión: Sesión de usuario terminada (UserID: 1001)
2024-04-25 09:09:00 INFO Apagado: Inicio de apagado de la aplicación
  INFO
```

-   **Acceder a columnas usando** `awk`

```
zaira@zaira-ThinkPad:~$ awk '{ print $1 }' sample.log
# salida
2024-04-25
2024-04-25
2024-04-25
2024-04-25
2024-04-25
2024-04-25
2024-04-25
2024-04-25
2024-04-25
2024-04-25

zaira@zaira-ThinkPad:~$ awk '{ print $2 }' sample.log
# salida
09:00:00
09:01:00
09:02:00
09:03:00
09:04:00
09:05:00
09:06:00
09:07:00
09:08:00
09:09:00
```

-   **Imprimir líneas que contienen un patrón específico (por ejemplo, ERROR)**

```
awk '/ERROR/ { print $0 }' logfile.log

# salida
2024-04-25 09:05:00 ERROR Network: Network timeout on request (ReqID: 456)
```

Esto imprime todas las líneas que contienen "ERROR".

-   **Extraer el primer campo (Fecha y Hora)**

```
awk '{ print $1, $2 }' logfile.log
# salida
2024-04-25 09:00:00
2024-04-25 09:01:00
2024-04-25 09:02:00
2024-04-25 09:03:00
2024-04-25 09:04:00
2024-04-25 09:05:00
2024-04-25 09:06:00
2024-04-25 09:07:00
2024-04-25 09:08:007
2024-04-25 09:09:00
```

Esto extraerá los dos primeros campos de cada línea, que en este caso serían la fecha y la hora.

-   **Resumir ocurrencias de cada nivel de registro**

```
awk '{ count[$3]++ } END { for (level in count) print level, count[level] }' logfile.log

# salida
 1
WARN 1
ERROR 1
DEBUG 2
INFO 6
```

La salida será un resumen del número de ocurrencias de cada nivel de registro.

-   **Filtrar campos específicos (por ejemplo, donde el tercer campo es INFO)**

```
awk '{ $3="INFO"; print }' sample.log

# salida
2024-04-25 09:00:00 INFO Startup: Application starting
2024-04-25 09:01:00 INFO Config: Configuration loaded successfully
2024-04-25 09:02:00 INFO Database: Database connection established
2024-04-25 09:03:00 INFO User: New user registered (UserID: 1001)
2024-04-25 09:04:00 INFO Security: Attempted login with incorrect credentials (UserID: 1001)
2024-04-25 09:05:00 INFO Network: Network timeout on request (ReqID: 456)
2024-04-25 09:06:00 INFO Email: Notification email sent (UserID: 1001)
2024-04-25 09:07:00 INFO API: API call with response time over threshold (Duration: 350ms)
2024-04-25 09:08:00 INFO Session: User session ended (UserID: 1001)
2024-04-25 09:09:00 INFO Shutdown: Application shutdown initiated
  INFO
```

Este comando extraerá todas las líneas donde el tercer campo es "INFO".

💡 **Consejo:** El separador predeterminado en `awk` es un espacio. Si tu archivo de registro utiliza un separador diferente, puedes especificarlo usando la opción `-F`. Por ejemplo, si tu archivo de registro usa dos puntos como separador, puedes usar `awk -F: '{ print $1 }' logfile.log` para extraer el primer campo.

#### Análisis de archivos de registro con `cut`

El comando `cut` es un comando simple pero potente utilizado para extraer secciones de texto de cada línea de entrada. Como los archivos de registro están estructurados y cada campo está delimitado por un carácter específico, como un espacio, tabulación, o un delimitador personalizado, `cut` hace un muy buen trabajo al extraer esos campos específicos.

La sintaxis básica del comando cut es:

```
cut [opciones] [archivo]
```

Algunas opciones comúnmente usadas para el comando cut:

-   `-d` : Especifica un delimitador utilizado como separador de campos.
    
-   `-f` : Selecciona los campos que se mostrarán.
    
-   `-c` : Especifica posiciones de caracteres.
    

Por ejemplo, el siguiente comando extraería el primer campo (separado por un espacio) de cada línea del archivo de registro:

```
cut -d ' ' -f 1 logfile.log
```

**Ejemplos de uso de**`cut`**para análisis de registros**

Supongamos que tienes un archivo de registro estructurado de la siguiente manera, donde los campos están separados por espacios:

```
2024-04-25 08:23:01 INFO 192.168.1.10 User logged in successfully.
2024-04-25 08:24:15 WARNING 192.168.1.10 Disk usage exceeds 90%.
2024-04-25 08:25:02 ERROR 10.0.0.5 Connection timed out.
...
```

`cut` puede ser usado de las siguientes maneras:

1.  **Extrayendo la hora de cada entrada de registro**:

```
cut -d ' ' -f 2 system.log

# Salida
08:23:01
08:24:15
08:25:02
...
```

Este comando usa un espacio como delimitador y selecciona el segundo campo, que es el componente de la hora de cada entrada de registro.

2.  **Extrayendo las direcciones IP de los registros**:

```
cut -d ' ' -f 4 system.log

# Salida
192.168.1.10
192.168.1.10
10.0.0.5
```

Este comando extrae el cuarto campo, que es la dirección IP de cada entrada de registro.

3.  **Extrayendo los niveles de registro (INFO, WARNING, ERROR)**:

```
cut -d ' ' -f 3 system.log

# Salida
INFO
WARNING
ERROR
```

Este extrae el tercer campo que contiene el nivel de registro.

4.  **Combinando**`cut`**con otros comandos:**

La salida de otros comandos puede ser pasada a `cut`. Supongamos que quieres filtrar los registros antes de cortar. Puedes usar `grep` para extraer líneas que contienen "ERROR" y luego usar `cut` para obtener información específica de esas líneas:

```
grep "ERROR" system.log | cut -d ' ' -f 1,2 

# Salida
2024-04-25 08:25:02
```

Este comando primero filtra las líneas que incluyen "ERROR", luego extrae la fecha y la hora de esas líneas.

5.  **Extrayendo múltiples campos**:

Es posible extraer múltiples campos a la vez especificando un rango o una lista separada por comas de los campos:

```
cut -d ' ' -f 1,2,3 system.log` 

# Salida
2024-04-25 08:23:01 INFO
2024-04-25 08:24:15 WARNING
2024-04-25 08:25:02 ERROR
...
```

El comando anterior extrae los tres primeros campos de cada entrada de registro, que son la fecha, la hora y el nivel de registro.
```

Ordenar y eliminar duplicados son operaciones comunes al trabajar con archivos de registro. Los comandos `sort` y `uniq` son comandos poderosos utilizados para ordenar y eliminar duplicados de la entrada, respectivamente.

**Sintaxis básica de sort**

El comando `sort` organiza líneas de texto alfabéticamente o numéricamente.

```
sort [opciones] [archivo]
```

Algunas opciones clave para el comando sort:

-   `-n`: Ordena el archivo asumiendo que el contenido es numérico.
    
-   `-r`: Invierte el orden de la clasificación.
    
-   `-k`: Especifica una clave o número de columna para ordenar.
    
-   `-u`: Ordena y elimina líneas duplicadas.
    

El comando `uniq` se utiliza para filtrar o contar y reportar líneas repetidas en un archivo.

La sintaxis de `uniq` es:

```
uniq [opciones] [archivo_entrada] [archivo_salida]
```

Algunas opciones clave para el comando `uniq` son:

-   `-c`: Prefija las líneas con el número de ocurrencias.
    
-   `-d`: Imprime solo las líneas duplicadas.
    
-   `-u`: Imprime solo las líneas únicas.
    

#### Ejemplos de uso de `sort` y `uniq` juntos para el análisis de registros

Supongamos las siguientes entradas de registro de ejemplo para estas demostraciones:

```
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-25 WARNING Uso de disco supera el 90%.
2024-04-26 ERROR Conexión agotada.
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-26 INFO Mantenimiento programado.
2024-04-26 ERROR Conexión agotada.
```

1.  **Ordenar entradas de registro por fecha**:

```
sort system.log

# Salida
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-25 WARNING Uso de disco supera el 90%.
2024-04-26 ERROR Conexión agotada.
2024-04-26 ERROR Conexión agotada.
2024-04-26 INFO Mantenimiento programado.
```

Esto ordena las entradas del registro alfabéticamente, lo que efectivamente las ordena por fecha si la fecha es el primer campo.

1.  **Ordenar y eliminar duplicados**:

```
sort system.log | uniq

# Salida
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-25 WARNING Uso de disco supera el 90%.
2024-04-26 ERROR Conexión agotada.
2024-04-26 INFO Mantenimiento programado.
```

Este comando ordena el archivo de registro y lo pasa a `uniq`, eliminando líneas duplicadas.

1.  **Contar ocurrencias de cada línea**:

```
sort system.log | uniq -c

# Salida
2 2024-04-25 INFO Usuario inició sesión exitosamente.
1 2024-04-25 WARNING Uso de disco supera el 90%.
2 2024-04-26 ERROR Conexión agotada.
1 2024-04-26 INFO Mantenimiento programado.
```

Ordena las entradas del registro y luego cuenta cada línea única. Según la salida, la línea `'2024-04-25 INFO Usuario inició sesión exitosamente.'` apareció 2 veces en el archivo.

1.  **Identificar entradas de registro únicas**:

```
sort system.log | uniq -u

# Salida

2024-04-25 WARNING Uso de disco supera el 90%.
2024-04-26 INFO Mantenimiento programado.
```

Este comando muestra líneas que son únicas.

2.  **Ordenar por nivel de registro**:

```
sort -k2 system.log

# Salida
2024-04-26 ERROR Conexión agotada.
2024-04-26 ERROR Conexión agotada.
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-25 INFO Usuario inició sesión exitosamente.
2024-04-26 INFO Mantenimiento programado.
2024-04-25 WARNING Uso de disco supera el 90%.
```

Ordena las entradas en función del segundo campo, que es el nivel de registro.

### 8.4. Gestionar Procesos de Linux desde la Línea de Comandos

Un proceso es una instancia en ejecución de un programa. Un proceso consta de:

-   Un espacio de direcciones de la memoria asignada.
    
-   Estados del proceso.
    
-   Propiedades como la propiedad, atributos de seguridad y uso de recursos.
    

Un proceso también tiene un entorno que consta de:

-   Variables locales y globales.
    
-   El contexto de planificación actual
    
-   Recursos del sistema asignados, como puertos de red o descriptores de archivos.
    

Cuando ejecutas el comando `ls -l`, el sistema operativo crea un nuevo proceso para ejecutar el comando. El proceso tiene un ID, un estado y se ejecuta hasta que el comando se completa.

#### Entendiendo la creación y el ciclo de vida del proceso

En Ubuntu, todos los procesos se originan desde el proceso inicial del sistema llamado `systemd`, que es el primer proceso iniciado por el kernel durante el arranque.

El proceso `systemd` tiene un ID de proceso (PID) de `1` y es responsable de inicializar el sistema, iniciar y gestionar otros procesos, y manejar servicios del sistema. Todos los demás procesos en el sistema son descendientes de `systemd`.

Un proceso padre duplica su propio espacio de direcciones (fork) para crear una nueva estructura de proceso (hijo). A cada nuevo proceso se le asigna un ID de proceso único (PID) para fines de seguimiento y seguridad. El PID y el ID del proceso padre (PPID) son parte del nuevo entorno de proceso. Cualquier proceso puede crear un proceso hijo.

![Proceso y su inicialización al proceso padre e hijo](https://cdn.hashnode.com/res/hashnode/image/upload/v1719584071059/f24fac4b-18f3-4a39-8659-93d32c533256.png)

A través de la rutina fork, un proceso hijo hereda identidades de seguridad, descriptores de archivos anteriores y actuales, privilegios de puerto y recursos, variables de entorno y código de programa. Un proceso hijo puede entonces ejecutar su propio código de programa.

Típicamente, un proceso padre duerme mientras el proceso hijo se ejecuta, poniendo una solicitud (wait) para ser notificado cuando el hijo se complete.

Al salir, el proceso hijo ya ha cerrado o descartado sus recursos y entorno. El único recurso restante, conocido como zombi, es una entrada en la tabla de procesos. El padre, señalizado al despertar cuando el hijo sale, limpia la tabla de procesos de la entrada del hijo, liberando así el último recurso del proceso hijo. El proceso padre entonces continúa ejecutando su propio código de programa.

Los procesos en Linux asumen diferentes estados durante su ciclo de vida. El estado de un proceso indica lo que el proceso está haciendo actualmente y cómo está interactuando con el sistema. Los procesos cambian de estado según su estado de ejecución y el algoritmo de planificación del sistema.

![Estados y transiciones de procesos en Linux](https://cdn.hashnode.com/res/hashnode/image/upload/v1719584116150/3054dfe2-c42c-4d62-9e12-e3aec479d53a.png)

Los procesos en un sistema Linux pueden estar en uno de los siguientes estados:

| **Estado** | **Descripción** |
| --- | --- |
| **(nuevo)** | Estado inicial cuando se crea un proceso mediante una llamada al sistema fork. |
| **Ejecutable (listo) (R)** | El proceso está listo para ejecutarse y esperando ser programado en una CPU. |
| **Ejecutando (usuario) (R)** | El proceso se está ejecutando en modo usuario, ejecutando aplicaciones de usuario. |
| **Ejecutando (kernel) (R)** | El proceso se está ejecutando en modo kernel, manejando llamadas al sistema o interrupciones de hardware. |
| **Durmiendo (S)** | El proceso está esperando a que se complete un evento (por ejemplo, una operación de E/S) y puede despertarse fácilmente. |
| **Durmiendo (ininterrumpido) (D)** | El proceso está en un estado de sueño ininterrumpido, esperando a que se complete una condición específica (generalmente E/S) y no puede ser interrumpido por señales. |
| **Durmiendo (durmiendo por disco) (K)** | El proceso está esperando a que se completen las operaciones de E/S del disco. |
| **Durmiendo (inactivo) (I)** | El proceso está inactivo, no está haciendo ningún trabajo y está esperando a que ocurra un evento. |
| **Detenido (T)** | La ejecución del proceso se ha detenido, típicamente por una señal, y puede reanudarse más tarde. |
| **Zombi (Z)** | El proceso ha completado su ejecución pero aún tiene una entrada en la tabla de procesos, esperando a que su padre lea su estado de salida. |

Los procesos cambian entre estos estados de las siguientes maneras:

| **Transición** | **Descripción** |
| --- | --- |
| **Fork** | Crea un nuevo proceso a partir de un proceso padre, cambiando de (nuevo) a Ejecutable (listo) (R). |
| **Planificación** | El planificador selecciona un proceso ejecutable, cambiándolo a Ejecutando (usuario) o Ejecutando (kernel). |
| **Ejecutar** | El proceso cambia de Ejecutable (listo) (R) a Ejecutando (kernel) (R) cuando se programa para su ejecución. |
| **Preempción o Reprogramación** | El proceso puede ser preempcionado o reprogramado, moviéndolo de nuevo a Ejecutable (listo) (R). |
| **Llamada al sistema** | El proceso realiza una llamada al sistema, cambiando de Ejecutando (usuario) (R) a Ejecutando (kernel) (R). |
| **Retorno** | El proceso completa una llamada al sistema y regresa a Ejecutando (usuario) (R). |
| **Esperar** | El proceso espera un evento, cambiando de Ejecutando (kernel) (R) a uno de los estados de Durmiendo (S, D, K, o I). |
| **Evento o Señal** | El proceso es despertado por un evento o señal, moviéndolo de un estado de Durmiendo de vuelta a Ejecutable (listo) (R). |
| **Suspender** | El proceso está suspendido, cambiando de Ejecutando (kernel) o Ejecutable (listo) a Detenido (T). |
| **Reanudar** | El proceso se reanuda, moviéndose de Detenido (T) de vuelta a Ejecutable (listo) (R). |
| **Salir** | El proceso termina, cambiando de Ejecutando (usuario) o Ejecutando (kernel) a Zombi (Z). |
| **Recolectar** | El proceso padre lee el estado de salida del proceso zombi, eliminándolo de la tabla de procesos. |

#### Cómo ver los procesos

Puedes usar el comando `ps` junto con una combinación de opciones para ver los procesos en un sistema Linux. El comando `ps` se utiliza para mostrar información sobre una selección de procesos activos. Por ejemplo, `ps aux` muestra todos los procesos que se están ejecutando en el sistema.

```
zaira@zaira:~$ ps aux
# Salida
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0 168140 11352 ?        Ss   May21   0:18 /sbin/init splash
root           2  0.0  0.0      0     0 ?        S    May21   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        I<   May21   0:00 [rcu_gp]
root           4  0.0  0.0      0     0 ?        I<   May21   0:00 [rcu_par_gp]
root           5  0.0  0.0      0     0 ?        I<   May21   0:00 [slub_flushwq]
root           6  0.0  0.0      0     0 ?        I<   May21   0:00 [netns]
root          11  0.0  0.0      0     0 ?        I<   May21   0:00 [mm_percpu_wq]
root          12  0.0  0.0      0     0 ?        I    May21   0:00 [rcu_tasks_kthread]
root          13  0.0  0.0      0     0 ?        I    May21   0:00 [rcu_tasks_rude_kthread]
*... salida truncada ....*
```

La salida anterior muestra una instantánea de los procesos que se están ejecutando actualmente en el sistema. Cada fila representa un proceso con las siguientes columnas:

1.  `USER`: El usuario que posee el proceso.
    
2.  `PID`: El ID del proceso.
    
3.  `%CPU`: El uso de CPU del proceso.
    
4.  `%MEM`: El uso de memoria del proceso.
    
5.  `VSZ`: El tamaño de la memoria virtual del proceso.
    
6.  `RSS`: El tamaño del conjunto residente, es decir, la memoria física no intercambiada que una tarea ha utilizado.
    
7.  `TTY`: El terminal de control del proceso. Un `?` indica que no tiene terminal de control.
    
8.  `STAT`: El estado del proceso.
    
    -   `R`: Ejecutando
        
    -   `I` o `S`: Sueño interrumpible (esperando a que se complete un evento)
        
    -   `D`: Sueño ininterrumpible (generalmente E/S)
        
    -   `T`: Detenido (ya sea por una señal de control de trabajo o porque está siendo rastreado)
        
    -   `Z`: Zombi (terminado pero no recolectado por su padre)
        
    -   `Ss`: Líder de sesión. Este es un proceso que ha iniciado una sesión y es un líder de un grupo de procesos y puede controlar señales de terminal. La primera `S` indica el estado de sueño, y la segunda `s` indica que es un líder de sesión.
        
9.  `START`: El tiempo o la fecha de inicio del proceso.
    
10.  `TIME`: El tiempo acumulado de CPU.
    
11.  `COMMAND`: El comando que inició el proceso.

En esta sección, aprenderás cómo puedes controlar los trabajos ejecutándolos en segundo plano o en primer plano.

Un trabajo es un proceso que es iniciado por una shell. Cuando ejecutas un comando en la terminal, se considera un trabajo. Un trabajo puede ejecutarse en primer plano o en segundo plano.

Para demostrar el control, primero crearás 3 procesos y luego los ejecutarás en segundo plano. Después de eso, enumerarás los procesos y los alternarás entre el primer plano y el segundo plano. Verás cómo ponerlos en suspensión o salir completamente.

1.  Crear Tres Procesos

Abre una terminal y inicia tres procesos de larga duración. Usa el comando `sleep`, que mantiene el proceso en ejecución durante un número específico de segundos.

```
# ejecuta el comando sleep por 300, 400 y 500 segundos
sleep 300 &
sleep 400 &
sleep 500 &
```

El `&` al final de cada comando mueve el proceso al segundo plano.

2.  Mostrar Trabajos en Segundo Plano

Usa el comando `jobs` para mostrar la lista de trabajos en segundo plano.

```
jobs
```

El resultado debería verse algo como esto:

```
jobs
[1]   Running                 sleep 300 &
[2]-  Running                 sleep 400 &
[3]+  Running                 sleep 500 &
```

3.  Traer un Trabajo en Segundo Plano al Primer Plano

Para traer un trabajo en segundo plano al primer plano, usa el comando `fg` seguido del número del trabajo. Por ejemplo, para traer el primer trabajo (`sleep 300`) al primer plano:

```
fg %1
```

Esto traerá el trabajo `1` al primer plano.

4.  Mover el Trabajo en Primer Plano de Nuevo al Segundo Plano

Mientras el trabajo se está ejecutando en el primer plano, puedes suspenderlo y moverlo de nuevo al segundo plano presionando `Ctrl+Z` para suspender el trabajo.

Un trabajo suspendido se verá así:

```
zaira@zaira:~$ fg %1
sleep 300

^Z
[1]+  Stopped                 sleep 300

zaira@zaira:~$ jobs
# trabajo suspendido 
[1]+  Stopped                 sleep 300
[2]   Running                 sleep 400 &
[3]-  Running                 sleep 500 &
```

Ahora usa el comando `bg` para reanudar el trabajo con ID 1 en segundo plano.

```
# Presiona Ctrl+Z para suspender el trabajo en primer plano
# Luego, reanúdalo en segundo plano
bg %1
```

5.  Mostrar los trabajos de nuevo

```
jobs
[1]   Running                 sleep 300 &
[2]-  Running                 sleep 400 &
[3]+  Running                 sleep 500 &
```

En este ejercicio, tú:

-   Iniciaste tres procesos en segundo plano usando comandos sleep.
    
-   Usaste `jobs` para mostrar la lista de trabajos en segundo plano.
    
-   Trajiste un trabajo al primer plano con `fg %número_del_trabajo`.
    
-   Suspendiste el trabajo con `Ctrl+Z` y lo moviste nuevamente al segundo plano con `bg %número_del_trabajo`.
    
-   Usaste `jobs` nuevamente para verificar el estado de los trabajos en segundo plano.
    

Ahora sabes cómo controlar los trabajos.

#### Matar procesos

Es posible terminar un proceso no respondiente o no deseado usando el comando `kill`. El comando `kill` envía una señal a un ID de proceso, solicitándole que termine.

Hay varias opciones disponibles con el comando `kill`.

```
# Opciones disponibles con kill

kill -l
 1) SIGHUP     2) SIGINT     3) SIGQUIT     4) SIGILL     5) SIGTRAP
 6) SIGABRT     7) SIGBUS     8) SIGFPE     9) SIGKILL    10) SIGUSR1
11) SIGSEGV    12) SIGUSR2    13) SIGPIPE    14) SIGALRM    15) SIGTERM
16) SIGSTKFLT    17) SIGCHLD    18) SIGCONT    19) SIGSTOP    20) SIGTSTP
21) SIGTTIN    22) SIGTTOU    23) SIGURG    24) 
...terminado
```

Aquí hay algunos ejemplos del comando `kill` en Linux:

1.  **Matar un proceso por PID (ID de Proceso):**
    
    ```
     kill 1234
    ```
    
    Este comando envía la señal `SIGTERM` por defecto al proceso con PID 1234, solicitándole que termine.
    
2.  **Matar un proceso por nombre:**
    
    ```
     pkill nombre_del_proceso
    ```
    
    Este comando envía la señal `SIGTERM` por defecto a todos los procesos con el nombre especificado.
    
3.  **Forzar la terminación de un proceso:**
    
    ```
     kill -9 1234
    ```
    
    Este comando envía la señal `SIGKILL` al proceso con PID 1234, terminándolo de manera forzosa.
    
4.  **Enviar una señal específica a un proceso:**
    
    ```
     kill -s SIGSTOP 1234
    ```
    
    Este comando envía la señal `SIGSTOP` al proceso con PID 1234, deteniéndolo.
    
5.  **Matar todos los procesos propiedad de un usuario específico:**
    
    ```
     pkill -u nombre_de_usuario
    ```
    
    Este comando envía la señal `SIGTERM` por defecto a todos los procesos propiedad del usuario especificado.
    

Estos ejemplos demuestran varias formas de usar el comando `kill` para gestionar procesos en un entorno Linux.

Aquí está la información sobre las opciones y señales del comando `kill` en forma de tabla: Esta tabla resume las opciones y señales más comunes del comando `kill` utilizadas en Linux para gestionar procesos.

| Comando / Opción | Señal | Descripción |
| --- | --- | --- |
| `kill <pid>` | `SIGTERM` | Solicita que el proceso termine de forma ordenada (señal por defecto). |
| `kill -9 <pid>` | `SIGKILL` | Fuerza la terminación inmediata del proceso sin limpieza. |
| `kill -SIGKILL <pid>` | `SIGKILL` | Fuerza la terminación inmediata del proceso sin limpieza. |
| `kill -15 <pid>` | `SIGTERM` | Envía explícitamente la señal `SIGTERM` solicitando una terminación ordenada. |
| `kill -SIGTERM <pid>` | `SIGTERM` | Envía explícitamente la señal `SIGTERM` solicitando una terminación ordenada. |
| `kill -1 <pid>` | `SIGHUP` | Tradicionalmente significa "colgar"; se puede usar para recargar archivos de configuración. |
| `kill -SIGHUP <pid>` | `SIGHUP` | Tradicionalmente significa "colgar"; se puede usar para recargar archivos de configuración. |
| `kill -2 <pid>` | `SIGINT` | Solicita que el proceso termine (igual que presionar `Ctrl+C` en la terminal). |
| `kill -SIGINT <pid>` | `SIGINT` | Solicita que el proceso termine (igual que presionar `Ctrl+C` en la terminal). |
| `kill -3 <pid>` | `SIGQUIT` | Causa que el proceso termine y genere un volcado de memoria para depuración. |
| `kill -SIGQUIT <pid>` | `SIGQUIT` | Causa que el proceso termine y genere un volcado de memoria para depuración. |
| `kill -19 <pid>` | `SIGSTOP` | Pausa el proceso. |
| `kill -SIGSTOP <pid>` | `SIGSTOP` | Pausa el proceso. |
| `kill -18 <pid>` | `SIGCONT` | Reanuda un proceso pausado. |
| `kill -SIGCONT <pid>` | `SIGCONT` | Reanuda un proceso pausado. |
| `killall <nombre>` | Varía | Envía una señal a todos los procesos con el nombre dado. |
| `killall -9 <nombre>` | `SIGKILL` | Fuerza la terminación de todos los procesos con el nombre dado. |
| `pkill <patrón>` | Varía | Envía una señal a los procesos basados en una coincidencia de patrón. |
| `pkill -9 <patrón>` | `SIGKILL` | Fuerza la terminación de todos los procesos que coinciden con el patrón. |
| `xkill` | `SIGKILL` | Utilidad gráfica que permite hacer clic en una ventana para matar el proceso correspondiente. |

Leer una entrada y escribir una salida es una parte esencial para entender la línea de comandos y la creación de scripts en shell. En Linux, cada proceso tiene tres flujos predeterminados:

1.  Entrada Estándar (`stdin`): Este flujo se utiliza para la entrada, típicamente desde el teclado. Cuando un programa lee de `stdin`, recibe datos ingresados por el usuario o redirigidos desde un archivo. Un descriptor de archivo es un identificador único que el sistema operativo asigna a un archivo abierto para realizar un seguimiento de los archivos abiertos.
    
    El descriptor de archivo para `stdin` es `0`.
    
2.  Salida Estándar (`stdout`): Este es el flujo de salida predeterminado donde un proceso escribe su salida. Por defecto, la salida estándar es la terminal. La salida también puede redirigirse a un archivo u otro programa. El descriptor de archivo para `stdout` es `1`.
    
3.  Error Estándar (`stderr`): Este es el flujo de error predeterminado donde un proceso escribe sus mensajes de error. Por defecto, el error estándar es la terminal, lo que permite ver los mensajes de error incluso si `stdout` está redirigido. El descriptor de archivo para `stderr` es `2`.
    

#### Redirección y Tuberías

**Redirección:** Puedes redirigir los flujos de error y salida a archivos u otros comandos. Por ejemplo:

```
# Redirigiendo stdout a un archivo
ls > output.txt

# Redirigiendo stderr a un archivo
ls non_existent_directory 2> error.txt

# Redirigiendo tanto stdout como stderr a un archivo
ls non_existent_directory > all_output.txt 2>&1
```

En el último comando,

-   `ls non_existent_directory`: lista el contenido de un directorio llamado non\_existent\_directory. Dado que este directorio no existe, `ls` generará un mensaje de error.
    
-   `> all_output.txt`: El operador `>` redirige la salida estándar (`stdout`) del comando `ls` al archivo `all_output.txt`. Si el archivo no existe, se creará. Si ya existe, su contenido se sobrescribirá.
    
-   `2>&1:`: Aquí, `2` representa el descriptor de archivo para el error estándar (`stderr`). `&1` representa el descriptor de archivo para la salida estándar (`stdout`). El carácter `&` se usa para especificar que `1` no es el nombre del archivo, sino un descriptor de archivo.
    

Así que, `2>&1` significa "redirigir stderr (2) a donde stdout (1) se esté redirigiendo", que en este caso es el archivo `all_output.txt`. Por lo tanto, tanto la salida (si la hubiera) como el mensaje de error de `ls` se escribirán en `all_output.txt`.

**Tuberías:**

Puedes usar tuberías (`|`) para pasar la salida de un comando como entrada a otro:

```
ls | grep image
# Salida
image-10.png
image-11.png
image-12.png
image-13.png
... Salida truncada ...
```

### 8.6 Automatización en Linux – Automatizar Tareas con Trabajos Cron

Cron es una poderosa utilidad para la programación de trabajos que está disponible en sistemas operativos similares a UNIX. Configurando cron, puedes establecer trabajos automatizados para que se ejecuten a diario, semanalmente, mensualmente o en otros tiempos específicos. Las capacidades de automatización proporcionadas por cron juegan un papel crucial en la administración de sistemas Linux.

El daemon `crond` (un tipo de programa informático que se ejecuta en segundo plano) habilita la funcionalidad de cron. Cron lee las **crontab** (tablas cron) para ejecutar scripts predefinidos.

Usando una sintaxis específica, puedes configurar un trabajo cron para programar scripts u otros comandos para que se ejecuten automáticamente.

**¿Qué son los trabajos cron en Linux?**

Cualquier tarea que programes a través de cron se llama trabajo cron.

Ahora, veamos cómo funcionan los trabajos cron.

#### Cómo controlar el acceso a crons

Para utilizar trabajos cron, un administrador necesita permitir que se agreguen trabajos cron para los usuarios en el archivo `/etc/cron.allow`.

Si obtienes un mensaje como este, significa que no tienes permiso para usar cron.

![Adición de trabajo cron denegada para el usuario John.](https://www.freecodecamp.org/news/content/images/2021/11/image-51.png)

Para permitir que John use cron, incluye su nombre en `/etc/cron.allow`. Crea el archivo si no existe. Esto permitirá a John crear y editar trabajos cron.

![Permitiendo a John en el archivo cron.allow](https://www.freecodecamp.org/news/content/images/2021/11/image-52.png)

A los usuarios también se les puede denegar el acceso a trabajos cron ingresando sus nombres de usuario en el archivo `/etc/cron.d/cron.deny`.

#### Cómo agregar trabajos cron en Linux

Primero, para usar trabajos cron, necesitarás verificar el estado del servicio cron. Si cron no está instalado, puedes descargarlo fácilmente a través del gestor de paquetes. Solo usa esto para verificar:

```
# Verificar el servicio cron en el sistema Linux
sudo systemctl status cron.service
```

#### Sintaxis del trabajo cron

Las crontabs utilizan las siguientes banderas para agregar y listar trabajos cron:

-   `crontab -e`: edita las entradas de crontab para agregar, eliminar o editar trabajos cron.
    
-   `crontab -l`: lista todos los trabajos cron para el usuario actual.
    
-   `crontab -u nombre_de_usuario -l`: lista los crons de otro usuario.
    
-   `crontab -u nombre_de_usuario -e`: edita los crons de otro usuario.
    

Cuando listas crons y existen, verás algo como esto:

```
# Ejemplo de trabajo cron
* * * * * sh /ruta/al/script.sh
```

En el ejemplo anterior,

-   `*` representa minuto(s), hora(s), día(s), mes(es), día(s) de la semana, respectivamente. Consulta los detalles de estos valores a continuación:

|  | **VALOR** | **DESCRIPCIÓN** |
| --- | --- | --- |
| Minutos | 0-59 | El comando se ejecutará en el minuto específico. |
| Horas | 0-23 | El comando se ejecutará en la hora específica. |
| Días | 1-31 | Los comandos se ejecutarán en estos días del mes. |
| Meses | 1-12 | El mes en el que se deben ejecutar las tareas. |
| Días de la semana | 0-6 | Días de la semana donde se ejecutarán los comandos. Aquí, 0 es domingo. |

A continuación se muestra una descripción de la sintaxis de las tareas programadas con cron:

```
*   *   *   *   *  sh /path/to/script/script.sh
|   |   |   |   |              |
|   |   |   |   |      Comando o Script a Ejecutar      
|   |   |   |   |
|   |   |   |   |
|   |   |   |   |
|   |   |   | Día de la Semana(0-6)
|   |   |   |
|   |   | Mes del Año(1-12)
|   |   |
|   | Día del Mes(1-31)  
|   |
| Hora(0-23)  
|
Minuto(0-59)
```

#### Ejemplos de tareas programadas con cron

A continuación se muestran algunos ejemplos de programación de tareas con cron.

| **HORARIO** | **VALOR PROGRAMADO** |
| --- | --- |
| `5 0 * 8 *` | A las 00:05 en agosto. |
| `5 4 * * 6` | A las 04:05 el sábado. |
| `0 22 * * 1-5` | A las 22:00 todos los días de la semana de lunes a viernes. |

Está bien si no logras entender todo esto de una vez. Puedes practicar y generar horarios de cron con el sitio web [crontab guru][54].

#### Cómo configurar una tarea cron

En esta sección, veremos un ejemplo de cómo programar un script simple con una tarea cron.

1.  Crea un script llamado `date-script.sh` que imprima la fecha y hora del sistema y la agregue a un archivo. El script se muestra a continuación:

```
#!/bin/bash

echo `date` >> date-out.txt
```

2. Haz que el script sea ejecutable otorgándole derechos de ejecución.

```
chmod 775 date-script.sh
```

3. Añade el script en el crontab usando `crontab -e`.

Aquí, lo hemos programado para que se ejecute cada minuto.

```
*/1 * * * * /bin/sh /root/date-script.sh
```

4. Verifica la salida del archivo `date-out.txt`. Según el script, la fecha del sistema debería imprimirse en este archivo cada minuto.

```
cat date-out.txt
# resultado
Mié 26 Jun 16:59:33 PKT 2024
Mié 26 Jun 17:00:01 PKT 2024
Mié 26 Jun 17:01:01 PKT 2024
Mié 26 Jun 17:02:01 PKT 2024
Mié 26 Jun 17:03:01 PKT 2024
Mié 26 Jun 17:04:01 PKT 2024
Mié 26 Jun 17:05:01 PKT 2024
Mié 26 Jun 17:06:01 PKT 2024
Mié 26 Jun 17:07:01 PKT 2024
```

**Cómo solucionar problemas de cron**

Las tareas cron son muy útiles, pero no siempre funcionan como se espera. Afortunadamente, hay algunos métodos efectivos que puedes usar para solucionarlas.

**1. Verificar el horario.**

Primero, puedes intentar verificar el horario que se ha establecido para la tarea cron. Puedes hacerlo con la sintaxis que viste en las secciones anteriores.

**2. Verificar los registros de cron.**

Primero, necesitas verificar si la tarea cron se ha ejecutado en el momento previsto o no. En Ubuntu, puedes comprobar esto en los registros de cron ubicados en `/var/log/syslog`.

Si hay una entrada en estos registros en el momento correcto, significa que la tarea cron se ha ejecutado según el horario que configuraste.

A continuación se muestran los registros de nuestro ejemplo de tarea cron. Ten en cuenta la primera columna que muestra la marca de tiempo. La ruta del script también se menciona al final de la línea. Las líneas #1, 3 y 5 muestran que el script se ejecutó según lo previsto.

```
1 Jun 26 17:02:01 zaira-ThinkPad CRON[27834]: (zaira) CMD (/bin/sh /home/zaira/date-script.sh)
2 Jun 26 17:02:02 zaira-ThinkPad systemd[2094]: Iniciado el extractor de metadatos de Tracker.
3 Jun 26 17:03:01 zaira-ThinkPad CRON[28255]: (zaira) CMD (/bin/sh /home/zaira/date-script.sh)
4 Jun 26 17:03:02 zaira-ThinkPad systemd[2094]: Iniciado el extractor de metadatos de Tracker.
5 Jun 26 17:04:01 zaira-ThinkPad CRON[28538]: (zaira) CMD (/bin/sh /home/zaira/date-script.sh)
```

**3. Redirigir la salida de cron a un archivo.**

Puedes redirigir la salida de una tarea cron a un archivo y verificar el archivo para detectar posibles errores.

```
# Redirigir la salida de cron a un archivo
* * * * * sh /path/to/script.sh &> log_file.log
```

### 8.7. Fundamentos de Redes en Linux

Linux ofrece una serie de comandos para ver información relacionada con la red. En esta sección discutiremos brevemente algunos de los comandos.

#### Ver interfaces de red con `ifconfig`

El comando `ifconfig` proporciona información sobre las interfaces de red. Aquí hay un ejemplo de salida:

```
ifconfig

# Salida
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.1.100  mascara 255.255.255.0  difusión 192.168.1.255
        inet6 fe80::a00:27ff:fe4e:66a1  longitud de prefijo 64  id_de_ámbito 0x20<enlace>
        ether 08:00:27:4e:66:a1  longitud de cola 1000  (Ethernet)
        RX paquetes 1024  bytes 654321 (654.3 KB)
        RX errores 0  descartados 0  sobrepasados 0  marco 0
        TX paquetes 512  bytes 123456 (123.4 KB)
        TX errores 0  descartados 0 sobrepasados 0  portadora 0  colisiones 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  mascara 255.0.0.0
        inet6 ::1  longitud de prefijo 128  id_de_ámbito 0x10<host>
        bucle  longitud de cola 1000  (Bucle Local)
        RX paquetes 256  bytes 20480 (20.4 KB)
        RX errores 0  descartados 0  sobrepasados 0  marco 0
        TX paquetes 256  bytes 20480 (20.4 KB)
        TX errores 0  descartados 0  sobrepasados 0  portadora 0  colisiones 0
```

La salida del comando `ifconfig` muestra las interfaces de red configuradas en el sistema, junto con detalles como direcciones IP, direcciones MAC, estadísticas de paquetes y más.

Estas interfaces pueden ser dispositivos físicos o virtuales.

Para extraer direcciones IPv4 e IPv6, puedes usar `ip -4 addr` y `ip -6 addr`, respectivamente.

**Ver actividad de red con**`netstat`

El comando `netstat` muestra la actividad y estadísticas de la red proporcionando la siguiente información:

Aquí hay algunos ejemplos de uso del comando `netstat` en la línea de comandos:

#### Comprobar la conectividad de red entre dos dispositivos usando `ping`

`ping` se usa para probar la conectividad de red entre dos dispositivos. Envía paquetes ICMP al dispositivo objetivo y espera una respuesta.

```
ping google.com
```

`ping` prueba si recibes una respuesta sin obtener un tiempo de espera.

```
ping google.com
PING google.com (142.250.181.46) 56(84) bytes of data.
64 bytes from fjr04s06-in-f14.1e100.net (142.250.181.46): icmp_seq=1 ttl=60 time=78.3 ms
64 bytes from fjr04s06-in-f14.1e100.net (142.250.181.46): icmp_seq=2 ttl=60 time=141 ms
64 bytes from fjr04s06-in-f14.1e100.net (142.250.181.46): icmp_seq=3 ttl=60 time=205 ms
64 bytes from fjr04s06-in-f14.1e100.net (142.250.181.46): icmp_seq=4 ttl=60 time=100 ms
^C
--- google.com ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3001ms
rtt min/avg/max/mdev = 78.308/131.053/204.783/48.152 ms
```

Puedes detener la respuesta con `Ctrl + C`.

#### Probando puntos de conexión con el comando `curl`

El comando `curl` significa "client URL" (URL del cliente). Se usa para transferir datos hacia o desde un servidor. También se puede usar para probar puntos de conexión de API que ayudan en la resolución de problemas de sistemas y aplicaciones.

Como ejemplo, puedes usar [`http://www.official-joke-api.appspot.com/`][55] para experimentar con el comando `curl`.

-   El comando `curl` sin ninguna opción usa el método GET de forma predeterminada.

```
curl http://www.official-joke-api.appspot.com/random_joke
{"type":"general",
"setup":"What did the fish say when it hit the wall?","punchline":"Dam.","id":1}
```

-   `curl -o` guarda la salida en el archivo mencionado.

```
curl -o random_joke.json http://www.official-joke-api.appspot.com/random_joke
# guarda la salida en random_joke.json
```

-   `curl -I` obtiene solo los encabezados.

```
curl -I http://www.official-joke-api.appspot.com/random_joke
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Vary: Accept-Encoding
X-Powered-By: Express
Access-Control-Allow-Origin: *
ETag: W/"71-NaOSpKuq8ChoxdHD24M0lrA+JXA"
X-Cloud-Trace-Context: 2653a86b36b8b131df37716f8b2dd44f
Content-Length: 113
Date: Thu, 06 Jun 2024 10:11:50 GMT
Server: Google Frontend
```

### 8.8. Resolución de Problemas en Linux: Herramientas y Técnicas

#### Informe de actividad del sistema con `sar`

El comando `sar` en Linux es una herramienta poderosa para recopilar, informar y guardar información de la actividad del sistema. Es parte del paquete `sysstat` y se usa ampliamente para monitorear el rendimiento del sistema a lo largo del tiempo.

Para usar `sar`, primero debes instalar `sysstat` usando `sudo apt install sysstat`.

Una vez instalado, inicia el servicio con `sudo systemctl start sysstat`.

Verifica el estado con `sudo systemctl status sysstat`.

Una vez que el estado es activo, el sistema comenzará a recopilar varias estadísticas que puedes usar para acceder y analizar datos históricos. Veremos eso en detalle pronto.

La sintaxis del comando `sar` es la siguiente:

```
sar [opciones] [intervalo] [conteo]
```

Por ejemplo, `sar -u 1 3` mostrará estadísticas de utilización de la CPU cada segundo tres veces.

```
sar -u 1 3
# Salida
Linux 6.5.0-28-generic (zaira-ThinkPad)     04/06/24     _x86_64_    (12 CPU)

19:09:26        CPU     %user     %nice   %system   %iowait    %steal     %idle
19:09:27        all      3.78      0.00      2.18      0.08      0.00     93.96
19:09:28        all      4.02      0.00      2.01      0.08      0.00     93.89
19:09:29        all      6.89      0.00      2.10      0.00      0.00     91.01
Promedio:        all      4.89      0.00      2.10      0.06      0.00     92.95
```

Aquí hay algunos casos de uso comunes y ejemplos de cómo usar el comando `sar`.

`sar` se puede usar para una variedad de propósitos:

##### 1\. Uso de memoria

Para verificar el uso de la memoria (libre y usada), usa:

```
sar -r 1 3

Linux 6.5.0-28-generic (zaira-ThinkPad)     04/06/24     _x86_64_    (12 CPU)

19:10:46    kbmemfree   kbavail kbmemused  %memused kbbuffers  kbcached  kbcommit   %commit  kbactive   kbinact   kbdirty
19:10:47      4600104   8934352   5502124     36.32    375844   4158352  15532012     65.99   6830564   2481260       264
19:10:48      4644668   8978940   5450252     35.98    375852   4165648  15549184     66.06   6776388   2481284        36
19:10:49      4646548   8980860   5448328     35.97    375860   4165648  15549224     66.06   6774368   2481292       116
Promedio:      4630440   8964717   5466901     36.09    375852   4163216  15543473     66.04   6793773   2481279       139
```

Este comando muestra estadísticas de memoria cada segundo tres veces.

##### 2\. Utilización del espacio de intercambio

Para ver las estadísticas de utilización del espacio de intercambio, usa:

```
sar -S 1 3

sar -S 1 3
Linux 6.5.0-28-generic (zaira-ThinkPad)     04/06/24     _x86_64_    (12 CPU)

19:11:20    kbswpfree kbswpused  %swpused  kbswpcad   %swpcad
19:11:21      8388604         0      0.00         0      0.00
19:11:22      8388604         0      0.00         0      0.00
19:11:23      8388604         0      0.00         0      0.00
Promedio:      8388604         0      0.00         0      0.00
```

Este comando ayuda a monitorear el uso de intercambio, lo cual es crucial para sistemas que se quedan sin memoria física.

##### 3\. Carga de dispositivos de E/S

```markdown
sar -d 1 3
```

Este comando proporciona estadísticas detalladas sobre las transferencias de datos hacia y desde dispositivos de bloque, y es útil para diagnosticar cuellos de botella de E/S.

##### 5\. Estadísticas de red

Para ver estadísticas de red, como el número de paquetes recibidos (transmitidos) por la interfaz de red:

```
sar -n DEV 1 3
# -n DEV indica a sar que reporte interfaces de dispositivos de red
sar -n DEV 1 3
Linux 6.5.0-28-generic (zaira-ThinkPad)     04/06/24     _x86_64_    (12 CPU)

19:12:47        IFACE   rxpck/s   txpck/s    rxkB/s    txkB/s   rxcmp/s   txcmp/s  rxmcst/s   %ifutil
19:12:48           lo      0.00      0.00      0.00      0.00      0.00      0.00      0.00      0.00
19:12:48       enp2s0      0.00      0.00      0.00      0.00      0.00      0.00      0.00      0.00
19:12:48       wlp3s0     10.00      3.00      1.83      0.37      0.00      0.00      0.00      0.00
19:12:48    br-5129d04f972f      0.00      0.00      0.00      0.00      0.00      0.00      0.00      0.00
.
.
.

Average:        IFACE   rxpck/s   txpck/s    rxkB/s    txkB/s   rxcmp/s   txcmp/s  rxmcst/s   %ifutil
Average:           lo      0.00      0.00      0.00      0.00      0.00      0.00      0.00      0.00
Average:       enp2s0      0.00      0.00      0.00      0.00      0.00      0.00      0.00      0.00
...salida truncada...
```

Esto muestra estadísticas de red cada segundo durante tres segundos, ayudando a monitorear el tráfico de red.

##### 6\. Datos históricos

Recuerde que previamente instalamos el paquete `sysstat` y ejecutamos el servicio. Siga los pasos a continuación para habilitar y acceder a los datos históricos.

1.  **Habilitar la recolección de datos:** Edite el archivo de configuración de `sysstat` para habilitar la recolección de datos.
    
    ```
     sudo nano /etc/default/sysstat
    ```
    
    Cambie `ENABLED="false"` a `ENABLED="true"`.
    
    ```
     vim /etc/default/sysstat
     #
     # Configuraciones por defecto para /etc/init.d/sysstat, /etc/cron.d/sysstat
     # y archivos /etc/cron.daily/sysstat
     #
    
     # ¿Debe sadc recolectar información de actividad del sistema? Los valores válidos
     # son "true" y "false". Por favor, no ponga otros valores, serán
     # sobrescritos por debconf.
     ENABLED="true"
    ```
    
2.  **Configurar el intervalo de recolección de datos:** Edite la configuración del trabajo cron para establecer el intervalo de recolección de datos.
    
    ```
     sudo nano /etc/cron.d/sysstat
    ```
    
    Por defecto, recolecta datos cada 10 minutos. Puede ajustar el intervalo modificando el horario del trabajo cron. Los archivos relevantes irán a la carpeta `/var/log/sysstat`.
    
3.  **Ver datos históricos:** Use el comando `sar` para ver datos históricos. Por ejemplo, para ver el uso de la CPU para el día actual:
    
    ```
     sar -u
    ```
    
    Para ver datos de una fecha específica:
    
    ```
     sar -u -f /var/log/sysstat/sa<DD>
    ```
    
    Reemplace `<DD>` con el día del mes para el cual quiere ver los datos.
    
    En el siguiente comando, `/var/log/sysstat/sa04` da estadísticas para el cuarto día del mes actual.
    

```
sar -u -f /var/log/sysstat/sa04
Linux 6.5.0-28-generic (zaira-ThinkPad)     04/06/24     _x86_64_    (12 CPU)

15:20:49     LINUX RESTART    (12 CPU)

16:13:30     LINUX RESTART    (12 CPU)

18:16:00        CPU     %user     %nice   %system   %iowait    %steal     %idle
18:16:01        all      0.25      0.00      0.67      0.08      0.00     99.00
Average:        all      0.25      0.00      0.67      0.08      0.00     99.00
```

##### 7\. Interrupciones de CPU en tiempo real

Para observar interrupciones en tiempo real por segundo atendidas por la CPU, use este comando:

```
sar -I SUM 1 3

# Salida
Linux 6.5.0-28-generic (zaira-ThinkPad)     04/06/24     _x86_64_    (12 CPU)

19:14:22         INTR    intr/s
19:14:23          sum   5784.00
19:14:24          sum   5694.00
19:14:25          sum   5795.00
Average:          sum   5757.67
```

Este comando ayuda a monitorear con qué frecuencia la CPU está manejando interrupciones, lo cual puede ser crucial para el ajuste de rendimiento en tiempo real.

Estos ejemplos ilustran cómo puede usar `sar` para monitorear varios aspectos del desempeño del sistema. El uso regular de `sar` puede ayudar a identificar cuellos de botella del sistema y asegurar que las aplicaciones sigan funcionando de manera eficiente.

### 8.9. Estrategia general de solución de problemas para servidores

**¿Por qué necesitamos entender el monitoreo?**

El monitoreo del sistema es un aspecto importante de la administración del sistema. Las aplicaciones críticas exigen un alto nivel de proactividad para prevenir fallos y reducir el impacto de las interrupciones.

Linux ofrece herramientas muy poderosas para evaluar la salud del sistema. En esta sección, aprenderá sobre los varios métodos disponibles para verificar la salud de su sistema e identificar los cuellos de botella.

#### Encontrar el promedio de carga y el tiempo de actividad del sistema

Pueden ocurrir reinicios del sistema que a veces pueden desordenar algunas configuraciones. Para revisar cuánto tiempo ha estado encendida la máquina, use el comando: `uptime`. Además del tiempo de actividad, el comando también muestra el promedio de carga.

```
[user@host ~]$ uptime 19:15:00 up 1:04, 0 users, load average: 2.92, 4.48, 5.20
```

El promedio de carga es la carga del sistema durante los últimos 1, 5 y 15 minutos. Una mirada rápida indica si la carga del sistema parece estar aumentando o disminuyendo con el tiempo.
```


La carga por CPU se puede calcular dividiendo el promedio de carga por el número total de CPUs disponibles.

Para encontrar el número de CPUs, utiliza el comando `lscpu`.

```
lscpu
# salida
Architecture:            x86_64
  CPU op-mode(s):        32-bit, 64-bit
  Address sizes:         48 bits physical, 48 bits virtual
  Byte Order:            Little Endian
CPU(s):                  12
  On-line CPU(s) list:   0-11
.
.
.
salida omitida
```

Si el promedio de carga parece aumentar y no disminuye, las CPUs están sobrecargadas. Hay algún proceso que está atascado o hay una fuga de memoria.

#### Calculando la memoria libre

A veces, una alta utilización de memoria puede estar causando problemas. Para comprobar la memoria disponible y la memoria en uso, utiliza el comando `free`.

```
free -mh
# salida
               total        used        free      shared  buff/cache   available
Mem:            14Gi       3.5Gi       7.7Gi       109Mi       3.2Gi        10Gi
Swap:          8.0Gi          0B       8.0Gi
```

#### Calculando el espacio en disco

Para asegurarse de que el sistema esté sano, no olvides el espacio en disco. Para listar todos los puntos de montaje disponibles y su respectivo porcentaje de uso, utiliza el siguiente comando. Idealmente, los espacios de disco utilizados no deberían exceder el 80%.

El comando `df` proporciona espacios de disco detallados.

```
df -h
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           1.5G  2.4M  1.5G   1% /run
/dev/nvme0n1p2  103G   34G   65G  35% /
tmpfs           7.3G   42M  7.2G   1% /dev/shm
tmpfs           5.0M  4.0K  5.0M   1% /run/lock
efivarfs        246K   93K  149K  39% /sys/firmware/efi/efivars
/dev/nvme0n1p3  130G   47G   77G  39% /home
/dev/nvme0n1p1  511M  6.1M  505M   2% /boot/efi
tmpfs           1.5G  140K  1.5G   1% /run/user/1000
```

#### Determinando los estados de los procesos

Los estados de los procesos se pueden monitorear para ver cualquier proceso atascado con un alto uso de memoria o CPU.

Vimos anteriormente que el comando `ps` brinda información útil sobre un proceso. Observa las columnas `CPU` y `MEM`.

```
[user@host ~]$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
 runner         1  0.1  0.0 1535464 15576 ?       S  19:18   0:00 /inject/init
 runner        14  0.0  0.0  21484  3836 pts/0    S   19:21   0:00 bash --norc
 runner        22  0.0  0.0  37380  3176 pts/0    R+   19:23   0:00 ps aux
```

#### Monitoreo en tiempo real del sistema

El monitoreo en tiempo real ofrece una ventana al estado del sistema en tiempo real.

Una utilidad que puedes usar para esto es el comando `top`.

El comando top muestra una vista dinámica de los procesos del sistema, mostrando un encabezado de resumen seguido de una lista de procesos o hilos. A diferencia de su contraparte estática `ps`, `top` actualiza continuamente las estadísticas del sistema.

Con `top`, puedes ver detalles bien organizados en una ventana compacta. Hay una serie de banderas, atajos y métodos de resaltado que vienen con `top`.

También puedes matar procesos usando `top`. Para eso, presiona `k` y luego ingresa el ID del proceso.

#### Interpretación de registros

Los registros del sistema y de aplicaciones llevan mucha información sobre lo que está sucediendo en el sistema. Contienen información útil y códigos de error que apuntan a fallos. Si buscas códigos de error en los registros, el tiempo de identificación y rectificación de problemas puede reducirse significativamente.

#### Análisis de puertos de red

El aspecto de la red no debe ser ignorado ya que los problemas de red son comunes y pueden impactar el sistema y los flujos de tráfico. Los problemas de red comunes incluyen agotamiento de puertos, estrangulamiento de puertos, recursos no liberados, etc.

Para identificar tales problemas, necesitamos entender los estados de los puertos.

Algunos de los estados de los puertos se explican brevemente aquí:

| **Estado** | **Descripción** |
| --- | --- |
| LISTEN | Representa puertos que están esperando una solicitud de conexión de cualquier TCP y puerto remoto. |
| ESTABLISHED | Representa conexiones que están abiertas y los datos recibidos pueden ser entregados al destino. |
| TIME WAIT | Representa el tiempo de espera para asegurar el reconocimiento de su solicitud de terminación de conexión. |
| FIN WAIT2 | Representa la espera de una solicitud de terminación de conexión del TCP remoto. |

Exploremos cómo podemos analizar la información relacionada con los puertos en Linux.

**Rangos de puertos:** Los rangos de puertos están definidos en el sistema, y el rango puede aumentarse o disminuirse en consecuencia. En el siguiente fragmento, el rango es de `15000` a `65000`, lo que hace un total de `50000` (65000 - 15000) puertos disponibles. Si los puertos utilizados están alcanzando o superando este límite, entonces hay un problema.

```
[user@host ~]$ /sbin/sysctl net.ipv4.ip_local_port_range
net.ipv4.ip_local_port_range = 15000    65000
```

El error reportado en los registros en tales casos puede ser `Failed to bind to port` o `Too many connections`.

#### Identificando pérdida de paquetes

En el monitoreo del sistema, necesitamos asegurar que la comunicación saliente y entrante esté intacta.

Un comando útil es `ping`. `ping` golpea el sistema de destino y trae la respuesta de vuelta. Observa las últimas líneas de estadísticas que muestran el porcentaje de pérdida de paquetes y el tiempo.

```
# ping IP de destino
[user@host ~]$ ping 10.13.6.113
 PING 10.13.6.141 (10.13.6.141) 56(84) bytes of data.
 64 bytes from 10.13.6.113: icmp_seq=1 ttl=128 time=0.652 ms
 64 bytes from 10.13.6.113: icmp_seq=2 ttl=128 time=0.593 ms
 64 bytes from 10.13.6.113: icmp_seq=3 ttl=128 time=0.478 ms
 64 bytes from 10.13.6.113: icmp_seq=4 ttl=128 time=0.384 ms
 64 bytes from 10.13.6.113: icmp_seq=5 ttl=128 time=0.432 ms
 64 bytes from 10.13.6.113: icmp_seq=6 ttl=128 time=0.747 ms
 64 bytes from 10.13.6.113: icmp_seq=7 ttl=128 time=0.379 ms
 ^C
 --- 10.13.6.113 ping statistics ---
 7 paquetes transmitidos, 7 recibidos,0% pérdida de paquetes, tiempo 6001ms
 rtt min/avg/max/mdev = 0.379/0.523/0.747/0.134 ms
```

#### Recolectando estadísticas para la investigación de problemas

Siempre es una buena práctica recolectar ciertas estadísticas que serían útiles para identificar la causa raíz más tarde. Usualmente, después del reinicio del sistema o del reinicio de servicios, perdemos la instantánea anterior del sistema y los registros.

A continuación se presentan algunos de los métodos para capturar una instantánea del sistema.

-   **Copia de seguridad de registros**

Antes de hacer cualquier cambio, copia los archivos de registro a otra ubicación. Esto es crucial para entender en qué estado se encontraba el sistema durante el momento del problema. A veces, los archivos de registro son la única ventana para mirar los estados anteriores del sistema ya que otras estadísticas de tiempo de ejecución se pierden.

-   **Captura de TCP**

Tcpdump es una utilidad de línea de comandos que te permite capturar y analizar el tráfico de red entrante y saliente. Se usa principalmente para ayudar a solucionar problemas de red. Si sientes que el tráfico del sistema se está viendo afectado, toma `tcpdump` de la siguiente manera:

```
sudo tcpdump -i any -w

# Donde,
# -i any captura tráfico de todas las interfaces
# -w especifica el nombre del archivo de salida

# Detén el comando después de unos minutos ya que el tamaño del archivo puede aumentar
# usa la extensión de archivo .pcap
```

Una vez capturado `tcpdump`, puedes usar herramientas como Wireshark para analizar visualmente el tráfico.

### Conclusión

Gracias por leer el libro hasta el final. Si lo encontraste útil, considera compartirlo con otros.

Sin embargo, este libro no termina aquí. Continuaré mejorándolo y agregando nuevos materiales en el futuro. Si encontraste algún problema o si deseas sugerir mejoras, [siéntete libre de abrir un PR/Issue.][56]

**¡Mantente Conectado y Continúa tu Viaje de Aprendizaje!**

Tu viaje con Linux no tiene que terminar aquí. Mantente conectado y lleva tus habilidades al siguiente nivel:

1.  **Sígueme en redes sociales**:
    
    -   [X][57]: Comparto contenido útil en formato corto allí. Mis DMs siempre están abiertos.
        
    -   [LinkedIn][58]: Comparto artículos y publicaciones sobre tecnología allí. Deja una recomendación en LinkedIn y respalda mis habilidades relevantes.
        
2.  **Accede a contenido exclusivo**: Para ayuda personalizada y contenido exclusivo ve [aquí][59].
    

Mis [artículos][60] y libros, como este, son parte de mi misión de aumentar la accesibilidad a contenido de calidad para todos. Este libro también estará disponible para ser traducido a otros idiomas. Cada pieza toma mucho tiempo y esfuerzo escribirla. Este libro será gratuito, para siempre. Si has disfrutado de mi trabajo y quieres mantenerme motivado, considera [invitarme un café][61].

¡Gracias una vez más y feliz aprendizaje!

[1]: #heading-part-1-introduction-to-linux
[2]: #heading-11-getting-started-with-linux
[3]: #heading-part-2-introduction-to-bash-shell-and-system-commands
[4]: #heading-21-getting-started-with-the-bash-shell
[5]: #heading-22-command-structure
[6]: #heading-23-bash-commands-and-keyboard-shortcuts
[7]: #heading-24-identifying-yourself-the-whoami-command
[8]: #heading-part-3-understanding-your-linux-system
[9]: #heading-31-discovering-your-os-and-specs
[10]: #heading-part-4-managing-files-from-the-command-line
[11]: #heading-41-the-linux-file-system-hierarchy
[12]: #heading-42-navigating-the-linux-file-system
[13]: #heading-43-managing-files-and-directories
[14]: #heading-45-basic-commands-for-viewing-files
[15]: #heading-part-5-the-essentials-of-text-editing-in-linux
[16]: #heading-51-mastering-vim-the-complete-guide
[17]: #heading-52-mastering-nano
[18]: #heading-part-6-bash-scripting
[19]: #heading-61-definition-of-bash-scripting
[20]: #heading-62-advantages-of-bash-scripting
[21]: #heading-63-overview-of-bash-shell-and-command-line-interface
[22]: #heading-64-how-to-create-and-execute-bash-scripts
[23]: #heading-65-bash-scripting-basics
[24]: #heading-part-7-managing-software-packages-in-linux
[25]: #heading-71-packages-and-package-management
[26]: #heading-72-installing-a-package-via-command-line
[27]: #heading-73-installing-a-package-via-an-advanced-graphical-method-synaptic
[28]: #heading-74-installing-downloaded-packages-from-a-website
[29]: #heading-part-8-advanced-linux-topics
[30]: #heading-81-user-management
[31]: #heading-82-connecting-to-remote-servers-via-ssh
[32]: #heading-83-advanced-log-parsing-and-analysis
[33]: #heading-84-managing-linux-processes-via-command-line
[34]: #heading-85-standard-input-and-output-streams-in-linux
[35]: #heading-86-automation-in-linux-automate-tasks-with-cron-jobs
[36]: #heading-87-linux-networking-basics
[37]: #heading-88-linux-troubleshooting-tools-and-techniques
[38]: #heading-89-general-troubleshooting-strategy-for-servers
[39]: #heading-conclusion
[40]: https://github.com/torvalds/linux
[41]: https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg
[42]: https://ubuntu.com/
[43]: https://linuxmint.com/
[44]: https://www.archlinux.org/
[45]: https://manjaro.org/
[46]: https://www.kali.org/
[47]: https://ubuntu.com/download/desktop
[48]: https://rufus.ie/
[49]: https://www.virtualbox.org/
[50]: https://multipass.run/
[51]: https://www.vmware.com/content/vmware/vmware-published-sites/us/products/workstation-player.html.html
[52]: https://replit.com/
[53]: https://jslinux.org/
[54]: https://crontab.guru/
[55]: http://www.official-joke-api.appspot.com/
[56]: https://github.com/zairahira/Mastering-Linux-Handbook
[57]: https://twitter.com/hira_zaira
[58]: https://www.linkedin.com/in/zaira-hira/
[59]: https://buymeacoffee.com/zairah/extras
[60]: https://www.freecodecamp.org/news/author/zaira/
[61]: https://buymeacoffee.com/zairah

