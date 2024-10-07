# GIT Y GITHUB

crear un **.gitignore** dentro de **.git** para crear una **FICHERO OCULTO** No se sube al GITHUB.

## CREAR O CAMBIAR PROYECTOS (carpetas) EN EL TERMINAL

- [x] **pwd** || _Ver en que proyecto (carpeta) estoy_
- [x] **cd ..**|| _Salir un proyecto anterior(carpeta anterior)_
- [x] **mkdir nombre_proyecto** || _Crear un nuevo proyecto (carpeta)_
- [x] **pwd** || _Ver en que proyecto (carpeta) estoy_
- [x] **cd nombre_proyecto** || _Me coloco en el proyecto (carpeta) que acabo de crear_
- [x] **pwd** || _Verifico que estoy en la carpeta recien creada_

## CREAR FICHEROS CON EL TERMINAL

_primero creamos nuestro git init_

- [x] **touch fichero1.txt** || _Creamos nuestro primer fichero_
- [x] **ls** || _vemos los cambios_
- [x] **cat fichero1.txt** || _Vemos el contenido del fichero_
- [x] **clear** || _Limpiar el terminal_

## SUBIR MI PRIMER PROYECTO AL REPOSITORIO GITHUB

- [x] **git init** || _Crea un nuevo subdirectorio llamado .git que es el esqueleto de GIT._

- [x] **git add .** (adjuntar todo) ó **git add "nombre archivo"** || _Para colocar el archivo en un área de preparación._

- [x] **git commit -m "nombre del commit"** || _Confirmamos los cambios con un commit._

- [x] **git commit -amend -m "nuevo nombre"** || _Si deseo editar el commit realizado._

- [x] **git branch -M main** || _Esta estableciendo o creando la Rama main._

- [x] **git remote add origin git@github.com:greis093/proyectoGITHUB.git** || _Se copia el enlace de nuestro GITHUB para enlazarlo_

- [x] **git push -u origin main** || _Sube tus cambios de la rama main al remoto origin y establece la relación de seguimiento para facilitar futuros push y pull en esa rama._

## SUBIR LOS CAMBIOS AL GITHUB

- [x] **git pull origin main** || _traer los cambios del repositorio_
- [x] **ls** || _vemos cambios de otras personas_
- [x] **git add .** ó **git add "nombre archivo"**|| _Para colocar el archivo en un área de preparación._
- [x] **git commit -m "nombre del commit** || _Confirmamos los cambios con un commit._
- [x] **git push origin main** || _Guarda todos los cambios en el GITHUB_

## CREAR NUEVAS RAMAS

- [x] **git branch** || _Visualizar en que rama nos encontramos lo muestra con un \*_
- [x] **git branch nombre_rama** || _Crea una nueva ramaa partir de la rama en la que estamos_
- [x] **git switch nombre_rama** || _Moverse a la rama creada_
