## 1. ¿Qué es Git?

Es un software para llevar el control de las diferentes versiones de nuestro código. Fué creado pensando en la eficiencia y la confiabilidad del mantenimiento de versiones.

Git permite a los desarrolladores colaborar de manera eficiente al mantener un historial completo de revisiones, facilitando la identificación de cambios, la resolución de conflictos y la gestión de ramas.

Tambien permite llevar un control de cambios muy exhaustivo, y en caso de error, siempre podremos recuperar versiones anteriores o más estables.

[video](https://www.youtube.com/watch?v=jGehuhFhtnE)

## 1.1 Características

- <u> Sistema de control de versiones distribuido:</u> Esto significa que el código existe, tanto localmente como en un repositorio remoto, permitiendo un seguimiento completo y descentralizado de los cambios.

- <u> Trabajo desconectado:</u> Posibilita el acceso al historial completo del código incluso en situaciones sin conexión a internet, facilitando la continuidad del desarrollo desde cualquier lugar, como en un portátil.

- <u> Suspensión de trabajos:</u> Permite pausar el desarrollo para abordar incidencias en producción, proporcionando flexibilidad para gestionar tareas críticas.

- <u> Commits atómicos:</u> Con la zona de stage, Git permite trabajar con distintos commits, fortaleciendo la capacidad de seleccionar y organizar tanto archivos como partes específicas de los mismos.

- <u> Flujos de trabajo con ramas:</u> Posibilita la creación de ramas para aislar partes del desarrollo, permitiendo una gestión eficiente y organizada del flujo total del proyecto.

- <u> Bajo residuo:</u> Toda la información se encuentra en una carpeta única .git, en la raíz del proyecto, lo que permite un manejo sencillo y modular de la información.

- <u> Interfaz amigable:</u> A pesar de ser una herramienta de línea de comandos, Git cuenta con interfaces gráficas que facilitan su uso, adaptándose a usuarios con diferentes niveles de experiencia.

- <u-> Acceso sin cliente:</u-> La capacidad de acceder a cualquier repositorio de Git sin necesidad de tener un cliente específico proporciona flexibilidad y accesibilidad.

- <u> Multiservidor: </u> Permite tener varios repositorios, lo que resulta útil para separar proyectos de clientes y desarrollo en un servidor, y aborda problemas legales al rastrear cambios y responsabilidades en el código.

## [Comandos de GIT básicos](https://www.hostinger.es/tutoriales/comandos-de-git)

[Pagina oficial Git](https://git-scm.com/docs)

Aquí hay algunos comandos básicos de GIT que debes conocer:

### git init:

Creará un nuevo repositorio local GIT.

El siguiente comando de Git creará un repositorio en el directorio actual:

        git init

Como alternativa, puedes crear un repositorio dentro de un nuevo directorio especificando el nombre del proyecto:

        git init [nombre del proyecto]

---

### git clone

Se usa para copiar un repositorio.

Si el repositorio está en un servidor remoto, usa:

        git clone nombredeusuario@host:/path/to/repository

A la inversa, ejecuta el siguiente comando básico para copiar un repositorio local:
git clone /path/to/repository

---

### git add

Se usa para agregar archivos al área de preparación.

Por ejemplo, el siguiente comando de Git básico indexará el archivo temp.txt:

        git add <temp.txt>

---

### git commit

Creará una instantánea de los cambios y la guardará en el directorio git.

        git commit –m “El mensaje que acompaña al commit va aquí”

Consejo profesional
Ten en cuenta que los cambios confirmados no llegarán al repositorio remoto.

---

### git ni

crear un archivo vacio

### git status

Muestra la lista de los archivos que se han cambiado junto con los archivos que están por ser preparados o confirmados.

        git status

---

### git push

Se usa para enviar confirmaciones locales a la rama maestra del repositorio remoto.

Aquí está la estructura básica del código:

        git push origin <master>

---

---

<SPAN>Consejo profesional:

Reemplaza <master> con la rama en la que quieres enviar los cambios cuando no quieras enviarlos a la rama maestra.</SPAN>

---

---

### git checkout

Crea ramas y te ayuda a navegar entre ellas.
Por ejemplo, el siguiente comando crea una nueva y automáticamente se cambia a ella:

        command git checkout -b <branch-name>

Para cambiar de una rama a otra, sólo usa:

        git checkout <branch-name>

---

### git remote

Te permite ver todos los repositorios remotos.

El siguiente comando listará todas las conexiones junto con sus URLs:

        git remote -v

Para conectar el repositorio local a un servidor remoto, usa este comando:

        git remote add origin <host-or-remoteURL>

Por otro lado, el siguiente comando borrará una conexión a un repositorio remoto especificado:

        git remote <nombre-del-repositorio>

---

### git branch

Se usa para listar, crear o borrar ramas.

Por ejemplo, si quieres listar todas las ramas presentes en el repositorio, el comando debería verse así:

        git branch

Si quieres borrar una rama, usa:

        git branch -d <branch-name>

---

### git pull

Fusiona todos los cambios que se han hecho en el repositorio remoto con el directorio de trabajo local.

        git pull

---

### git merge

Se usa para fusionar una rama con otra rama activa:

        git merge <branch-name>

---

### git diff

Se usa para hacer una lista de conflictos.

Para poder ver conflictos con respecto al archivo base, usa:
git diff --base <file-name>

El siguiente comando se usa para ver los conflictos que hay entre ramas antes de fusionarlas:

        git diff <source-branch> <target-branch>

Para ver una lista de todos los conflictos presentes usa:
git diff

---

### git tag

Marca commits específicos. Los desarrolladores lo usan para marcar puntos de lanzamiento como v1.0 y v2.0.

        git tag 1.1.0 <instert-commitID-here>

---

---

### git config

Puede ser usado para establecer una configuración específica de usuario, como el email, nombre de usuario y tipo de formato, etc.

Por ejemplo, el siguiente comando se usa para establecer un email:

        git config --global user.email tuemail@ejemplo.com

La opción -global le dice a GIT que vas a usar ese correo electrónico para todos los repositorios locales.

Si quieres utilizar diferentes correos electrónicos para diferentes repositorios, usa el siguiente comando:
git config --local user.email tuemail@ejemplo.com

### git reset

Sirve para resetear el index y el directorio de trabajo al último estado de confirmación.

        git reset - -hard HEAD

---

---

### git log

Se usa para ver el historial del repositorio listando ciertos detalles de la confirmación.

Al ejecutar el comando se obtiene una salida como ésta:

        commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw
        Author: Alex Hunter <alexh@gmail.com>
        Date: Mon Oct 1 12:56:29 2016 -0600

---

### git rm

Se puede usar para remover archivos del index y del directorio de trabajo.

        git rm filename.txt

---

### git stash

Guardará momentáneamente los cambios que no están listos para ser confirmados. De esta manera, pudes volver al proyecto más tarde.

        git stash

---

### git show

Se usa para mostrar información sobre cualquier objeto git.

        git show

---

### git fetch

Le permite al usuario buscar todos los objetos de un repositorio remoto que actualmente no se encuentran en el directorio de trabajo local.

        git fetch origin

---

### git ls-tree

Te permite ver un objeto de árbol junto con el nombre y modo de cada ítem, y el valor blob de [SHA-1.](https://es.wikipedia.org/wiki/Secure_Hash_Algorithm)

Si quieres ver el HEAD, usa:

        git ls-tree HEAD

---

### git cat-file

Se usa para ver la información de tipo y tamaño de un objeto del repositorio.

Usa la opción -p junto con el valor [SHA-1.](https://es.wikipedia.org/wiki/Secure_Hash_Algorithm) del objeto para ver la información de un objeto específico, por ejemplo:

        git cat-file –p d670460b4b4aece5915caf5c68d12f560a9fe3e4

---

### git grep

Le permite al usuario buscar frases y palabras específicas en los árboles de confirmación, el directorio de trabajo y en el área de preparación.

Para buscar por www.hostinger.com en todos los archivos, usa:

        git grep “www.hostinger.com”

---

### gitk

Muestra la interfaz gráfica para un repositorio local.

Simplemente ejecuta:
gitk

---

### git instaweb

Te permite explorar tu repositorio local en la interfaz GitWeb.

Por ejemplo:

        git instaweb –http=webrick

---

### git gc

Limpiará archivos innecesarios y optimizará el repositorio local.

        git gc

---

### git archive

Le permite al usuario crear archivos zip o tar que contengan los constituyentes de un solo árbol de repositorio.

Por ejemplo:

        git archive - -format=tar master

---

### git prune

Elimina los objetos que no tengan ningún apuntador entrante.

        git prune

---

### git fsck

Realiza una comprobación de integridad del sistema de archivos git e identifica cualquier objeto corrupto

        git fsck

---

### git rebase

Se usa para aplicar ciertos cambios de una rama en otra.

Por ejemplo:

        git rebase master

---
