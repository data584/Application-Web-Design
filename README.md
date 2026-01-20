# Project Title
Este proyecto es una pratica para diseño web


## datos personales

- dato 1
- dato 2
- dato 3


## Datos de la materia:

- dato 1
- dato 2
- dato 3


## Descripción:
en esta materia se vera laravel y composer


## seccion nueva:
Esta es una nueva seccion


## explicacion de algunos titulos
1. titulos y subtitulo se usa el simbolo # se van acumulando para los subtitulos (ej: ## titulo 2), entre mas # mas pequeño es el texto con un maximo de 6 gatos
```sh
# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6
```


2. para el texto en negritas y cursiva
```sh
*Texto en cursiva*
_Texto en cursiva_
**Texto en negrita**
__Texto en negrita__
***Texto en cursiva y negrita***
___Texto en cursiva y negrita___
```

*Texto en cursiva*
_Texto en cursiva_
**Texto en negrita**
__Texto en negrita__
***Texto en cursiva y negrita***
___Texto en cursiva y negrita___



3. lista ordenada
```sh
1. Elemento de la lista 1
2. Elemento de la lista 2
3. Elemento de la lista 3
```
1. Elemento de la lista 1
2. Elemento de la lista 2
3. Elemento de la lista 3



3. lista desordenada
```sh
- Elemento de la lista 1
- Elemento de la lista 2
- Elemento de la lista 3
```
- Elemento de la lista 1
- Elemento de la lista 2
- Elemento de la lista 3




4. enlaces
```sh
[texto del enlace](https://google.com/ "Título opcional del enlace")
<https://google.com>
```
[texto del enlace](https://google.com/ "Título opcional del enlace")
<https://google.com>


5. Imagenes
```sh
![Esta es una imagen de ejemplo](https://unsplash.com/es/fotos/muestras-color-crema-morado-y-blanco-con-delicadas-flores-secas-srOymzEIv30)
```
![Esta es una imagen de ejemplo](https://unsplash.com/es/fotos/muestras-color-crema-morado-y-blanco-con-delicadas-flores-secas-srOymzEIv30)


6. codigo
para el codigo lo puedes poner resaltado
```sh
`texto resaltado`
```
`texto resaltado`

o puedes usar
```sh
```sh
el texto se vera asi
`` `
```
```sh
el texto se vera asi
```

## Comandos de git
- Ver el estado del repositorio local
Enumera los archivos que se han preparado, los que están sin preparar y los archivos sin seguimiento.
```sh
git status
```

- Agregar archivos al Stage
```sh
git add . -> para agregar toda la carpeta
git add archivo -> para agregar un archivo en especifico
```

- Agregar comentarios a un commit
`git commit` sube el commit, para el comentario hay que agregar -m y poner un comentario
```sh
git commit -M "comentario" 
```

- Subir cambios al repositorio remoto
primero se inicializa con `git init`, despues se añaden los archivos con `git add`, se especifica la rama con `git branch`, se añade el repositorio remoto con `git remote add origin`, y al final se realiza el commit
```sh
git init
git add .
git branch -M main
git remote add origin https://github/user/aplicacion.git
git commit -M "comentario" 
```


- Crear, listar, cambiar y eliminar ramas

    - crear ramas: 
        - `git branch nombre-de-la-rama` crear ramas permaneciendp en la rama actual
        - `git checkout -b nombre-de-la-rama` crear y cambiar a la nueva rama
        - `git switch -c nombre-de-la-rama` crear y cambiar a la nueva rama (forma mas moderna)
    - listar ramas: 
        - `git branch` ramas locales 
        - `git branch -a` ramas locales y remotas 
        - `git branch -r` ramas remotas 

    - cambiar:
        `git switch [nombre-de-la-rama]` para moverse entre ramas
    
    - eliminar:
        - `git branch -D nombre-de-la-rama` elimina una rama local aun si fue fusionada 
        - `git push origin --delete nombre-de-la-rama` elimina una rama remota


- Regresar el repositorio a un commit específico (rollback)
    -  primero se usa `git log` para encontrar el hash (ID) del commit que se quiere deshacer
        - `git revert HEAD` para el último commit.
        - `git revert hash_del_commit` para un commit específico

        