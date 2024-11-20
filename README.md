#!/bin/bash



# Clonar el repositorio (las credenciales ya están configuradas en Jenkins)
echo "Clonando el repositorio..."
git clone https://github.com/RodrigoZapanaFlores/TRabajoEntornos1.git

# Cambiar al directorio del repositorio clonado
cd Jenkins

# Ejecutar el script build.sh
echo "Ejecutando build.sh..."
./build.sh

# Cambiar a la rama main
echo "Cambiando a la rama main..."
git checkout main

# Hacer pull de los últimos cambios en la rama RodZap
echo "Haciendo pull de los últimos cambios en RodZap..."
git pull origin main

#copiar archivos html de la carpeta web hacia main
git checkout RodZap -- web/*.html

git add .

# Realizar el commit de los cambios
echo "Realizando el commit de los cambios..."
git commit -a -m "Desplegar sitio web en main"

# Subir los cambios a GitHub
echo "Subiendo los cambios a GitHub..."
git push origin main

# Finalización correcta del script
echo "Script completado correctamente."
exit 0
