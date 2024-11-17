#!/bin/bash

# Verificar la ubicación actual
pwd

# Clonar el repositorio
git clone https://RodrigoZapanaFlores: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@github.com/RodrigoZapanaFlores/TRabajoEntornos1.git

# Cambiar al directorio del repositorio clonado
cd TRabajoEntornos1

# Cambiar a la rama RodZap
git checkout RodZap

# Hacer pull de los últimos cambios en la rama RodZap
git pull origin RodZap

# Listar los archivos en el directorio
ls

# Asignar permisos de ejecución a todos los scripts necesarios
chmod +x build.sh inicio.sh pagina1.sh pagina2.sh pagina3.sh cabecera.sh navegacion.sh pie.sh

# Ejecutar el script build.sh
./build.sh

# Configurar el usuario de Git
git config --global user.email "Rodrigozapanaflores@gmail.com"
git config --global user.name "RodrigoZapanaFlores"

# Cambiar a la rama main
git stash
git checkout main

# Hacer pull de los últimos cambios en la rama main
git pull origin main

# Copiar los archivos HTML generados desde la carpeta web
cp -r web/* .

# Agregar los archivos al repositorio
git add .

# Realizar el commit de los cambios
git commit -a -m "Desplegar sitio web en main"

# Subir los cambios a GitHub
git push -u https://RodrigoZapanaFlores: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@github.com/RodrigoZapanaFlores/TRabajoEntornos1.git main

# Finalización correcta del script
exit 0

