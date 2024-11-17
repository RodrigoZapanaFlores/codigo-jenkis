# codigo-jenkis

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

# Hacer ejecutable el script build.sh y ejecutarlo
chmod +x build.sh
./build.sh

# Cambiar a la rama main
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

