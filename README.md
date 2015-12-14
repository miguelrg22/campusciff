# EJERCICIO

## Creo un directorio local de trabajo.

$ mkdir ejercicioGit

$ cd ejercicioGit

Inicializo en ejercicioGit git creando el archivo .git 

$ git init


## 2.1 Crear un repositorio en vuestro GitHub llamado campusciff.


## 2.2 Clonamos nuestro repositorio en local.

$ git clone

$ cd campusciff

## 2.3 Creamos un documento **README.md** donde vamos incorporando los comandos, explicaciones y capturas de pantalla necesarias.

$ touch README.md

$ vi README.md

$ git add .

Añado con add . todos los arhivos a  _Staging área_ , que en este caso sólo se añade *README.md*.

## 2.4 Hacemos un commit con el mensaje *commit inicial*.

$ git commit -m "commit inicial"

## 2.5 Subimos los cambios al repositorio remoto.

$ git push -u origin master

## 2.6.1 Creamos en el repositorio local un fichero llamado *privado.txt*.

$ touch privado.txt

## 2.6.2 Creamos en el repositorio local una carpeta llamada *privada*.

$ mkdir privada

## 2.7 Realizar los cambios oportunos para que el archivo y la carpeta sean ignorados por git.

Creo el archivo .gitignore

$ touch .gitignore

Añado a a lista de excepciones privado.txt y privada.

$ echo privado.txt > .gitignore

$ echo privada/ > .gitignore

Guardo los comandos en README.md y lo subo a GitHub.

$ git add .

$ git commit -m "completado el archivo README.md"

$ git push origin master


## 2.8 Añado un fichero *1.txt* al repositorio local.

$ touch 1.txt

## 2.9 Creo un **tag v0.1**.

$ git tag v0.1

Guardos los cambios con otro commit 

$ git add .

$ git commit -m "añadida etiqueta v0.1"

## 2.10 Subir los cambios al repositorio remoto.

$ git push --tag origin master

## 2.11 Crear una **rama v0.2**.

$ git branch v0.2

Guardo los cambios 

$ git add .

$ git commit -m "añadida rama v0.2"
