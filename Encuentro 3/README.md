# Modelos de Diseño de Sistemas Operativos/ Tarea Encuentro 3

Monolíticos:

Los sistemas operativos monolíticos se caracterizan por implementar en el núcleo los cuatro componentes fundamentales del sistema operativo, que son la planificación de procesos, la administración de la memoria principal, la administración de ficheros y la gestión de los dispositivos de entrada/salida.
Los sistemas operativos de propósito general son predominantemente monolíticos hoy día, algunos ejemplos son:
Sistemas operativos UNIX, tales como FreeBSD, NetBSD y OpenBSD.
Sistemas operativos GNU/Linux, y por tanto, Android también.

Micronúcleo:

Se caracterizan por disponer de un núcleo que implementa únicamente:
	Planificación de procesos
	Mecanismo de comunicación entre procesos
	Gestión de interrupciones
Además, existen procesos servidores que se ejecutan en modo no privilegiado del procesador - que, por supuesto, se ejecutan fuera del espacio del núcleo del sistema operativo - y que implementan los siguientes componentes:
	Administración de memoria principal
	Administración de ficheros
	Gestión de dispositivos de entrada/salida.
Siguiendo este esquema, cuando un proceso cualquiera solicita un servicio a través de una llamada al sistema, el micronúcleo canaliza la petición al proceso servidor correspondiente. Dicha comunicación se realiza mediante mensajería.
La principal ventaja de los sistemas operativos micronúcleo es que, al ejecutar menos líneas de código en modo privilegiado, de manera intuitiva son más fiables. Otras ventajas son que se garantiza el aislamiento de las partes que están fuera del núcleo. Generalmente, si un proceso servidor tiene un bug en su código que hace que entre en una condición de error, se puede relanzar sin tener que reiniciar el sistema por completo.
Híbridos

«Híbrido» implica que el núcleo en cuestión usa conceptos de arquitectura tanto del diseño monolítico como del micronúcleo, específicamente el paso de mensajes y la ejecución de ciertos componentes del sistema operativo en espacio de usuario.
Algunos ejemplos de núcleos híbridos:
	Microsoft Windows NT, usado en todos los sistemas que usan el código base de Windows NT.
	XNU (usado en Mac OS X), es un micronúcleo modificado, debido a la inclusión de código del núcleo de FreeBSD en el núcleo basado en Mach.
	DragonFlyBSD, es el primer sistema BSD que adopta una arquitectura de núcleo híbrido sin basarse en Mach.
	ReactOS.
¿Qué es el Kernel?
El kernel es definido como el núcleo o corazón del sistema operativo, y se encarga principalmente de mediar entre los procesos de usuario y el hardware disponible en la máquina, es decir, concede el acceso al hardware, al software que lo solicite, de una manera segura; y el procesamiento paralelo de varias tareas.
¿Qué es el Shell?
La interfaz con el sistema operativo se denomina shell. El shell es la capa más externa del sistema operativo. Los shells incorporan un lenguaje de programación para controlar procesos y archivos, además de iniciar y controlar otros programas.
¿Qué es SSH?
SSH son las siglas de Secure SHell y es un protocolo de red destinado principalmente a la conexión con máquinas a las que accedemos por línea de comandos
¿Qué es CLI?
Una interfaz de línea de comandos (CLI) es una interfaz de usuario (UI) basada en texto que se utiliza para ver y administrar archivos de computadora
¿Qué es GUI?
La Interfaz gráfica de usuario, conocida también como GUI (Graphical user interface) es el entorno que utiliza un conjunto de imágenes y objetos gráficos para representar información y acciones disponibles en la interfaz mediante las cuales una máquina y el usuario interactúan
¿Qué es API?
API significa “interfaz de programación de aplicaciones”.






