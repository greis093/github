# GIT Y GITHUB

crear un **.gitignore** dentro de **.git** para crear una **FICHERO OCULTO** No se sube al GITHUB.

## CREAR O CAMBIAR PROYECTOS (carpetas) EN EL TERMINAL

- [x] **pwd** || _Ver en que proyecto (carpeta) estoy._
- [x] **cd ..**|| _Salir un proyecto anterior(carpeta anterior)._
- [x] **mkdir nombre_proyecto** || _Crear un nuevo proyecto (carpeta)._
- [x] **pwd** || _Ver en que proyecto (carpeta) estoy._
- [x] **cd nombre_proyecto** || _Me coloco en el proyecto (carpeta) que acabo de crear._
- [x] **pwd** || _Verifico que estoy en la carpeta recien creada._

## CREAR FICHEROS CON EL TERMINAL

_Primero creamos nuestro git init_

- [x] **touch fichero1.txt** || _Creamos nuestro primer fichero._
- [x] **ls** || _Vemos los cambios._
- [x] **cat fichero1.txt** || _Vemos el contenido del fichero._
- [x] **clear** || _Limpiar el terminal._

## SUBIR MI PRIMER PROYECTO AL REPOSITORIO GITHUB

- [x] **git init** || _Crea un nuevo subdirectorio llamado .git que es el esqueleto de GIT._
- [x] **git add .** (adjuntar todo) ó **git add "nombre archivo"** || _Para colocar el archivo en un área de preparación._
- [x] **git commit -m "nombre del commit"** || _Confirmamos los cambios con un commit._
- [x] **git commit -amend -m "nuevo nombre"** || _Si deseo editar el commit realizado._
- [x] **git branch -M main** || _Esta estableciendo o creando la Rama main._
- [x] **git remote add origin git@github.com:greis093/proyectoGITHUB.git** || _Se copia el enlace de nuestro GITHUB para enlazarlo._
- [x] **git push -u origin main** || _Sube tus cambios de la rama main al remoto origin y establece la relación de seguimiento para facilitar futuros push y pull en esa rama._

## SUBIR LOS CAMBIOS AL GITHUB

- [x] **git pull origin main** || _Traer los cambios del repositorio._
- [x] **ls** || _vemos cambios de otras personas._
- [x] **git add .** ó **git add "nombre archivo"**|| _Para colocar el archivo en un área de preparación._
- [x] **git commit -m "nombre del commit** || _Confirmamos los cambios con un commit._
  - **git show id_commit** || _Muestra la información (mensaje,fecha,autor,cambios realizados-diff en ese commit)._
  - **git show** || _Muestra el ID del último commit._
  - **git show --stat id_commit** || _Ver un resumen del commit (resumen,modificaciones,lo eliminado)._
- [x] **git push origin main** || _Guarda todos los cambios en el GITHUB._

## CREAR NUEVAS RAMAS

- [x] **git branch** || _Visualizar en que rama nos encontramos lo muestra con un \*_
  - **git branch -a** || _Muesta rama remota y rama local._
- [x] **git branch nombre_rama** || _Crea una nueva rama partir de la rama en la que estamos._
- [x] **git switch nombre_rama** || _Moverse a la rama creada._
- [x] **git switch master** || _Regresamos a la rama principal._
- [x] **cat nombre_rama** || _Revisamos los cambios de la rama creada._

  ### SUBIR MI RAMA CREADA A MI GITHUB

  - [x] **git add .** ó **git add "nombre archivo"**
  - [x] **git commit -m "nombre del commit"**
  - [x] **git push origin nombre_rama**

## CAMBIAR NOMBRE DE UNA RAMA

- [x] **git branch** || _Visualizar en que rama nos encontramos lo muestra con un \*._
- [x] **git branch -m renombrar_rama** || _Renombramos la rama._

## ELIMINAR UNA RAMA

- [x] **git branch -d nombre_rama** || _Eliminar un rama (no debemos estar en esa rama)._
- [x] **git branch -D nombre_rama** || _Eliminar un rama **no fusionada** pide esta confirmación adicional._
- [x] **git branch** || _Verificamos que la rama no se encuentra \*._

## UNIR RAMAS - MERGE

1.  FAST FORWARD MERGE : Unir una rama_A (no tiene cambios) con otra rama_B (con cambios).
2.  MERGE SIN CONFLICTOS: Unir una rama_A (con cambios) con otra rama_B (con cambios).
3.  MERGE CON CONFLICTOS: Unir una rama_A (cambios fichero_X) con otra rama_B (cambios fichero_X).
    - Mantener los ramos de una rama o modificar manualmente los cambios

- [x] **git branch** || _Visualizar en que rama nos encontramos lo muestra con un \*_
- [x] **git switch master** || _Cambiar a la rama master_
- [x] **git branch** || _Verificar que estamos en la rama master \*_
- [x] **git merge nombre_rama -m "nombre_commit"** || _Unirlo a la rama master_
  - **git merge --abort** || _Si deseas desacer el merge._

### REVISAR FICHEROS ANTES DE SUBIRLOS A GITHUB

- [x] **git diff** || _Nos muestra el cambio que **No han sido añadidos en la zona de praparación**._
- [x] **git diff HEAD fichero1.txt fichero2.txt** || _Mostar diferencias entre el último commit y el fichero (zona de trabajo)._
- [x] **git diff --cached** || _Mostrar diferencias entre el último commit realizado y la zona de preparación (git add)._
- [x] **git diff commit1 commit2** || _Mostrar diferencias entre 2 commit \*._
  - **git log --oneline** || _Detalle de los commit._

## GUARDAR CAMBIOS CUANDO NO QUEREMOS USAR COMMIT

- [x] **git stash** || _Guarda los cambios sin hacer commit (se guarda a partir del ultimo commit)._
- [x] **git stash apply** || _Recuperar varias veces los cambios de **git stash**._
- [x] **git stash pop** || _Recupera los cambios de **git stash** (ya no se vuelve a recuperar el **git stash**)._
- [x] **git stash list** || _Lista los cambios guardador varias veces por **git stash**._
- [x] **git stash drop stash@{N}** || _Borrar los cambios guardados en **git stash**._
- [x] **git stash clear** || _Borrar todos los cambios guardados en **git stash**._

## MOVERSE ENTRE COMMIT

- [x] **git log --oneline** || _Ver el ID de los commit._
- [x] **git checkout id_commit** || _Permite moverse a otro commit._
- [x] **git checkout master~1** || _Volver un commit anterior de la rama master (master~N)._

## RESTABLECER FICHEROS

- [x] **git restore fichero1.txt** || _Restaurar fichero a como estaba en el último commit._
- [x] **git restore --source HEAD~1 fichero1.txt** || _Cambia la fuente desde donde se restaura el fichero._
- [x] **git restore --staged fichero1.txt** || _Quitar de la zona de preparación el fichero(se elimino el git add)._

## ELIMINAR COMMIT

- [x] **git reset id_commit** || _Elimina el commit hasta el commit indicado (permanentemente)._
  - **git log --oneline**|| _Verificar los commit._
    _Si trabajas en **Equipo** utiliza el *revert* que no lo elimina crea uno nuevo indicando el borrado._
- [x] **git revert id_commit** || _Regresa al commit indicado._

## CLONAR UN REPOSITORIO DE GITHUB

_Primero crear tu **.git** con git init_

- [x] **git clone https://ruta_repositorio_clonar** || _Copiamos la ruta del repositorio que clonaremos._
