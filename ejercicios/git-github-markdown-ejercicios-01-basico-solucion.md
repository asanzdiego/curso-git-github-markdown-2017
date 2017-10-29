# Solución ejercicios Git, GitHub y Markdown



## Repositorio masteruah

1. Crear un repositorio en vuestro GitHub llamado **masteruah**.


![Crear un repositorio](../slides/img/git/github-new-repo.png)

1. Clonar vuestro repositio en local.

~~~
git clone git@github.com:asanzdiego/masteruah.git
~~~

## README

1. Crear (si no lo habéis creado ya) en vuestro repositorio local
un documento **README.md**.

> Notas: en este documento tendreís que ir poniendo los **comandos**
> que habéis tenido que utilizar durante todos los ejercicios
> y las **explicaciones y capturas de pantalla** que consideréis **necesarias**.

~~~
touch README.md
~~~

## Commit inicial

1. Añadir al README.md los comanddos utilizados hasta ahora
y hacer un coomit inicial con el mensaje **commit inicial**.

~~~
git add .
git commit -m "commit inicial"
~~~

## Push inicial

1. Subir los cambios al repositorio remoto.

~~~
git push origin master
~~~

## Ignorar archivos

1. Crear en el repositorio local un fichero llamado **privado.txt**.

~~~
touch privado.txt
~~~

1. Crear en el repositorio local una carpeta llamada **privada**.

~~~
mkdir privada
~~~

1. Realizar los cambios oportunos para que tanto el archivo como
la carpeta sean ignorados por git.

~~~
echo "privado.txt" > .gitignore
echo "/privada" > .gitignore
git add .
git commit -m "añadido fichero .gitignore"
~~~

## Añadir fichero 1.txt

1. Añadir fichero **1.txt** al repositorio local.

~~~
touch 1.txt
git add .
git commit -m "añadido 1.txt"
~~~

## Crear el tag v0.1

1. Crear un tag **v0.1**.

~~~
git tag v0.1
~~~

## Subir el tag v0.1

1. Subir los cambios al repositorio remoto.

~~~
git push --tag origin master
~~~

## Crear una rama v0.2

1. Crear una rama **v0.2**.

~~~
git branch v0.2
~~~

1. Posiciona tu carpeta de trabajo en esta rama.

~~~
git checkout v0.2
~~~

## Añadir fichero 1.txt

1. Añadir un fichero **2.txt** en la rama **v0.2**.

~~~
touch 2.txt
git add .
git commit -m "añadido 2.txt"
~~~
