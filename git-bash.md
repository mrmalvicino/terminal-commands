# Git Bash

- [Descargar Git](https://git-scm.com/)

## Crear repositorio

1. Inicializar Git en una carpeta:

```
git init
```

:warning: **El siguiente paso es solo si se está creando un repositorio desde una terminal por primera vez.**

2. (*Opcional*) Definir nombre de usuario y mail:

```
git config --global user.name "username"
git config --global user.email mail@gmail.com
```

:warning: **En caso de todavía no haberlo hecho, crear dentro de la carpeta los directorios y archivos necesarios para comenzar a escribir código, antes del siguiente paso.**

1. Agregar código y hacer un primer commit:

```
git add .
git commit -m "First commit"
```

4. Subir el contenido de la carpeta a la rama "main" de un repositorio vacío llamado "new-repo":

```
git remote add origin www.github.com/user/new-repo.git
git push -u origin main
```

:warning: **Si se está creando un repositorio desde una terminal por primera vez, luego del paso anterior debería abrirse una interfaz de inicio de sesión para vincular la cuenta de Github. El repositorio comenzará a subirse a continuación.**

## Consultas

Consultar el estado de un repositorio:

```
git status
```

Consultar el detalle de todos los commits hechos a lo largo de las distintas versiones:

```
git log
```

Descargar el repositorio "repo" del usuario "user":

```
git clone www.github.com/user/repo.git
```

## Implementación

Implementar todos los cambios hechos:

```
git add .
```

Guardar una captura del estado del repositorio especificando las implementaciones hechas:

```
git commit -m "Escribir acá las implementaciones hechas"
```

Guardar los commits hechos en la rama "main" del repositorio de GitHub:

```
git push -u origin main
```

## Git LFS (Large Files Storage)

- [Descargar Git LFS](https://git-lfs.github.com/)

Usar Git LFS en el repositorio:

```
git lfs install
```

Guardar todos los archivos con extensión "png":

```
git lfs track '*.png'
```

Guardar todos los archivos con extensión "png" de la carpeta "images":

```
git lfs track 'images/*.png'
```

Guardar todos los archivos de la carpeta "images":

```
git lfs track 'images/'
```

Consultar una lista de lo que se está guardando en Git LFS:

```
git lfs track
```

Consultar el detalle de todos los archivos guardados en Git LFS:

```
git lfs ls-files
```

## Otros

Borrrar el último commit sin dejar rastro:

```
git reset --hard HEAD~1
git push -f origin main
```