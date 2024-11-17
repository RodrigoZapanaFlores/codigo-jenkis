#!/bin/bash

# Verificar la ubicación actual
pwd

# Clonar el repositorio
echo "Clonando el repositorio..."
git clone https://RodrigoZapanaFlores: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@github.com/RodrigoZapanaFlores/TRabajoEntornos1.git

# Cambiar al directorio del repositorio clonado
cd TRabajoEntornos1

# Cambiar a la rama RodZap
echo "Cambiando a la rama RodZap..."
git checkout RodZap

# Hacer pull de los últimos cambios en la rama RodZap
echo "Haciendo pull de los últimos cambios en RodZap..."
git pull origin RodZap

# Listar los archivos en el directorio
echo "Archivos en el directorio TRabajoEntornos1:"
ls

# Asignar permisos de ejecución a todos los scripts necesarios
echo "Asignando permisos de ejecución a los scripts..."
chmod +x build.sh inicio.sh pagina1.sh pagina2.sh pagina3.sh cabecera.sh navegacion.sh pie.sh

# Ejecutar el script build.sh
echo "Ejecutando build.sh..."
./build.sh

# Verificar si los archivos HTML han sido generados correctamente
if [[ -e web/inicio.html && -e web/pagina1.html && -e web/pagina2.html && -e web/pagina3.html ]]; then
    echo "Archivos HTML generados correctamente."
else
    echo "Error: Uno o más archivos HTML no existen."
    exit 1
fi

# Copiar los archivos HTML generados desde la carpeta web
echo "Copiando archivos HTML a la raíz del repositorio..."
cp web/inicio.html .
cp web/pagina1.html .
cp web/pagina2.html .
cp web/pagina3.html

# Verificar que los archivos han sido copiados correctamente
if [[ -e inicio.html && -e pagina1.html && -e pagina2.html && -e pagina3.html ]]; then
    echo "Archivos HTML copiados correctamente a la raíz del repositorio."
else
    echo "Error: La copia de archivos HTML ha fallado."
    exit 1
fi

# Configurar el usuario de Git
echo "Configurando el usuario de Git..."
git config --global user.email "Rodrigozapanaflores@gmail.com"
git config --global user.name "RodrigoZapanaFlores"

# Cambiar a la rama main
echo "Cambiando a la rama main..."
git stash
git checkout main

# Hacer pull de los últimos cambios en la rama main
echo "Haciendo pull de los últimos cambios en main..."
git pull origin main

# Agregar los archivos al repositorio
echo "Agregando los archivos al repositorio..."
git add inicio.html pagina1.html pagina2.html pagina3.html

# Realizar el commit de los cambios
echo "Realizando el commit de los cambios..."
git commit -a -m "Desplegar sitio web en main"

# Subir los cambios a GitHub
echo "Subiendo los cambios a GitHub..."
git push -u https://RodrigoZapanaFlores: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@github.com/RodrigoZapanaFlores/TRabajoEntornos1.git main

# Finalización correcta del script
echo "Script completado correctamente."
exit 0
