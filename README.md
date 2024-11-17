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
[workspace] $ /bin/bash /home/rzf/Descargas/apache-tomcat-10.1.33/temp/jenkins10634743950065564706.sh
/home/rzf/.jenkins/jobs/construirydesplegar/workspace
fatal: la ruta de destino 'TRabajoEntornos1' ya existe y no es un directorio vacío.
Ya en 'RodZap'
M	build.sh
A	inicio.html
A	pagina1.html
A	pagina2.html
A	pagina3.html
A	w3.css
M	web/inicio.html
M	web/pagina1.html
M	web/pagina2.html
M	web/pagina3.html
Tu rama está actualizada con 'origin/RodZap'.
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            RodZap     -> FETCH_HEAD
Ya está actualizado.
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
w3.css
web
se borra la web y se vuelve a crear
finalizado
El archivo no existe
--2024-11-17 02:49:34--  https://www.w3schools.com/w3css/4/w3.css
Resolviendo www.w3schools.com (www.w3schools.com)... 192.229.133.221
Conectando con www.w3schools.com (www.w3schools.com)[192.229.133.221]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 23427 (23K) [text/css]
Guardando como: ‘w3.css’

     0K .......... .......... ..                              100%  127K=0,2s

2024-11-17 02:49:36 (127 KB/s) - ‘w3.css’ guardado [23427/23427]

Directorio de trabajo y estado de índice WIP on RodZap: 6da879b files.sh guardados
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            main       -> FETCH_HEAD
   9c84fc5..1a2fcaa  main       -> origin/main
Actualizando 9c84fc5..1a2fcaa
Fast-forward
 README.md | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)
cp: no se puede efectuar `stat' sobre 'web/*': No existe el archivo o el directorio
En la rama main
Tu rama está actualizada con 'origin/main'.

nada para hacer commit, el árbol de trabajo está limpio
remote: Invalid username or password.
fatal: Autenticación falló para 'https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git/'
Finished: SUCCESS

