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


## 2.13 Subir los cambios al repositorio remoto.

$ git push origin v0.2

$ git checkout master

$ git push origin master 

Para subir todos los cambios realizados a GitHub, ya sean en la rama v0.2 como en la master. 


## 2.14.1 Posicionarse en la rama **master**.

$ git checkout master #Aunque me he posicionado en el paso anterior.

## 2.14.2 Hacer _merge_ de la rama **v0.2** en la rama _master_.

$ git merge v0.2

## 2.15 En la rama master poner _Hola_ en el fichero 1.txt y hacer commit.

$ echo "Hola" > 1.txt

$ git add .

$ git commit -m "añadido Hola a 1.txt"

## 2.16 Posicionarse en la rama **v0.2** y poner _Adios_ en el fichero 1.txt y hacer commit.

$ git checkout v0.2

$ echo "Adios" > 1.txt

$ git add .

$ git commit -m "añadido Adios a 1.txt"

## 2.17 Posicionarse de nuevo en la rama master y hacer merge con la rama v0.2.

$ git checkout master

$ git merge v0.2

Se encuentra un fallo en el merge en el archivo 1.txt

## 2.18 Listar las ramas con merge y las ramas sin merge.

Para saber cuales están con merge

$ git branch --merged  #Que es la rama master

$ git branch --no-merged  #Que es v0.2


## 2.19 Arreglar el conflicto anterior en 1.txt y hacer commit.

Entro en 1.txt

$ vi 1.txt  #Borro todo menos Hola.

$ git add .

$ git status  #Y compruebo que no hay problemas ahora, para así seguir con el commit.

$ git commit -m "merge solucionado"

## 2.20.1 Crear un tag **v0.2**.

$ git tag v0.2

## 2.20.2 Borrar la rama **v0.2**.

$ git branch -d v0.2

## 2.21 Listar los distintos commits con sus ramas y sus tags.

$ git log

Para ver de una forma más esquemática esos commits con sus ramas y tags.

$ git log --oneline --decorate --graph --all




![Observamos que sólo queda la rama master](\campusciff\gitlog.jpg)



## 2.24 Crear tabla de varios compañeros de clase:



| NOMBRE | GITHUB   |
|--------|-----------|
| Amalia Suárez García |   [asuarezg](https://github.com/asuarezg)      |
| Carlos Alberto Paz Santos  | [cpazsantos](https://github.com/cpazsantos)|
| José Antonio Rita Gordillo | [jaritgor](https://github.com/jaritgor) |
| Patricia Iglesias Mateos   | [Pimateos](https://github.com/Pimateos) |


## 2.25

Ok.

## 2.26

Ok.

## 2.27

Ok.

## 2.28

Ok.

## 2.29

Ok.

## 2.30

Ok.
