## Clase 04

## git stash
- exite dentro de git
* no se puede subir al remoto
*trabaja con una estructura de pila(se puede vulnerar)

## Listar los stashes

````sh
git stash loist
````

<<<<<<< Updated upstream
## Crear un stash
````sh
git satsh -m "mensaje descriptivo"
````

## Ver contenido del stash

````sh
git stash show<identificador del stash>
git stash show 0
git stgash show stash{0}
=======
## Recuoerar el stash

````sh
git stash pop #recupera el ultimo stash realizado y si no hya conflicto lo borra
````

## Aplicar un stash en particular

````sh
git stash apply 1 #stasht @{1}
git stash apply 2 #stasht @{2}
````
## Eliminar un stash en particular

````sh
git stash drop #borra el stash arriba de todo
git stash drop 1 #borra el primer stash
git stash drop 0 #borra el segundo stash stash
<<<<<<< HEAD
=======
````

## Git resets
Me permite deshacer commit . hay 3 tipos 

## Git resets soft
Me permite deshacer unos o varios commits y los cambios lo arroja al staging area

````sh
git resets --soft <hash>
````

## Git reset mixed (defauld)
Me permite desg¡hacer uno o varios commits y los cambios los arroja al wd

````sh
git reset <hash>
git reset --mixed <hash>
````

## Git reset had
Me permite deshaher uno o varios commits y los cambios los descarta(pierdo los cambios de los archivos)

````sh
git reset --hard <hash>
>>>>>>> feature/resets
````

## Trabajar con personas donde no conozco 
