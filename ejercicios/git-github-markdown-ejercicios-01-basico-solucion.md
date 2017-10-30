# Solución ejercicios básicos de Git, GitHub y Markdown



## Repositorio masteruah

- Crear un repositorio en vuestro GitHub llamado **masteruah**.

~~~
En el menú de GitHub > Pulsar en el icono “+” > Pinchar en “New repository”
~~~

- Clonar vuestro repositio en local.

~~~
git clone git@github.com:asanzdiego/masteruah.git
~~~

## README

- Crear (si no lo habéis creado ya) en vuestro repositorio local
un documento **README.md**.

> Notas: en este documento tendreís que ir poniendo los **comandos**
> que habéis tenido que utilizar durante todos los ejercicios
> y las **explicaciones y capturas de pantalla** que consideréis **necesarias**.

~~~
touch README.md
~~~

## Commit inicial

- Añadir al README.md los comanddos utilizados hasta ahora
y hacer un coomit inicial con el mensaje **commit inicial**.

~~~
git add .
git commit -m "commit inicial"
~~~

## Push inicial

- Subir los cambios al repositorio remoto.

~~~
git push origin master
~~~

## Ignorar archivos

- Crear en el repositorio local un fichero llamado **privado.txt**.

~~~
touch privado.txt
~~~

- Crear en el repositorio local una carpeta llamada **privada**.

~~~
mkdir privada
~~~

- Realizar los cambios oportunos para que tanto el archivo como
la carpeta sean ignorados por git.

~~~
echo "privado.txt" > .gitignore
echo "/privada" >> .gitignore
git add .
git commit -m "añadido fichero .gitignore"
~~~

## Añadir fichero 1.txt

- Añadir fichero **1.txt** al repositorio local.

~~~
touch 1.txt
git add .
git commit -m "añadido 1.txt"
~~~

## Crear el tag v0.1

- Crear un tag **v0.1**.

~~~
git tag v0.1
~~~

## Subir el tag v0.1

- Subir los cambios al repositorio remoto.

~~~
git push --tag origin master
~~~

## Cuenta de GitHub

- Poner una foto en vuestro perfil de GitHub.

~~~
En el menú de GitHub > Pulsar en la imágen de tu avatar > Pinchar en “Settings” > Pinchar en "Profile"
~~~

- Poner el doble factor de autentificación en vuestra cuenta de GitHub.

~~~
En el menú de GitHub > Pulsar en la imágen de tu avatar > Pinchar en “Settings” > Pinchar en "Security"
~~~

- Añadir (si no lo habéis hecho ya) la clave pública que se corresponde a tu ordenador.

[Seguir esta guía](https://help.github.com/articles/generating-ssh-keys/)

## Uso social de GitHub

- Preguntar los nombres de usuario de GitHub de tus compañeros de clase, búscalos, y sigueles.

~~~
Ir a http://github.com/usuario y pulsar en "Follow"
~~~

- Seguir los repositorios **masteruah** del resto de tus compañeros.

~~~
Ir a http://github.com/usuario y pulsar en "Follow"
~~~

- Añadir una estrella a los repositorios **masteruah** del resto de tus compañeros.

~~~
Ir a http://github.com/usuario/masteruah y pulsar en "Star"
~~~

## Crear una tabla

- Crear una tabla de este estilo en el fichero **README.md**
con la información de varios de tus compañeros de clase:

~~~
|        NOMBRE          |                     GITHUB                        |
|------------------------|---------------------------------------------------|
| Nombre del compañero 1 | [enlace a github 1](http://github.com/asanzdiego) |
| Nombre del compañero 2 | [enlace a github 1](http://github.com/asanzdiego) |
| Nombre del compañero 3 | [enlace a github 3](http://github.com/asanzdiego) |
~~~

## Colaboradores

- Poner a [github.com/asanzdiego](http://github.com/asanzdiego)
como colaborador del repositorio **masteruah**

~~~
Ir a http://github.com/usuario/masteruah > Pinchar en "Settings" > Pinchar en "Collaborators"
~~~