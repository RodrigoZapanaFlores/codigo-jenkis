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


Lanzada por el usuario RodrigoZapanaflores
Running as SYSTEM
Ejecutando. en el espacio de trabajo /home/rzf/.jenkins/jobs/construirydesplegar/workspace
[WS-CLEANUP] Deleting project workspace...
[WS-CLEANUP] Deferred wipeout is used...
[WS-CLEANUP] Done
The recommended git tool is: NONE
using credential 9d658c61-9fb4-4957-a797-8936eb97aaed
Cloning the remote Git repository
Cloning repository https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
 > git init /home/rzf/.jenkins/jobs/construirydesplegar/workspace # timeout=10
Fetching upstream changes from https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
 > git --version # timeout=10
 > git --version # 'git version 2.45.2'
using GIT_ASKPASS to set credentials 
 > git fetch --tags --force --progress -- https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
 > git rev-parse refs/remotes/origin/RodZap^{commit} # timeout=10
Checking out Revision 6da879b950b84a33d9bb9fff690d8de800229fef (refs/remotes/origin/RodZap)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
Commit message: "files.sh"
 > git rev-list --no-walk 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
[workspace] $ /bin/bash /home/rzf/Descargas/apache-tomcat-10.1.33/temp/jenkins17718202020245151436.sh
/home/rzf/.jenkins/jobs/construirydesplegar/workspace
Clonando el repositorio...
Clonando en 'TRabajoEntornos1'...
Cambiando a la rama RodZap...
Cambiado a nueva rama 'RodZap'
rama 'RodZap' configurada para rastrear 'origin/RodZap'.
Haciendo pull de los últimos cambios en RodZap...
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            RodZap     -> FETCH_HEAD
Ya está actualizado.
Archivos en el directorio TRabajoEntornos1:
build.sh
cabecera.sh
inicio.sh
navegacion.sh
pagina1.sh
pagina2.sh
pagina3.sh
pie.sh
README.md
web
Asignando permisos de ejecución a los scripts...
Ejecutando build.sh...
se borra la web y se vuelve a crear
finalizado
El archivo no existe
--2024-11-17 04:46:26--  https://www.w3schools.com/w3css/4/w3.css
Resolviendo www.w3schools.com (www.w3schools.com)... 192.229.133.221
Conectando con www.w3schools.com (www.w3schools.com)[192.229.133.221]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 23427 (23K) [text/css]
Guardando como: ‘w3.css’

     0K .......... .......... ..                              100% 22,9K=1,0s

2024-11-17 04:46:29 (22,9 KB/s) - ‘w3.css’ guardado [23427/23427]

Archivos HTML generados correctamente.
Copiando archivos HTML a la raíz del repositorio...
Archivos HTML copiados correctamente a la raíz del repositorio.
Configurando el usuario de Git...
Limpiando el árbol de trabajo...
Directorio de trabajo y estado de índice WIP on RodZap: 6da879b files.sh guardados
Descartado refs/stash@{0} (0ddf04c08a703a7b16c7382d09b1552cb78790ee)
Cambiando a la rama main...
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
Haciendo pull de los últimos cambios en main...
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            main       -> FETCH_HEAD
Ya está actualizado.
Agregando los archivos al repositorio...
Realizando el commit de los cambios...
[main 9659d64] Desplegar sitio web en main
 4 files changed, 131 insertions(+)
 create mode 100644 inicio.html
 create mode 100644 pagina1.html
 create mode 100644 pagina2.html
 create mode 100644 pagina3.html
Subiendo los cambios a GitHub...
remote: Invalid username or password.
fatal: Autenticación falló para 'https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git/'
Script completado correctamente.
Finished: SUCCESS

