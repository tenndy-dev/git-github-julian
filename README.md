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

## Comandos y configuración

### Configuración de git

- git config
- git config --list
- git config --global user.name "<nombre>"
- git config --global user.email "<correo>"

### Comandos generales

- git init: Iniciar un repositorio de git en local
- git status: ver el estado de los archivos
- git add <Archivo>: agregar los cambios de un archivo
- git add .: agragar todos los cambios
- git restore --staged <file>: quitar de staged
- git rm --cached <file>: qitar de registro
- git add commit -m "<Mensaje>": guardar cambios con mensaje
- git log: registro de commits
- git log --stat: ver cambios especificos a partir del commit
- git show <archivo>: mostrar cambios
- git diff <indicador> <indicador>: comparar versiones
- git reset --soft: Se devuelven los cambios pero lo que esta en staged sigue
- git reset --hard: se devuelven los cambios permanentemente
- git checkout <indicador> <archivo>: ver un archivo en estado original en un commit
- git checkout <master> <archivo>: actualizar a lo de master
- git push
- git fetch
- git merge
- git pull
