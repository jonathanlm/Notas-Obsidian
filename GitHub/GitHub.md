Para bajar actualizaciones
> Git Pull

Para subir actualizaciones
> Git Push

Las versiones que se va subiendo son
> Commits

## Primer Paso
Tenemos que crear un repositorio en nuestro GitHub
![[001.jpg|500]]

## Segundo Paso
Tenemos que instalar nuestro GitHub de la siguiente pagina
>https://git-scm.com/downloads

## Tercer Paso
Antes de instalar Nuestro Git debemos de escoger nuestro editor por defecto debemos escoger NANO, si se domina otro editor como VIM, escoger el que mas convenga. Luego dar Next hasta finalizar.
![[002.jpg|400]]

## Cuarto Paso
- Para subir algun archivo a Git tendremos que abrir un terminal. Y escribir el siguiente comando para saber si tenemos instalado Git 
>git --version
![[003.jpg]]
- Luego ubicarnos en la carpeta donde se encuentra nuestro archivo en este caso mis notas de LaTeX "cd" = para ingresar a cualquier carpeta "ls"= para ver que contiene esa carpeta ![[004.jpg]]

## Quinto Paso
- Ahora debemos inicializar un repositorio Git: Si el directorio actual no es un repositorio Git válido, puedes inicializar uno nuevo utilizando el comando 

>git init. 

Esto creará un nuevo repositorio Git en el directorio actual y debería resolver cualquier error.
- Se nos creara una carpeta de GitHub a causa del 

>git init

- Posteriormente usaremos el comando de "git add LaTeX" = LaTeX es el nombre de la carpeta que se subira al repositorio de git en la nube.

>git add LaTeX

![[006.jpg|450]]
![[005.jpg]]

## Sexto Paso
- Para subir varias directorios a GitHub se hara de la siguiente manera
> git add .obsidian/ ANEXOS/ LaTeX/
![[008.jpg]]

## Septimo Paso
- Ahora debemos hacer un commit que significa dar una descripcion de la carpeta o directorio que subiras a Git, se usara el siguiente comando 
>git commit -m "Version01"

![[007.jpg]]

## Octavo paso
- Debemos de conectar el repositorio local con el repositorio remoto en GitHub. Ejecuta el siguiente comando:

>git remote add origin https://github.com/jonathanlm/notas-obsidian.git

- Finalmente se ejecuta el siguiente comando 

>git push -u origin master

	- El "master" significa la rama donde se subira el commit el que esta por defecto es "master"

- ==Para mas informacion sobre ramas  terminando el noveno paso==

## Noveno Paso
Para descargar debemos de situarnos en la consola en el lugar que queremos descargar el proyecto o directorio.
![[009.jpg]]

- Una vez seleccionado en el terminal la carpeta donde se descargar se utilizara los siguientes comandos

>git clone https://github.com/jonathanlm/notas-obsidian.git

# Ramas
- Para descargar un commit anterior se hara lo siguiente: Se va en el terminal al directorio que esta tu proyecto. Se escribira el siguiente codigo

>git log

- Podremos ver todas las versiones que hicimos, las versiones que se muestra esta en la ==Rama master== que pertenece a la version 03. Por otro lado vemos que hay otra rama llamada ==rama-anterior== que pertenece a la version 02

![[010.jpg]]

## Crear una nueva Rama
- Una vez estando en el directorio de tu proyecto en la consola usaremos el siguiente codigo

>git checkout -b rama-anterior 1c7c236d9e96f2bde8d3781242d37a44bae5f9d7

- Lo cual ==rama-anterior== significa el nombre que tendra la nueva rama. Y los numero ==1c7c236d9e96f2bde8d3781242d37a44bae5f9d7== son los commit que se hizo en este caso el codigo pertenece a la version 02.

- Ahora colocamos el siguiente codigo
>git clone --branch rama-anterior --single-branch <https://github.com/jonathanlm/notas-obsidian.git>

## Como cambiar de rama a rama
primero colocamos 

>git branch

- Luego hacemos un 

>git checkout "nombre de la rama sin comillas"

- Puede ser dos, uno que creamos anteriormente "master" y "rama-anterior"
- Confirmamos la rama que usaremos

>git checkout master

- Podemos usar tambien 

> git checkout rama-anterior

Hasta aqui mi version 04