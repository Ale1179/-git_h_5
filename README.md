# HACK - GIT 5

##### ### ## ENVIAR UNA RAMA REMOTA.

-Crear un nuevo repositorio en github nombre: git_h_5

-Crear un repositorio local

-git init

-Registrar el repositorio remoto con tú repositorio local

-git remote add origin (pegar_la_ruta_del_repositorio_local)
Verificamos la ruta remota

-git remote -v

-Elaborar un archivo con el nombre de "inicio.txt"

-touch inicio.txt

Incorporar "inicio.txt" para un commit
-git add .

-git commit -m "feat: add inicio.txt"

-git push -u origin master

-Ahora creamos una rama remota llamada "feature/actividades" y le adjuntamos 2 archivos "foo.txt" y "bar.txt"
touch foo.txt
touch bar.txt

Producimos el commit, aunque antes creamos la rama y nos vamos a ella, para desde ahí hacer el commit

-git branch feature/actividades

-git switch feature/actividades

-git add .

-git status

-git commit -m "feat: add 2 files foo.txt and bar.txt"

Aunque nos indican que falta crear otro archivo llamado "qux.txt" al commit

touch qux.txt

-git add .

-git commit --amend -m "feat: add 3 files foo.txt, bar.txt, qux.txt"

Enviamos la rama remota

-git push -u origin feature/actividades

-Verificar en el repositorio remoto que se envio la rama.

Regresamos a master

-git switch master

-Creamos una nueva rama llamada "hotfix/registroDeUsuario" por una emergencia, en ella crear un archivo llamado "registro_de_usuarios.txt"

git branch hotfix/registroDeUsuario
git switch hotfix/registroDeUsuario

-touch registro_de_usuarios.txt

-git add . 

-git commit -m "hotfix: add registro_de_usuarios.txt"

-Enviamos la rama "hotfix/registroDeUsuario" al repositorio remoto y revisamos el repositorio remoto

-git push -u origin hotfix/registroDeUsuario

-Retornamos a master y analizamos todas las las ramas locales y remotas

-git switch master

-git branch -a

-Eliminamos la rama remota "feature/actividades" y revisamos el repositorio

-git switch master

-git push origin --delete feature/actividades

Hacemos una mirada a las ramas

-git branch -a





##  FIN.

