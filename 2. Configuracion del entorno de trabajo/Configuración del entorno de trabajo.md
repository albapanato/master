<style></style>

<style> u{color:#007dc3} h2 {color:#4f6780; font-size:27px}  h3 {color:#9dc5ff; font-size:22px}  h4 {color:#c3b1e1; font-size:18px; font-weight:600} span {color:#46a8f0; font-size:16px} </style>

## Modulo 1. Fundamentos de desarrollo web

### Unidad 2: Configuración del entorno de trabajo.

#### Indice:

- [1. Editor de texto](#editor-de-texto)

  - [1.1 Caracteristicas VS Code](#visual-studio-code)
  - [1.2 Configuraciones VS Code (link-video)](#link-video-cambiar-configuraciones-en-vs-code)

- [2. Terminal](#terminal-ó-cmd)

  - [2.1 Comandos basicos de terminal UNIX (Lynux/MAC)](#comandos-basicos-de-terminal-unix-lynuxmac)
  - [2.2 Comandos basicos de terminal Windows](#comandos-basicos-de-terminal-windows)

- [3. Navegador](#navegador)

<br>

## 1. Editor de texto

El editor de texto es una herramienta crucial para escribir código, con funcionalidades esenciales como el resaltado de sintaxis, el autocompletado, la detección de errores y el soporte para diversos lenguajes de programación. Nosotros trabajaremos con Visual Studio Code.

### 1.1 Visual Studio Code

Características clave que convierten a Visual Studio Code en una opción popular para el desarrollo web son:

- <span> Multiplataforma :</span> Es compatible con Windows, macOS y Linux, lo que permite a los desarrolladores trabajar en diferentes sistemas operativos.

- <span> Ligero, pero potente :</span> Aunque se clasifica como un "editor de código ligero", VSCode ofrece muchas funciones avanzadas, como resaltado de sintaxis, autocompletado, depuración integrada y control de versiones.

- <span> Extensiones :</span> La capacidad de ampliación mediante extensiones es una característica destacada. Los desarrolladores pueden personalizar su entorno agregando extensiones para admitir diferentes lenguajes, herramientas y temas.

- <span> Integración con Git :</span> Tiene una sólida integración con Git, facilitando el seguimiento de cambios en el código y colaboración en proyectos.

- <span> Comunidad activa :</span> Dado que es de código abierto, cuenta con una comunidad activa que contribuye con extensiones y mejoras constantes.

- <span> Soporte para múltiples lenguajes :</span> Aunque inicialmente se centró en JavaScript y TypeScript, VSCode ahora ofrece soporte para una amplia variedad de lenguajes de programación.

- <span> Terminal integrada :</span> Incluye una terminal integrada que permite a los desarrolladores ejecutar comandos directamente desde el IDE.

Estas características proporcionan a los desarrolladores un entorno versátil y eficiente para trabajar en proyectos de desarrollo web. Cabe destacar que VScode no tiene capacidad para la compilación y ejecución de código directamente en el editor, tendremos que recurrir a otros métodos para ello.

### 1.2 Link video cambiar configuraciones en VS Code:

- [video](https://www.youtube.com/watch?v=uyEUVgNMvGI)

<br>

## 2. Terminal ó CMD

    Existen muchas aplicaciones de las que un desarrollador utiliza en su día a día que no se encuentran en su versión de escritorio, si no que se ejecutan a través de una línea de comandos.

    A través de una línea de comandos se pueden ejecutar tareas sencillas, pero también podemos accionar complejos flujos de trabajo que el sistema operativo no nos permite realizar a través de ventanas o botones predeterminados.

    Muchos frameworks de desarrollo, como pueden ser Angular o React, incluyen una herramienta por línea de comandos para poder ejecutar sus acciones más habituales. Comprender cómo funcionan estas herramientas agiliza y optimiza el día a día del programador.

### 2.1 Comandos basicos de terminal UNIX (Lynux/MAC)

- <u>pwd</u> = Para encontrar la ruta del directorio (carpeta) de trabajo actual en el que te encuentras.

- <u>cd</u> = cambiar directorio;

  - cd = para ir a la carpeta
  - cd .. = para ir un directorio hacia arriba.

- <u>ls</u> = lista del contenido del directorio.

  - ls -R = también listará todos los archivos en los subdirectorios.
  - ls -a = mostrará los archivos ocultos.
  - ls -al = listará los archivos y directorios con información detallada como los permisos, el tamaño, el propietario, etc.

- <u>cp</u> = copiar un archivo.

- <u>mv</u> = mover archivos.

- <u>mkdir</u> = crear un nuevo directorio.

- <u>rmdir</u> = solo elimina un directorio que estén vacíos.

- <u>rm</u> = para borrar recursivamente.

  - rm - r = Borra el contenido de la carpeta + la carpeta
    Nota: Este comando elimina y no se puede deshacer, ya que no va a la papelera de reciclaje

- <u>touch</u> = crea un archivo en blanco.

- <u>clear</u> = limpia la terminal.

- <u> cat</u> = muestra el contenido de un archivo de texto desde el propio CMD.

  <br>

### 2.2 Comandos basicos de terminal (Windows)

- <button>ctrl</button> + C = reiniciar la consola si se queda pillada.

- <u>cd</u> = cambiar directorio, con esto podemos acceder a una carpeta deseada.

  - cd ../ = De esta manera indicamos el sentido opuesto, osea una carpeta anterior.
  - cd / = Accedemos al directorio raiz. (C:\>)

- <u>dir</u> = lista del contenido del directorio o carpeta donde te encuentras, mostrando todas las subcarpetas o archivos que tiene".

- <u>mkdir</u> = para crear un directorio/carpeta.

- <u>new-item -itemtype file </u> + ( nombre del archivo . sufijo del archivo) = crea un archivo, directorio

- <u>copy</u> ó <u>cp</u> = copia uno o más archivos en la dirección que tu elijas.

- <u>move</u> ó <u>mv</u> = Traslada un archivo de una carpeta a otra sin necesidad de interfaz.

- <u>del</u> = Borra el archivo que pongas después del comando.

  - <u>rmdir</u> = solo elimina un directorio que estén vacíos.

- <u>md</u> = Puedes crear una carpeta a través del comando md nombredecarpeta.

- <u>type</u> ó <u> cat</u> = muestra el contenido de un archivo de texto desde el propio CMD.

- <u>cls</u> o <u>clear</u> = limpia la terminal en Power Shell, en CMD solo funciona cls.

- <u>rename-item</u> nombreArchivo.txt <u>-newName</u> nuevoNombre.txt = cambia el nombre d eun archivo, no se puede cambiar formato.

- <u>get-content</u> contenido1.txt | <u>set-content</u> pasteContenido.txt = copia el contenido de un archivo y lo pega en otro archivo. Si están en diferentes carpetas, habrá que añadir la ruta de la carpeta.

  Ejemplo : (<u>get-content</u> contenido1.txt | <u>set-content</u> ..\..\pasteContenido.txt)

<br>

## 3. Navegador

El navegador web no solo sirve para navegar por Internet, sino que también se convierte en una herramienta de desarrollo esencial.

No todos los navegadores permiten visualizar los elementos gráficos de la misma manera y no todos los navegadores van implementando los cambios producidos en las nuevas versiones de HTML, CSS o Javascript. Por ello, uno de los grandes trabajos que tiene el desarrollador de aplicaciones Front, es el de adaptar sus programas para que existan el menor número de diferencias entre navegador y navegador.

Como herramientas de desarrollo, recomendamos que uses Chrome o Firefox (existe una versión especial para desarrolladores).

Pincha en el nombre para acceder al link de descarga para que puedas acceder rápidamente e instalarlos en tu sistema.

- [GOOGLE CHROME](https://www.google.com/intl/es_es/chrome/) Es un navegador web rápido y seguro, con gran cantidad de extensiones disponibles y sincronización de datos entre dispositivos.

- [FIREFOX](https://www.mozilla.org/es-ES/firefox/new/) Es un navegador centrado en la privacidad, es de código abierto y cuenta con una gran cantidad de extensiones disponibles.

- [FIREFOX DEVELOPER EDITION](https://www.mozilla.org/es-ES/firefox/developer/) Es una versión para desarrolladores web que ofrece herramientas integradas para facilitar el trabajo de los desarrolladores web.
