# Trabajo Individual 
Name = Viraca Pacolla Joel Carlos
Celular = 64866872
Email = joelviraca@gmail.com

##clase 1
### que es git?
Es un sistema de Control de Versiones Distribuido(CVS).
permite guardar archivos y las versiones guardandolos del tiempo de manera local
### como nacio Git?
Linus Torvalds
un colaborador externo cuando habia una colaboracion externa lo hacie mediante Email, para poner su codigo o no hacerlo de manera manual uno por uno es laborioso.
En contraste para en conjunto con su comunidad usando BitKeeper, la regla de los colaboradores de no usar otro codigo en otro repositorio, pero la regla no fue cumplida quitandole el acceso a linus Torvalds, creando asi Git 
###como instalamos git?
Para su presente instalacion se hara lo siguiente :
En Windows

La forma más fácil:

Ve a la web oficial:
👉 https://git-scm.com/
Descarga el instalador
Ejecuta el .exe
Dale Next a todo (la configuración por defecto funciona bien)

Esto te instala:

Git

En maCos:
En macOS
Opción 1 (la más fácil)

Abre Terminal y escribe:

git --version

Si no lo tienes, macOS te pedirá instalarlo automáticamente.
En Linux: 
Ubuntu / Debian
sudo apt update
sudo apt install git
Fedora
sudo dnf install git
Arch Linux
sudo pacman -S git
###Comandos vistos
git config --global user.name "Joel carlos viraca pacolla" #crea nombre de usuario
git config --global user.email "joelviraca@amil.com" #crea email para la creacion
git config --global --list #listado de todas lo creado
git init
git add README.md
git status
git commit

##Clase 2
###estados de Git
tenemor primero lo que son los estados de git
Directorio de Trabajo, Stage Area, Reporitorio local
El directorio de Trabajo se basa en crear modificar o eliminar ficheros si es necesario hacerlo, si quiere guardar prepara cambios.
Stage Area es el area de espera lo que se quiere guardar, confirmando loa cambios antes de subir un commit
Repositorio local es cuando tienes historial teniendo ya ID que ya forman parte de la historia de cambios
###Directorio de Trabajo modificado
Es una carpeta comun donde git cataloga en dos estados: Untracked, Modified
Untracked: que no tiene seguimiento esta siendo observado a traves de git status cuyo archivo no tiene una version antigua.
Modified: sucede cuando git ya cumple con una version antigua ya esta siendo registrado sabiendo cuando modificaste, eliminaste o cambiaste de nombre dicho archivo
si antes de haber ejecutado .gitignore pasa automaticamente a uno de los dos estados 
###comandos
git status: observa el estado del archivo ya sea modifocado o eliminado o creado
git restore <archivo> Archivo modificado vuelva a su estado original
.gitignore: git no ve el archivo que creaste
git add <archivo>: adrega el archivo este archivo agrega uno por uno
git add .: agrega todos los archivos que esten obsevados por git, este es un comando mas que todo utilizado en git para actualizar las ramas o archivos nuevos cuando trabajas en un git en escritorio
git restore --staged <archivo> sacar un archivo stage area para volver al estado aterior
###Repositorio Local
git commit -m "mensaje" : se crea un commit para que el repositorio quesea creado garde todos los cambios que estan en staged y pasen a ser parte del historial
git reset --soft HEAD~1 : desacer el ultimo commit del comando

###Buenas Practicas
los commits son modifiacones pequenias mejoras haceidno cambios a codigo fuente, es mejor hacer commits pequenios que graban tu progreso con iteraciones pequenias 
los commits deben de tener lo siguiente que contengan verbos usando palabras claves para su revision
por ejemplo:
verbos imperativos(add, change, Fix, Remove)
El uso de , o . a la hora de usar commits ya que cada caracter cuenta a la hora e escribir un cambio asi que es mejor no usarlo :
Escribir buenos commits:
-usar como maximo 50 caracteres
-usar prefijos para los commits para hacerlos mas semanticos => git commit -m "feat:Add new search feature"
###Escribir buenos commits
Prefijos:
feat: para una nueva característica para el usuario.
fix: para un bug que afecta al usuario.
perf: para cambios que mejoran el rendimiento del sitio.
build: para cambios en el sistema de build, tareas de despliegue o instalación.
ci: para cambios en la integración continua.
docs: para cambios en la documentación.
refactor: para refactorización del código como cambios de nombre de variables o funciones.
style: para cambios de formato, tabulaciones, espacios o puntos y coma, etc; no afectan al
usuario.
test: para tests o refactorización de uno ya existente.
Si es necesario es mejor aniadir todo el contexto que sea necesario en el cuerpo del commit.

 
