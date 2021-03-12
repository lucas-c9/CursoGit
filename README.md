<h1 align="center">GIT</h1>
<p align = "center">💡 Conceptos y comandos para entender mejor el funcionamiento de Git.</p>

## Table of Contents

- [git init](#init)
- [git clone](#clone)
- [git status](#status)
- [git show](#show)
- [git log](#log)
- [git blame](#blame)
- [git branch](#branch)
- [git checkout](#checkout)
- [git merge](#merge)
- [git add](#add)
- [git commit](#commit)
- [git pull](#pull)
- [git push](#push)
- [git help](#help)

## Git init<a name = "init"></a>

El comando `git init` crea un nuevo repositorio local en el directorio donde ejecutemos el comando.
Esto crea un subdirectorio nuevo llamado .git, el cual contiene todos los archivos necesarios del repositorio (un esqueleto de un repositorio de Git). 
Todavía no hay nada en tu proyecto que esté bajo seguimiento hasta no agregar archivos con el comando `git add`.

## Git clone<a name = "clone"></a>

## Git status <a name = "status"></a>

## Git show <a name = "show"></a>
El comando show se utiliza para mostrar informacion sobre cualquier objeto git 

## Git log <a name = "log"></a>
El comando git log se utiliza para exporar el historial del repositorio.

## Git blame <a name = "blame"></a>
El comando git blame se usa para examenit contenido de un archivo y ver cuando se modifico y quien lo modifico

## Git branch <a name = "branch"></a>

Con el comando `git branch` podemos "ver" las ramas que fueron creadas en nuestro repositorio, saber cual es la rama actual y tambien crear nuevas ramas.

su sintaxis es:

`git branch`   ---> para conocer le listado de todas las ramas, se muestra con "asterisco"<nombre> y destacada en color la rama actual

`git branch <nuevarama>` permite crear una rama nueva de nombre <nuevarama>


## Git checkout <a name = "checkout"></a>

El comando `git checkout` te permite navegar entre las ramas creadas por `git branch`. Verificar una rama actualiza los archivos en el directorio de trabajo para que coincidan con la versión almacenada en esa rama, y ​​le dice a Git que registre todas las nuevas confirmaciones en esa rama.

La sintaxis basica del comando es:

     `git checkout [-q] [-f] [-m] [<branch>]`


   Uno de los parametros mas usados y recomendados es -b que sirve para crear una nueba rama y cambiar automaticamente a ella.

     `git checkout -b <new_branch>`

## Git merge <a name = "merge"></a>

El comando `git merge <rama>` sirve basicamente para "fusionar" ramas de trabajo.

Para hacer un merge nos situamos en una rama, en este caso la "master", y decimos con qué otra rama se debe fusionar el código.

El siguiente comando, lanzado desde la rama "master", permite fusionarla con la rama "experimental".

	`git merge experimental`

Cuando varias personas trabajan en un desarrollo y cada una lleva adelante el manteniemiento, desarrollo y/o actualización de una parte del código, cada una de ellas debería abrir una rama para trabajar y luego de terminado el desarrollo o actualización "fusionar" su trabajo a la rama general de código.
Esto es lo que hace Merge.


## Git add <a name = "add"></a>
El comando add sirve para agregar los archivos que hemos modificados para luego estos agregarlos a un commit.
`git add archivo.txt` este comando agregara unicamente archivo.txt. Es decir sirve para agregar archivo por archivo que ha sido modificado
`git add .` este comando agregara todo los archivos que han sido modificados automaticamente.
## Git commit <a name = "commit"></a>
El comando commit sirve para que una vez agregado los archivos que hemos modificados estos sean agrupados en un commit, ademas el mismo puede tener un mensaje detallando que cambios hemos realizados o caracteristicas que hemos agregado.
`git commit` este comando agrupara los archivos que hemos modificados en un commit. Una vez ejecutado este comando se nos abrira un editor de texto para agregar un mensaje acerca del commit realizado.
`git commit -m "Mensaje"` este comando es similar a los anterior, solo que podemos agregar entre las comillas el mensaje de manera mas rapida.
## Git pull <a name = "pull"></a>

## Git push <a name = "push"></a>

## Git help <a name = "help"></a>
El commando help sirve para acceder de manera mas detallada a los parametros que utiliza un comando en especifico o sobre git. Esto nos ayudara a entender que otras funcionalidades puede tener el mismo.
`git help` este comando muestra todas las funciones que podemos realizar con una breve descripcion de las mismas.
`git [comando] --help` este comando nos mostrara especificamente que funcionalidades extra o parametros a utilizar son acerca de ese comando.
