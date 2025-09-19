# CLASE 02 -git desarrollo colaborativo
 ## .gitkeep
 Es un archivp que me permite hacer un commit para guardar una carpeta nio detectada cuando esta vascia

 ## .gitignore
 Arcchivo que me permite ignorar archivos o carpetas completas que no quiero que se guarden dentro del repositorio para que no lo suba y guarde dentro del repositorio 

 ## repaso comando basicos
 ## Marcar archivps que quiero que sean parte del proximo commit
 osea marcar archuvos que estan en el wd terminado y que quierp llevarlo al  area de confirmacion para que sean pare del proximo commit
 '''sh
 git add<nombre.archivo1><nombre-archivo2>
 git add <nombre-archivo>
 git 
 '''

 ## Ver el contenido deun commit hecho
 '''
 git show <hash>
 git show 235bf89

 ## Guardar los cambios en el remositorio
'''sh
git commit -m "Mensaje"
git commit # se abre el ditor para escribir el mensaje
git commit -a # se hace un add no se hace un add untracked y se abre el editor para escribir el mensaje
'''
**NOTA**: LOS MENSAJES IDEALMENTE PUEDEN TENER 80 CARACTERES
## Ver los commits dentro del repositorio
'''sh
git log #largo con detalle
git log --oneline # corto solo el mensaje
git log -2 #me muestra 2 commit del listados, los ultimos 2
--oneline-2 # corto solo el mensaje y solo los ultimos
'''