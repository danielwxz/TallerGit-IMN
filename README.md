# TallerGit-IMN

Practica de uno de git y GitHub en el IMN

Fecha: 25 de marzo 2020

Taller virtual.

# Explicación del funcionamiento de git y GitHub

# Configuración inicial:
git config --global user.name "Daniel Soto"

git config --global user.email "<daniel.wxz@gmail.com>"

# Clonar un repositorio:
git clone https://github.com/danielwxz/TallerGit-IMN.git

# Comandos de información

git status

git log

git log --oneline

# Agregar documento:
touch Daniel.txt

git status

git add Daniel.txt

git status

git commit -m "Envio archivo Daniel.txt"

git log 

git log --oneline

# Para actualizar el repositorio desde GitHub:
git pull origin master

# Para actualizar el repositorio hacia GitHub:
git push origin master

# Creación de ramas:
git branch # para ver las existentes

git branch soto  # crea la rama soto

git branch cervantes  # crea la rama cervantes

# Cambiar de rama:

Vamos a crear varios documentos y carpetas

git checkout soto

touch archivosPy.txt

touch codigo.py

mkdir test 

touch test/programa.py

git checkout cervantes

touch archivosR.txt

touch codigo.R

mkdir test 

touch test/programa.R

# Actualizar la rama soto en el origen:

git push origin soto

# Asignar etiquetas a los commits:

git tag v1 codigo_commit

# Unir rama soto con cervantes:

git merge cervantes  # debo de estar en la rama soto

# Para revisar los commits:

git log

# Para ver todas las ramas del proyecto:

git branch --all

# Usar un commit del pasado:

git checkout codigo_commit

# Se pueden hacer cambios pero hay que guardarlos en una nueva rama:

git checkout -b nueva_rama

# Cambiar a la version etiquetada:

git checkout v1

# Buscar los cambios hechos

git diff numero_commit numero_commit

# Borrar una rama

git branch -d cervantes

# para descartar los últimos 3 commits:

git reset --hard HEAD~3

La diferencia entre checkout y reset es que en éste último se descartan las revisiones, mientras que con checkout se preservan.


## Bibliografía útil:

git --fast-version-control
https://git-scm.com/book/es/v2

git - la guía sencilla
https://rogerdudler.github.io/git-guide/index.es.html

Git y Github | Curso Práctico de Git y Github Desde Cero
https://www.youtube.com/watch?v=HiXLkL42tMU
