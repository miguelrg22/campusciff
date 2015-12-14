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

echo privado.txt > .gitignore

echo privada/ > .gitignore

