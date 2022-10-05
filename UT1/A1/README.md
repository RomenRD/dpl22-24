# UT1-A1: Trabajando con git

## Alumnos:

Víctor Manuel Cabrera Abreu (alu1)

Romen Ramos Díaz (alu2)

## 1. Crear Repositorio

Creamos el repositorio desde GitHub y lo llamamos git-work. Tras crearlo con un README.md y una licencia MIT lo clonamos a nuestra máquina con `git clone https://github.com/vmcabreu/git-work.git`

### Creación del repositorio:
<img src="img\0.png">

<img src="img\1.png">

## 2. Creación de ficheros

Tras crear el repositorio y clonarlo, añadiremos tres ficheros al proyecto: index.html, cover.css,bootstrap.min.css

<img src="img\2.png">

Después de crear estos ficheros, subiremos los cambios al upstream mediante varios comandos:
- `git add .` Primero preparamos los cambios realizados en nuestro proyecto
- `git commit -m` Confirmamos mediante un commit junto a un mensaje descriptivo de los cambios
- `git push` Finalizamos subimos las modificaciones hechas al upstream

<img src="img\3.png">

## 3. Fork
Mediante la opción en GitHub de Fork, el alu2 creará un fork del repositorio git-work.

<img src="img\3_1.png">

Tras esto clonará, el fork para poder colaborar en el proyecto.

## 4. Creación de ramas
Alu2 creará una rama en su repo, llamada custom-text mediante `git branch custom-text`.
Tras la creación de la rama, alu2 se mueve a ella con un `git switch custom-text` y se asegura de que esta en la rama correcta con el comando `git branch` .
El alu2 añadirá cambio al index.html y lo subirá al upstream como ya hicimos antes:
- `git add index.html`
- `git commit -m "Cambios en el index.html"` 
- `git --set-upstream origin custom-text`

## 5. Pull Request
El siguiente paso es que alu2 le solicite un pull request a alu1 mediante la web de GitHub.
Para poder aprobar este Pull Request, alu1 probará los cambios en su máquina. Para ello, alu1 necesita acceder a la rama custom-text en el remoto de alu2.
Por lo tanto alu1 añade el remoto en su máquina (`git add RomenRD https://github.com/RomenRD/git-work.git`) y descargamos la rama que queremos con `git fetch RomenRD custom-text` y ahora alu1 se situa en la rama con `git switch custom-text`

<img src="img\4.png">

## 6. Merge

## 7. Conflicto

## 8. Release
  
 
