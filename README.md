# git-github-julian

## ¿Porque utilizar Git?

Git nos permite tener un control de versiones es decir tener un registro
de todos los cambios que hagamos en 1 o mas archivos

### ¿que es el staging y los repositorios?

El staging es un espacio en memoria ram, es donde se guardan los cambios
luego de haber enviado los cambios a staging, cuando se le da commit se
envia al repositorio

### Entorno de desarrollo personal

1. Driectorio de trabajo
2. Preparacion o Staging
3. Repositorio local
4. Repositorio remoto

### Ramas

Las ramas son formas de hacer cambios sin afectar el estado de la rama principal

## Llaves publicas y privadas

cifrado asimetrico de un solo camino, las llaves estan vinculadas lo que se cifre con la llave publica solo lo puede abrir la llave privada

### configuracion llave publica y privada

En el entorno local se crea las dos llaves y se le envia la llave publica a GitHub y se conecta por un protocolo nuevo, github enviara automaticamente otra llave publica para la comunicación

- carpeta home
- ssh-keygen -t rsa -b 4096 -C correo

## tags y versiones

Un tag sirve para dar referencia a una parte del codigo dividiendolo por lo general en versiones para llevar un control de avances en cada etapa

## Contribuyendo a un repositorio Fork

Tomar una copia del estado actual del proyexto y hacerlo propio

## Guardar cambios en memoria

Sirve cuando se quiere hacer cambios de un committ anterior pero sin guardar los cambios actuales (RECOMENDADO)

## Comandos y configuración

### Configuración de git

- git config
- git config --list
- git config --global user.name nombre
- git config --global user.email correo

### Comandos generales

- git init: Iniciar un repositorio de git en local
- git status: ver el estado de los archivos
- git add Archivo: agregar los cambios de un archivo
- git add .: agragar todos los cambios
- git restore --staged file: quitar de staged
- git rm --cached file: qitar de registro
- git add commit -m Mensaje: guardar cambios con mensaje
- git log: registro de commits
- git log --stat: ver cambios especificos a partir del commit
- git log --all: muestra todo el historial
- git log --all --graph --decorate --oneline: muestra todo el historial comprimido graficamente
- git show archivo: mostrar cambios
- git diff indicador indicador: comparar versiones
- git reset --soft: Se devuelven los cambios pero lo que esta en staged sigue
- git reset --hard: se devuelven los cambios permanentemente
- git checkout indicador archivo: ver un archivo en estado original en un commit
- git checkout master archivo: actualizar a lo de master
- git branch nombre: crear rama
- git checkout rama: cambiar de rama
- git merge: unir ramas
- git remote add origin link: agregar repositorio remoto
- git remote -v: informacion del repositorio remoto
- git push origin main: enviar cambios
- git merge rama: unir ramas
- git pull origin main: traer los cambios del repositorio remoto
- git remore set-url origin linkSSH
- git fetch
- git tag -a v0.1 -m "mensaje" indicador: crear un nuevo tag
- git tag: ver los tags
- git show-ref --tags: ver a que parte pertenece cada tag
- git push origin --tags: enviar los tags creados
- git tag -d tag: borrar un tag
- git push origin : refs/tags/(tag): Borrar el tag en github antes borrado en local
- git clone (link): clonar repositorio
- git stash: guardar cambios en memoria
- git stash list: lista de los cambios en memoria
- git stash pop: Agregar los cambios que estan en memoria
- git stash drop: Eliminar los cambios que estan en memoria
- git clean --dry-run: simula lo que va a borrar
- git clean -f: borra los datos clonados
- git cherry-pick (indicador commit): traer commits viejos de una rama
- git commit --amend: agregar cambios al ultimo commit
- git reflog: se ve todo el registro
- git reset --HARD indicador: resetear a un commit anterior, si se a dañado algo
- git grep (palabra): buscar una plabra en los archivos
- git grep -n (palabra): buscar una plabra en los archivos en que linea
- git grep -c (palabra): buscar una plabra en los archivos cuantas veces
- git log -S: buscar en los commits
- git shortlog: muestra commits por persona
- git shortlog -sn --all: cuantos commits a hecho cada persona
- git shortlog -sn --all --no-merges: cuantos commits a hecho cada persona
- git blame: quien hizo que
- git comando --help: como funciona un comando
- git branch -r: ramas remotas
- git branch -a: todas las ramas
