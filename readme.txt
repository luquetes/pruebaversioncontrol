Version Control
---------------

Version Control básicamente es una manera organizada de poder compartir archivos. Lo usa cualquier equipo de trabajo mínimamente serio, donde haya una X cantidad de desarrolladores laburando sobre un mismo proyecto.

Existen un montón de herramientas para ésto, como por ejemplo SVN o git

El más conocido y el más popular y el más moderno es nada más y nada menos que "git".

git es un servicio o un sistema de línea de comandos que te permite ejecutar, desde una consola, determinados comandos a través de los cuales podés conectarte a un "REPOSITORIO" remoto.

Qué CARAJO es un repositorio? y por qué es remoto?
-------------

El repositorio es aquel lugar donde toooooodo nuestro laburo se va a estar subiendo. Es remoto porque está hosteado en git (más precisamente, en github, que es el sitio de git donde cualquier persona del mundo que se cree una cuenta puede subir sus proyectos)


Ok, cómo subo mi proyectoooo?
-----------------------------

En primer lugar, y cuando ya tenemos una cuenta de github creada, tenemos que ir a nuestro perfil y crear un repositorio (es el botón ese verde que dice New)

Una vez creado el repositorio, lo que queda es subir nuestro proyecto. Subir nuestro proyecto por primera vez se llama "inicializar".
Tooodos los pasos necesarios te los da github porque es re copado, y solamente hay que seguir el orden que indica.

Para ésto, hay que usar el comando "git init".

Este comando crea un repositorio local en la carpeta donde estemos parados. Para crearlo, lo que hace es simplemente crear una carpetita que se llama ".git", que es la encargada de llevar un control total de tooodos los cambios que ocurran en nuestra aplicación o nuestro sitio de manera local, o sea en nuestra computadora.

Al mismo tiempo, podemos ver que al inicializar el repo, nos aparece un (master) en azul al lado de la ruta en la que estamos parados.
Ese nombrecito que aparece en azul se llama "branch", y nos está mostrando en qué branch estamos parados.
Por defecto, nos deja en la branch master, que es la branch principal de todo el proyecto.

Existen una BANDA de comandos en git, de los cuales en el día a día en cualquier laburo, solamente se usan unos pocos.

git init: Es el que ya vimos, que nos permite inicializar un proyecto. Si ya tenemos un proyecto armado, o nos bajamos/clonamos un proyecto externo, no hace falta correrlo.

git status: Este es bastante útil, porque te devuelve el status actual del branch en el que estés parado.

git add: Este sirve registrar qué se va a commitear. Todo aquello que no se registre, no va a entrar en el commit, por ende no se va a guardar cuando querramos subir nuestros cambios al repositorio remoto.
Para registrar un archivo, es tan fácil como hacer "git add" y luego el nombre del archivo.
Por otro lado, si usamos "git add" y punto (.), todos los archivos sin registrar (en rojo), pasan a ser registrados (en verde!)

git commit: Esto lo que hace es generar un "paquete" donde van a estar todos los archivos que nosotros queremos subir. Al generar un paquete aislado, cualquier cambio posterior que hagamos a los archivos, habrá que registrarlos y commitearlos de nuevo si es queremos subirlos también.

git commit -m: Sirve para acompañar el commit de un mensaje. Esto es extremadamente util, porque les sirve a los demás compañeros de tu equipo, poder identificar qué es lo que estás subiendo.
El mensaje va entre comillas!

git push: Sirve para subir cambios a un repositorio. Para ésto es necesario indicarle a nuestro repositorio local dónde subirlo. Es decir, indicarle un destino. Para esto usamos git remote add origin (esto se ve igual en el propio repositorio remoto cuando lo creás por primera vez)

git pull: Así como existe git push para SUBIR cambios, existe git pull para BAJAR cambios, actualizándonos para estar en el mismo punto que el resto del equipo. Como buena práctica, se recomienda siempre que antes de empezar a trabajar, siempre hacer un git pull. SIEMPRE. SIEEEEEEMPRE.
