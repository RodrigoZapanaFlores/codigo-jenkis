Lanzada por el usuario RodrigoZapanaflores
Running as SYSTEM
Ejecutando. en el espacio de trabajo /home/rzf/.jenkins/jobs/construirydesplegar/workspace
The recommended git tool is: NONE
using credential 9d658c61-9fb4-4957-a797-8936eb97aaed
 > git rev-parse --resolve-git-dir /home/rzf/.jenkins/jobs/construirydesplegar/workspace/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git # timeout=10
Fetching upstream changes from https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
 > git --version # timeout=10
 > git --version # 'git version 2.45.2'
using GIT_ASKPASS to set credentials 
 > git fetch --tags --force --progress -- https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/RodZap^{commit} # timeout=10
Checking out Revision 6da879b950b84a33d9bb9fff690d8de800229fef (refs/remotes/origin/RodZap)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
Commit message: "files.sh"
 > git rev-list --no-walk 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
[workspace] $ /bin/bash /home/rzf/Descargas/apache-tomcat-10.1.33/temp/jenkins7335570827916442974.sh
/home/rzf/.jenkins/jobs/construirydesplegar/workspace
Clonando el repositorio...
fatal: la ruta de destino 'TRabajoEntornos1' ya existe y no es un directorio vacío.
Cambiando a la rama RodZap...
Cambiado a rama 'RodZap'
Tu rama está adelantada a 'origin/RodZap' por 1 commit.
  (usa "git push" para publicar tus commits locales)
Haciendo pull de los últimos cambios en RodZap...
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            RodZap     -> FETCH_HEAD
Ya está actualizado.
Archivos en el directorio TRabajoEntornos1:
build.sh
cabecera.sh
inicio.html
inicio.sh
navegacion.sh
pagina1.html
pagina1.sh
pagina2.html
pagina2.sh
pagina3.html
pagina3.sh
pie.sh
README.md
web
Asignando permisos de ejecución a los scripts...
Ejecutando build.sh...
se borra la web y se vuelve a crear
finalizado
El archivo no existe
--2024-11-17 04:10:37--  https://www.w3schools.com/w3css/4/w3.css
Resolviendo www.w3schools.com (www.w3schools.com)... 192.229.133.221
Conectando con www.w3schools.com (www.w3schools.com)[192.229.133.221]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 23427 (23K) [text/css]
Guardando como: ‘w3.css’

     0K .......... .......... ..                              100% 45,4K=0,5s

2024-11-17 04:10:40 (45,4 KB/s) - ‘w3.css’ guardado [23427/23427]

Archivos HTML generados correctamente.
Copiando archivos HTML a la raíz del repositorio...
Archivos HTML copiados correctamente a la raíz del repositorio.
Configurando el usuario de Git...
Limpiando el árbol de trabajo...
Directorio de trabajo y estado de índice WIP on RodZap: 6fc55d8 Desplegar sitio web en main guardados
Descartado refs/stash@{0} (7969430d47f40e841a2ed04e8a0a69b7b9c2a64d)
Cambiando a la rama main...
Cambiado a rama 'main'
Tu rama está adelantada a 'origin/main' por 1 commit.
  (usa "git push" para publicar tus commits locales)
Haciendo pull de los últimos cambios en main...
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            main       -> FETCH_HEAD
La rama actual main está actualizada.
Agregando los archivos al repositorio...
Realizando el commit de los cambios...
En la rama main
Tu rama está adelantada a 'origin/main' por 1 commit.
  (usa "git push" para publicar tus commits locales)

nada para hacer commit, el árbol de trabajo está limpio
Subiendo los cambios a GitHub...
remote: Invalid username or password.
fatal: Autenticación falló para 'https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git/'
Build step 'Ejecutar linea de comandos (shell)' marked build as failure
Finished: FAILURE
