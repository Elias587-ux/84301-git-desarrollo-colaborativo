## Clase 3 
## Estados de los archivos
git status
## Agregar a la zona de staging area o index area de confirmacion
git add <nombre-archivo>
git add . #todos los archivos

## pERSISTIR  los archivos que coloco en elc staging area hacer un commit
git commit -m "mensaje"
git  commit #abre el editor de texto y me permite escribir un mensaje

## Ver commits que hice
git log #forma larga
git log --oneline # Forma corta
git log -5 # Cantidad de commits que quiero que muestre
## Como veo la diferencia entre lo que tengo en el working directory y local repo

git diff

## Ver la diferencia entre 2 ramas .La rama main y la rama dev
poner el nombre de la rama
git sgit <nombre- rama>
git switch main
git diff dev

## Como arreglo el mensaje de un commit 
git add <archivo-que-me-olvide>
git commit --amend # ademas de corregir el mensaje Tambien podemos comentar,agregar archivos que te faltaron/olvide en el staging area
## Como creo una rama

git branch <nombre-rama>
## Cambiarse de rama
````sh
git switch <nombre-rama>
````
## fusionar dos ramas
````sh
git merge <nombre-rama>
si me quiero traer los cambios en dev de la rama main
git switch main
git merge dev
````

## Hacer un commit sin cambiar el mensaje pero agregadon archivos o en linea de guardar dentro de commit
````sh
git add . #Agrego los archivos que fueron modificados
git commit --amend --no-edit # evito cambiar el mensaje
````
## Agregar modificavcione sde archivos granularmente AGREGAR PARTED DEL CODIGO AGREGADON EN UN ARCHIVO
````sh
git add --patch
````
## Git alias
## Crear un alias
````sh
git config --global alias.s "status"
git config --global alias.sc "status --short"
git config --global alias.ll "log"
git config --global alias.l "log --oneline"
git config --global alias.amend "commit --amend --no-edit"
git config --global alias.c "commit -m"
````
## Para ver los alias
## lsitar los alias que tengo cargado
````sh
git config --list
git config --get-regexp alias
````