Lanzada por el usuario RodrigoZapanaflores
Running as SYSTEM
Ejecutando. en el espacio de trabajo /home/rzf/.jenkins/jobs/construirydesplegar/workspace
The recommended git tool is: NONE
No credentials specified
Cloning the remote Git repository
Cloning repository https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
 > git init /home/rzf/.jenkins/jobs/construirydesplegar/workspace # timeout=10
Fetching upstream changes from https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
 > git --version # timeout=10
 > git --version # 'git version 2.45.2'
 > git fetch --tags --force --progress -- https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
 > git rev-parse refs/remotes/origin/RodZap^{commit} # timeout=10
Checking out Revision 6da879b950b84a33d9bb9fff690d8de800229fef (refs/remotes/origin/RodZap)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 6da879b950b84a33d9bb9fff690d8de800229fef # timeout=10
Commit message: "files.sh"
First time build. Skipping changelog.
[workspace] $ /bin/bash /home/rzf/Descargas/apache-tomcat-10.1.33/temp/jenkins17843929867053708440.sh
/home/rzf/.jenkins/jobs/construirydesplegar/workspace
Clonando en 'TRabajoEntornos1'...
Cambiado a nueva rama 'RodZap'
rama 'RodZap' configurada para rastrear 'origin/RodZap'.
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            RodZap     -> FETCH_HEAD
Ya está actualizado.
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
se borra la web y se vuelve a crear
./build.sh: línea 7: ./inicio.sh: Permiso denegado
./build.sh: línea 8: ./pagina1.sh: Permiso denegado
./build.sh: línea 9: ./pagina2.sh: Permiso denegado
./build.sh: línea 10: ./pagina3.sh: Permiso denegado
finalizado
El archivo no existe
--2024-11-17 02:20:11--  https://www.w3schools.com/w3css/4/w3.css
Resolviendo www.w3schools.com (www.w3schools.com)... 192.229.133.221
Conectando con www.w3schools.com (www.w3schools.com)[192.229.133.221]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 23427 (23K) [text/css]
Guardando como: ‘w3.css’

     0K .......... .......... ..                              100% 15,3K=1,5s

2024-11-17 02:20:15 (15,3 KB/s) - ‘w3.css’ guardado [23427/23427]

error: Los cambios locales de los siguientes archivos serán sobrescritos por checkout:
	build.sh
	web/inicio.html
	web/pagina1.html
	web/pagina2.html
	web/pagina3.html
Por favor realice un commit con los cambios o un stash antes de cambiar ramas.
Abortando
Desde https://github.com/RodrigoZapanaFlores/TRabajoEntornos1
 * branch            main       -> FETCH_HEAD
Ya está actualizado.
Identidad del autor desconocido

*** Por favor cuéntame quién eres.

Ejecuta

  git config --global user.email "you@example.com"
  git config --global user.name "Tu Nombre"

para configurar la identidad por defecto de tu cuenta.
Omite --global para configurar tu identidad solo en este repositorio.

fatal: no es posible auto-detectar la dirección de correo (se obtuvo 'rzf@rzf-VirtualBox.(none)')
remote: Invalid username or password.
fatal: Autenticación falló para 'https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git/'
Finished: SUCCESS

