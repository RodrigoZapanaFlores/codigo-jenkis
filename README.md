Lanzada por el usuario RodrigoZapanaflores

Running as SYSTEM
Ejecutando. en el espacio de trabajo /home/rzf/.jenkins/jobs/construirydesplegar/workspace
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /home/rzf/.jenkins/jobs/construirydesplegar/workspace/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git # timeout=10
Fetching upstream changes from https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
 > git --version # timeout=10
 > git --version # 'git version 2.45.2'
 > git fetch --tags --force --progress -- https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/RodZap^{commit} # timeout=10
Checking out Revision 6da879b950b84a33d9bb9fff690d8de800229fef (refs/remotes/origin/RodZap)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
Commit message: "files.sh"
 > git rev-list --no-walk 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
[workspace] $ /bin/bash /home/rzf/Descargas/apache-tomcat-10.1.33/temp/jenkins7647430482096415356.sh
/home/rzf/.jenkins/jobs/construirydesplegar/workspace
Clonando el repositorio...
fatal: la ruta de destino 'TRabajoEntornos1' ya existe y no es un directorio vacío.
Cambiando a la rama RodZap...
Cambiado a rama 'RodZap'
Tu rama está actualizada con 'origin/RodZap'.
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
--2024-11-17 03:33:43--  https://www.w3schools.com/w3css/4/w3.css
Resolviendo www.w3schools.com (www.w3schools.com)... 192.229.133.221
Conectando con www.w3schools.com (www.w3schools.com)[192.229.133.221]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 23427 (23K) [text/css]
Guardando como: ‘w3.css’

     0K .......... .......... ..                              100% 15,2K=1,5s

2024-11-17 03:33:47 (15,2 KB/s) - ‘w3.css’ guardado [23427/23427]

Archivos HTML generados correctamente.
Copiando archivos HTML a la raíz del repositorio...
Archivos HTML copiados correctamente a la raíz del repositorio.
Configurando el usuario de Git...
Cambiando a la rama main...
Directorio de trabajo y estado de índice WIP on RodZap: 6da879b files.sh guardados
error: Los siguientes archivos sin seguimiento en el árbol de trabajo serán sobrescritos al actualizar el árbol de trabajo:
	inicio.html
	pagina1.html
	pagina2.html
	pagina3.html
Por favor, muévelos o elimínalos antes de cambiar de rama.
Abortando
Haciendo pull de los últimos cambios en main...
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            main       -> FETCH_HEAD
hint: Las ramas se han divergido y hay que especificar cómo reconciliarlas.
hint: Se puede hacerlo ejecutando uno de los comandos siguiente antes del
hint: próximo pull:
hint:
hint:   git config pull.rebase false  # fusionar
hint:   git config pull.rebase true   # rebasar
hint:   git config pull.ff only       # solo avance rápido
hint:
hint: Se puede reemplazar "git config" con "git config --global" para aplicar
hint: la preferencia en todos los repositorios. También se puede pasar
hint: --rebase, --no-rebase o --ff-only en el comando para sobrescribir la
hint: configuración por defecto en cada invocación.
fatal: Necesita especificar cómo reconciliar las ramas divergentes.
Agregando los archivos al repositorio...
Realizando el commit de los cambios...
[RodZap 6fc55d8] Desplegar sitio web en main
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
