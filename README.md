# Apuntes de Clase De Python
## Contenido
Dentro de este readme se encuentran codigos realizados en clase de python (que cree con ayuda de [Manuel Sáenz](https://github.com/manuelsaenz), no pude compartir el repositorio por que este era privado y yo no era dueño), en el repositorio tambien se encuentra una captura de la creacio nde una variable de entorno y de un perfil en Visual Studio Code.

# Comandos
## Bash
### Comandos
- `pwd`: Muestra ruta actual (print working directory).
- `clear`, `cls`: Limpia la terminal.
- `promp_dirtrim=#`: cantidad de caracteres a mostrar.
- `help`: Muestra los comandos y su función.
- `cd ruta`: Cambio de directorio (Change directory).
- `cd ..`: Regreso de directorio.
- `mkdir Nombre`: make directory “” (crea un directorio).
- `>`: Agrega el resultado de un comando a un archivo y sustituye lo existente en dicho archivo.
- `>>`: Agrega texto manteniendo el anterior.
- `touch`: Crea un archivo.
- `rd -rf ruta`: Remueve un directorio (-rf: remueve con recursividad).
- `cat`: Muestra contenido de un texto.
- `echo`: Imprime en pantalla.
- `ls -a, -l, -al`: Muestra los archivos, (-a: muestra lo oculto, -l: muestra atributos, -al: combina los anteriores)
- `history`: Muestra el historial.
- `!numero`: Pone la instrucción del indice del historial.
- `alias NombreDelAlias = ´instrucciones a realizar´`: Crea un alias con esa instruccion, alias sin opciones muestra los alias existentes.
- `mv nombreViejo nombreNuevo`: Cambia el nombre de un archivo.
- `code ruta/archivo`: Abre VSC con la ruta o el archivo.
- `exit`: Cierra sesion/terminal.
- `explorer ruta`: Abre el explorador de archivos en la ruta especificada
- `python --version`: Imprime version de Python.
- `python archivo.py`: Ejecuta archivo en Python.
- `ll`: Es un alias a ls -l

## GIT
Configuracion antes de realizar algun commit
~~~
git config --global user.name = "Nombre"
git config --global user.email = "correo@dominio.com"
~~~

- `git status`: Estatus del archivo.
- `git diff`: Muestra los cambios.
- `git init`: Inicia el proyecto.
- `git add archivo`: Agrega el archivo al staging area.
- `git commit --amend -m ""`: Crea punto de guardado (--amend agrega al ultimo commit (incluye archivos)).
- `git restore -–staged`: Retorna al último commit guardado.
- `git checkout hash`: retorna a la version del hash mencionado.
- `git clone`: Clona el repositorio del link.
- `git switch rama`: Cambia a una rama //No usar.
- `git commit -am “mensaje”`: Subir cambios al commit de una.
- `git switch -c "nombreDeLaRama"`: Crear una nueva rama y se cambia a ella //No usar.
- `git merge --abort "nombreDeLaRama"`: Fusiona los commits de las rama especificada en la rama actual (--abort aborta el merge, no lleva el nombre de rama).
- `git branch -M --all nombreDeLaRama`: --all: muestra las ramas, con el nombre de la rama: crea una nueva rama, -M rama: establece la rama como main?
- `git remote add origin link`: Agregar un conexión remota.
- `git remote show origin`: Muestra la conexion remota.
- `git checkout nombreDeLaRama`: Cambiamos de rama.
- `git log --oneline --all --graph --decorate`: Muestra todos los registros de commit de todas las ramas decorado en una grafica, cada rama en una linea.
- `git push -u origin main/--all`: Hace un push (commit a la nube) a la conexion remota de la rama especificada (o todas en el caso de --all).
- `git pull origin main`: Hace una actualizacion del codigo encontrado en la conexion remota, de la rama especificada.
- `git fetch origin main`: Obtiene los datos del repositorio remoto, y los agrega a la rama espejo.
- `git rm --cache`: elimina el cache de los proyectos.

## Vim
- `I`: Cambia al modo de insercion.
- `ESC`: Cambia al modo codigo
- `:wq`: Sirve para salir y guardar los cambios.
- `:q!`: :q sale, :q! sale sin guardar nada

## Python
- `print("", "", sep="", end="")` = imprime un string; el valor asignado a sep separara los parametros con dicho valor, el valor asignado a end sera agregado al final del print
- `input("")` = pide un dato del usuario; "" es la instruccion que se imprime al pedirlo
- `python -m  venv nombreDelEntorno` = Crea un nuevo entorno (Instala un entorno virtual y le asigna un nombre).
- `pip install ipython` = Instala una dependencia de iPython (un shell interactivo que añade funcionalidades (Interprete mejor para python)).
- `python -m pip install -U pip` = Actualiza el pip (programa para gestionar las librerias).
- `python -m pip install colorama`= Instala una libreria para importar colores en la salida de la terminal.
- `ipython`= Activa el shell de ipython (un shell con mas funcionalidades y demas).


Activar el entorno con consola de Bash:
Se utiliza el source (activa un programa que se hizo con bash):
- Opción 1: Entramos en la carpeta del entorno, scripts, activate y listo! (.bat)
- Opción 2: source ruta relativa/absoluta del entorno, scripts, activate y listo! (.sh)
