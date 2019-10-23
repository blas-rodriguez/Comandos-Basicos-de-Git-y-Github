# Comandos Baicos para git y Github 
## ls -al
listar directorio actual

## mkdir: "proyecto1"
crear la carpeta proyecto1
## touch "vacío.txt"
crear un archivo vacío.txt
## cat "vacío.txt"
Sirve para  abrir el archivo vacio.txt
## history
Sirve para mostrar un historial de comandos
## !72 
Con el signo ! y el numero de linea sirve para invocar un comando seleccionado
## git rm "vacio.txt"
Sirve para borrar un archivo:
## git rm -rf
Sirve para la eliminación recursiva de un archivo
## git rm -- help
Sirve para ver como funciona la funcion rm
## git rm --cached archivo
Esto simplemente elimina el seguimiento de un archivo (el estado en que se encuentra un archivo una vez agregado, es decir, git add [file] )
## git reset HEAD archivo
Esto simplemente continúa haciendo un seguimiento de los cambios en el file, pero lo colocará de nuevo en el área "sin explorar".
## git init 
Sirve para inicializar el repositorio
## git add 
Sirve para agregar al staging  esperando a que lo envies al repositorio sin rastrear
## git add . 
agrega todos los archivos del directorio
## git commit -m "mensaje" 
Sirve para subir los cambios al  repositorio
Cada vez que hago un commit estoy realizando una versión. que se lo envía a la rama seleccionada.
## git checkout rama
traer un archivo osea traer los cambios realizados
## code
 es para abrir el editor de texto code visual studio
## git status 
Sirve  para ver el estado de mi proyecto para ver si algo se modificó o algo quedó en el stash
---configurar quienes somos nosotros---
## git config --list 
ver configuraciones de git
## git config --list --show-origin 
Sirve para casos avanzado
## git config --global user.name "nombre"
## git config --global user.email "correo@hotmail.com"
## code archivo.txt 
Sirve para editar el archivo.txt
## git log archivo.txt 
Sirve para ver el historial de un archivo
## git show arhivos.txt 
Sirve para mostrar los cambios de un archivo
## esc+shif+z+z 
Sirve para salir de la consola de mensajes
## git diff numero numero 
Sirve para ver la diferencia entre una versión y otra version)
## git reset numero 
Sirve para volver a la versión anterior
## git reset  hard 
todo vuele a la version anterior
## git log --stat 
es para ver la cantidad de bit en archivos
## git  log --all 
muestra todos los commit que se realizaron
## git log --all --graph 
muestra gráficamente los commit que se realizaron
## git log --all --graph --decorate --oneline
te muestra comprimido en una línea los commit que se realizaron
## alias arbolito=”git log --all --graph --decorate --oneline” 
lo que hacemos con el comando alias solo asignamos a una variable en este caso arbolito toda una funcion o comando como en este caso el comando anterior y cada vez que necesites llamar a ese comando solo ejecutas la palabra arbolito
## git tag -a v0.1 -m “esta es una verecion ” 01212425 
con este comando le asignamos un tag a una versión de los commit en este caso le asigno el tag v0.1 al ash 01212425
## git tag 
listar los tag
## git show-ref --tags 
listar los tags más detallados
## git push origin --tags 
empujamos solo los tag al repositorio remoto
## git tag -d v0.1 
borro el tag v0.1 en el repositorio local
## git push origin :ref/tags/v0.1 
borro en el repositorio remoto el tag v0.1
## git show-branch 
muestra el historial de las ramas
## git show -branch --all 
muestra el historial de las ramas más detallado
## gitk 
muestra un software que especifica los cambios que fuiste realizando en
servidor remoto
## git clone url “”
trae una copia del servidor a mi maquina
## git push rama rama
subir todo al servidor remoto
## git fetch rama rama
trae a la máquina pero no cambia nada hasta que se haga un git merge
## git merge rama 
Sirve para unir una rama en el la rama seleccionada
## git pull  rama rama
traer todo del repositorio remoto a la rama que estamos seleccionada
## git commit -am "mensaje" 
realiza el add y commit a la rama seleccionada
## git branch "cabecera" 
crea una rama 
## git checkout cabecera 
me muevo a la rama que quiera en este caso cabecera
## git branch 
es para ver en qué rama estas
## git merge cabecera 
es el que va a unir la rama cabecera dentro de la rama master. solo si tenemos seleccionada la rama master
## git remote add origin ""
Sirve para agregar un repositorio remoto
git remote add (para agregar un repositorio remoto)
## git remote 
Nos muestra la dirección que estamos en este caso el origen
## git remote -v 
nos muestra los lugares de donde haremos un fetch(traer) y push(llevar).
## git push origin master
Sirve para subir a origin (repositorio remoto) la rama master
## git pull origin master 
Sirve para traer lo ultimo que hay en repositorio remoto a la rama master
## git push origin cabecera 
Sirve para subir a origin todo de lo que hay en rama cabecera
## git clone url “”
clona solo el repositorio especificado en la carpeta seleccionada
## ssh-keygen - t rsa -b 4096 -C "correo@gmail.com" 
creamos una llave pública y privada
## eval $(ssh-agent -s) 
es para activar la conexión con github con llaves
## ssh-add path/id_rsa 
agregamos la llave con la que vamos a hacer la conexión
## git remote -v 
Sirve para ver las url de nuestro repositorio
## git remote set-url origin 
cambia la url de origin. podemos especificar si queremos cambiar para fech o push
## git remote add origin “url”
en caso de que no tengas asignada el origin
## git pull origin master --allow-unrelated-histories 
en caso que no quiera hacer un push
## git pull rama rama
es para traer cosas del repositorio
## git pull origin master 
es para traer y reemplazar origin en master
## git push origin master 
empujamos el master al repositorio remoto origin
## git log --all --graph 
es para ver los log detalladamente o gráficamente
## git log --all -- graph --decorate --oneline
ver más detalladamente los log
## git tag -a v0.1 -m "resultado de las primeras clases " f9300fa
esto es para hacer un tag en la versión de un proyecto en este caso 
vamos a meter ese mensaje en la versión f9300fa
## git tag 
muestra todos los tag
## gi show-ref --tags 
es para ver el ash de un tag. osea a donde está apuntado
## git push origin --tags
Sirve para enviar los tags al repositorio remoto
## git tag -d dormido 
Sirve para borrar un tag en nuestra maquina
## git push origin :refs/tags/dormir
borra el tag del repositorio remoto
## git show-branch 
muestra las ramas del proyecto
## git show-branch --all 
muestra todas las ramas del proyecto pero más detallado
## gitk 
te muestra un soft con las ramas
## git clone url 
es para traer un proyecto público o privado. nada más que en el privado vas a tener que poner la contraseña
después de hecha la modificacion.hacemos un commit
luego un git pull origin master
## git push origin master
primero agregamos desde github el colaborador desde setting
## pull-requests.
se hace este metodo para subir una rama o modificación del proyecto . pero lo especial que tiene es que si no sos administrador del proyecto. lo que realizas es una pregunta o comentario al administrador para que puedas hacer evaluar las operaciones que quieren hacer 
se puede agregar a  colaboradores para que verifiquen ese pullrequests y lo aprueben
## fork (tenedor)
solo se puede hacer con proyectos públicos. la idea es hacer un clone del repo. osea se hacer una copia en tu repositorio y se lo trabaja desde ahí. Pero solo en tu cuenta. no lo podras subir a master de quien lo creo amenos que seas colaborador. o amenos que realices un pullrequests.
otro tema que pasa. Es que como vs copiaste la rama principal del proyecto original. vs siempre tenes una version vieja del proyecto por ende tenes que crear una rama nueva y agregar en “remote add” la dirección que apunte directamente al repositorio del proyecto principal. lo que hace esto es que siempre vas a tener una rama actualizada y vos podes trabajar con 2 ramas a la vez en una vas haciendo un pull para estar actualizado y en otra haces cambios para luego hacer un pullrequests.
## deployment 
en esta parte lo que realizamos es utilizar la metodología de git pull  para usarla directamente en producción y así poder ejecutar nuestro programa
## gitignore
es un archivo de git que sirve para ignorar archivos que quieres que se suban a github
## readme.md
es un html que se explica sobre el proyecto que estás viendo. osea como una presentación.
una buena pagina para editar tu md es : https://pandao.github.io/editor.md/en.html 
## github pagues
es un servicio de github en el cual puedes publicar tus proyectos públicos
https://pages.github.com/ 
## rebase
Es una mala práctica. lo que se hace es traer una rama y ponerla directamente sobre la rama principal
me posiciono sobre la rama principal master y hago lo siguiente:
git rebase rama-que-quiero-pegar-en-el-master
y tmb se tiene que hacer al revés. pero primero en la rama que no es la master
## git stash 
sirve para no guardar los cambios antes del commit. osea si modifiqué algún archivo pero no quiero commitearlo puedo apretar git stash y volver para no hacer el commit
## git stash list 
nos muestra en detalle el stash que no se guardó
## git stash pop
muestra el stash que no se guardó 
## git stash branch inglis-version
lo que hacemos es pasar todo lo que tenemos en stash a la rama ”inglis-version” y automáticamente nos pasamos a la rama creada
## git stash drop
sirve para borrar el stash que no se commitio
en síntesis sirve para salvar un stash antes del commit
## git clean --dry-run
sirve para que me muestra que son las cosas que quiere limpiar. osea borrar. cuando no queremos que se guarde en el commit podemos borrar todo lo que está de más 
## git clean -f
sirve para borrar o limpiar los archivos listados con el comando anterior
las carpetas no las va a borrar debido a que no rastrea las carpetas sino los archivos. En ese caso se tendría que borrar manualmente la carpeta.tampoco borra los archivos que estén en gitignore.
## git cherry-pick
sirve para hacer un merge de un punto de la rama con otro punto de otra rama o la misma.
osea sirve para pegar cosas de otros puntos de ramas a la rama que yo quiero
## git amend (remendar)
git commit --amend “texto”
sirve para los cambios que hice los  va a pegar al commit anterior. no va a crear uno nuevo.
es como que modifica al commit anterior pero no crea un commit nuevo.
## git reflog
sirve para ver un historial de todos los head que hicimos ya sea que estén borrados o con merge o cualquier cosa. con este comando podemos entender que paso
## git reset --soft
sirve para volver de version pero te guarda lo que tengas en stash
## git reset --hard ash
sirve para borrar todo el commit.
## git reset head04
te vuelve al commit especificado “” (este ash lo sacamos desde git reflog)
## git grep -n palabra
sirve para buscar palabras pero dentro de tu proyecto traqueado por git
## git grep -c “palab”
sirve para contar cuantas veces use una palabra
## git log -S “palabra”
sirve para buscar una palabra dentro de los commit de git.
## git shortlog
te muestra un log por la cantidad de tus miembros de tu equipo
## git shortlog -sn
muestra la cantidad de integrantes que colaboran al proyecto
## git shortlog -sn --all
muestra la cantidad de commit que realizaron los usuarios del proyecto
## git shortlog -sn --all --no-merges
muestra la cantidad de commit que realizaron los colaboradores del proyecto excluyendo los merges.
## git config --global alias.stats “git shortlog -sn --all --no-merges”
crea una especie de función. osea me crea la palabra stats en el comando que esta entre comillas (git stats)
## git blame “nombre del archivo”
donde podemos ver quien trabajó en ese archivo 
## git blame -c “archivo”
muestra lo mismo que lo anterior pero más ordenado
git blame --help
nos abre en el navegador de cómo funciona el comando que seleccionamos
blame sirve para ver quien modifico un archivo por última vez
## git blame “archivo” -L35-60 -c
sirve para mostrar que pasó en esas líneas ordenadamente
## git branch -r
sirve para ver las ramas remotas
## git branch -a
sirve para ver todas las ramas
