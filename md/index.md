---
hide:
  - navigation
  - toc
  - footer
---

## Resumen de Comandos git
![git](img/git_image.png)

1. **git init**.- inicializa un repositorio.
2. **git add**.- añade elementos de la copia de trabajo (working) en el control de versiones (área de preparado o staging).
    - **git add**.- Añade todos los elementos de la copia de trabajo (working)
    - **git add <nombre fichero>**.- Añade el fichero <nombre fichero> de la copia de trabajo (working)
3. **git status**.- muestra el estado de la copia de trabajo (working).
4.	**git commit**.- sube los cambios de la copia de trabajo bajo el control de versiones (que están en zona de intercambio personal) (working) en el repositorio local.
    - **git commit -m “Mensaje de la versión”** .- Se añade un mensaje a la versión para así localizarla con mayor facilidad.
    - **git commit --amend -m “Mensaje modificado”**.- Cambia el mensaje de la última versión (HEAD)
5.	**git log**.- muestra la lista de versiones subidas en el repositorio local.
    - ** git log --oneline**.- muestra las versiones subidas en local de forma resumida.
    - ** git log --graph --all --oneline**.-  muestra un resumen de las versiones subidas, de manera gráfica, útil cuando trabajamos con ramas.
6.	**git annotate <nombre fichero>**.- Muestra en pantalla los los usuarios que han modificado el fichero <nombre fichero>
7.	**git checkout -- <nombre fichero>**.- Recupera el fichero <nombre fichero> de la última versión de nuestro repositorio (HEAD).
    - **git checkout -- **.- Recupera todos los ficheros de la última versión de nuestro repositorio (HEAD).
    - ** git checkout <nombre de rama>** .- Cambiar a la rama <nombre rama>
    - ** git checkout –b <nombre rama>**.- crea una rama <nombre rama> y cambia a esa rama.
8.	** git reset <nombre fichero>** .- elimina el fichero <nombre fichero> de la zona de intercambio temporal (staging area)
    - ** git reset --soft HEAD~1 **.- deshace el último commit, pero mantiene los cambios en la zona de intercambio temporal (staging area).
    - ** git reset --hard HEAD~1 **.- deshace el último commit, dejando los fichero tal y como se guardaron en la versión anterior, en la que apunta ahora el HEAD.
9.	**git branch <nombre rama>**.- crea nueva rama <nombre rama>.
    - **git branch –av**.- muestra las ramas del repositorio
    - **git branch –d <nombre rama>**.- elimina la rama <nombre rama>
10.	**git diff**.- muestra los cambios que se han añadido en una versión.
    - **git diff <cod. Hash versión>...HEAD**.- Compara los cambios entre dos versiones.
11.	** git merge <rama1>**.- fusiona los cambios entre dos ramas. Fusiona la <rama1> con la rama en la que estoy actualmente. 
12.	**git show**.- muestra información sobre la versión indicada.
13.	**git push**.- sube los cambios del repositorio local a un repositorio remoto.
14.	**git pull <nombre remoto>**.- baja los cambios de un repositorio remoto al repositorio local.
15.	**git remote**.- añade un repositorio remoto o lista los repositorios remotos enlazados con el repositorio local.
    - **git remote –v**.- muestra los repositorios remotos configurados
    - **git remote add <nombre remoto> URL**.- configura un dispositivo remoto con el nombre <nombre remoto>.
16.	**archivo .gitignore**.- permite añadir una lista de archivos y directorios para excluir del sistema de control de versiones.


