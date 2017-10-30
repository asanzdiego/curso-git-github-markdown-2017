# Solución ejercicios avanzados de Git, GitHub y Markdown



## Crear rama remota v0.2

- Subir los cambios al reposiorio remoto.

~~~
git push origin v0.2
~~~

## Merge directo

- Posicionarse en la rama **master**.

~~~
git checkout master
~~~

- Hacer un merge de la rama **v0.2** en la rama **master**.

~~~
git merge v0.2 -m "merge v0.2 sin conflictos"
~~~

## Merge con conflicto

- En la rama **master** poner **Hola** en el fichero **1.txt** y hacer commit.

~~~
git checkout master
echo "Hola" >> 1.txt
git add .
git commit -m "hola en 1.txt"
~~~

- Posicionarse en la rama **v0.2** y poner **Adios** en el fichero "1.txt" y hacer commit.

~~~
git checkout v0.2
echo "Adios" >> 1.txt
git add .
git commit -m "adios en 1.txt"
~~~

- Posicionarse de nuevo en la rama **master** y hacer un merge con la rama **v0.2**

~~~
git checkout master
git merge v0.2
vim 1.txt
git add .
git commit -m "arreglado merge en 1.txt"
~~~

## Listado de ramas

- Listar las ramas con merge y las ramas sin merge.

~~~
git branch --merged
git branch --no-merged
~~~

## Arreglar conflicto

- Arreglar el conflicto anterior y hacer un commit.

~~~
vim 1.txt
git add .
git commit -m "arreglado merge en 1.txt"
~~~

## Borrar rama

- Crear un tag **v0.2**

~~~
git tag v0.2
~~~

- Borrar la rama **v0.2**

~~~
git branch -d v0.2
~~~

## Listado de cambios

- Listar los distintos commits con sus ramas y sus tags.

~~~
git config --global alias.list 'log --oneline --decorate --graph --all'
git list
~~~

## Cuenta de GitHub

- Poner una foto en vuestro perfil de GitHub.

- Poner el doble factor de autentificación en vuestra cuenta de GitHub.

- Añadir (si no lo habéis hecho ya) la clave pública que se corresponde a tu ordenador.

## Uso social de GitHub

- Preguntar los nombres de usuario de GitHub de tus compañeros de clase, búscalos, y sigueles.

- Seguir los repositorios **masteruah** del resto de tus compañeros.

- Añadir una estrella a los repositorios **masteruah** del resto de tus compañeros.

## Crear una tabla

- Crear una tabla de este estilo en el fichero **README.md** con la información
de varios de tus compañeros de clase:

|        NOMBRE          |                     GITHUB                        |
|------------------------|---------------------------------------------------|
| Nombre del compañero 1 | [enlace a github 1](http://github.com/asanzdiego) |
| Nombre del compañero 2 | [enlace a github 1](http://github.com/asanzdiego) |
| Nombre del compañero 3 | [enlace a github 3](http://github.com/asanzdiego) |

## Colaboradores

- Poner a [github.com/asanzdiego](http://github.com/asanzdiego) como colaborador
del repositorio **masteruah**

## Crear una organización

- Crear una organización llamada **masteruah-tunombredeusuariodegithub**

## Crear equipos

- Crear 2 equipos en la organización **masteruah-tunombredeusuariodegithub**,
uno llamado **administradores** con más permisos y otro **colaboradores** con menos permisos.

- Meter a [github.com/asanzdiego](http://github.com/asanzdiego) y a 2 de vuestros
compañeros de clase en el equipo **administradores**.

- Meter a [github.com/asanzdiego](http://github.com/asanzdiego) y a otros 2 de vuestros
compañeros de clase en el equipo **colaboradores**.

## Crear un index.html

- Crear un index.html que se pueda ver como página web en la organización.

## Crear Pull-requests

- Hacer 2 forks de 2 repositorios **masteruah-tunombredeusuariodegithub.github.io**
de 2 organizaciones de las que no seais ni administradiores ni colaboradores.

- Crearos una rama en cada fork.

- En cada rama modificar el fichero **index.html** añadiendo vuestro nombre.

- Con cada rama hacer un pull-request.

## Gestionar Pull-requests

- Aceptar los pull-request que lleguen a los repositorios de tu organización.
