# codigo-jenkis

#!/bin/bash

# Verificar la ubicación actual
pwd

# Verificar si el repositorio ya ha sido clonado
if [[ -d TRabajoEntornos1 ]] ; then
    echo "El repositorio ya ha sido clonado"
    cd TRabajoEntornos1
else
    echo "El repositorio no ha sido clonado, clonando ahora..."
    git clone https://RodrigoZapanaFlores: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@github.com/RodrigoZapanaFlores/TRabajoEntornos1.git
    if [[ $? -ne 0 ]] ; then
        echo "La clonación del repositorio ha fallado"
        exit 1
    fi
    cd TRabajoEntornos1
fi

# Verificar la rama actual
git checkout RodZap

# Listar los archivos en el directorio
ls

# Verificar si build.sh existe y ejecutarlo
if [[ -e build.sh ]] ; then
    echo "El archivo build.sh existe, ejecutándolo..."
else
    echo "El archivo build.sh no existe, deteniendo la ejecución."
    exit 1
fi

# Hacer ejecutable el script build.sh
chmod +x build.sh

# Construir el sitio web
./build.sh

# Cambiar a la rama main
git checkout main

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
