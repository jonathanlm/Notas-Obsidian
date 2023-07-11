# LaTeX 
## Introducción
Para indicar que un documento LATEX es un libro, se debe utilizar el comando o macro **"\documentclass{book}"** y ==para indicar que es un artículo==, se debe utilizar **"\documentclass{article}"**

Un documento LATEX está conformado por texto ordinario al igual que en word (también se incluyen las expresiones matemáticas).

>Basicamente cualquier comando esta acompañado de un contraslash " \ "

- Un documento cualquiera (puede ser un libro científico) casi siempre consta de expresiones matemáticas. Estas expresiones matemáticas en LATEX se escriben dentro del modo matemático y ==para inicializar y finalizar el modo matemático se debe utilizar el signo dólar==, ![[imagen001.png]]

- Existen comandos definidos solo para modo matemático y para modo texto ![[imagen002.png]]

## Editar
El siguiente paso es editar y compilar un documento LATEX:
- ![[Pasted image 20230706023814.png]]

## Compilación
Generalmente se muestran en los editores las
opciones como <mark style="background: #BBFABBA6;">“pdflatex, xelatex, lualatex y otras”</mark> (en la mayoría de los casos se utiliza **<mark style="background: #FF5582A6;">pdflatex</mark>**)

## Cuerpo de un Documento de LaTeX
Un Documento de LaTeX consta de 2 partes:
- **Un Preámbulo**: Van los código de configuración del documento, como tamaños de letras, medidas de margen del articulo o libro.
- **Un Cuerpo del Documento**: Va todo código que se observa o imprime en el documento PDF, obtenido de la compilación de un documento LaTeX.
| ![[imagen003.png|300]] | ![[imagen004.png]]|

## Paquetes LaTeX
Para importar un paquete se invoca el comando **" \usepackage{nombre paquete} "** en el que el argumento obligatorio es el nombre del paquete. 

LaTeX no es un lenguaje de programación sino que es un texto sin formato y TeX, es un lenguaje de expansion de macros.

## Nombres de comandos y entornos
==Los nombres de los comandos y entornos pueden llevar caracteres alfanuméricos==, ==**pero no pueden comenzar con un numero**==.
- El nombre del comando "mycommand" es valido
![[imagen005.jpg|300]]
- <mark style="background: #FF5582A6;">Y el nombre "3mycomando" no es valido</mark>

## Tipos de comandos
### Comandos simples
Los comandos mas simples son de la forma:
- " \bfseries "
- " \sum "
- " \tableofcontents "
- " \newpage "
### Comandos con uno o mas argumentos obligatorios
Los comandos con 1 o mas argumentos son de la forma:
- " \textbf{texto en negrita} "
- " \frac{numerador}{denominador} "
- " \includegraphics{imagen} "
- " \chapter{titulo del capitulo} "
### Comandos con argumentos opcionales
Los comandos con argumentos opcionales son de la forma.
- " \documentclass[==12pt==]{==article==} "
- " \includegraphics[==width=0.5\textwidth==]{imagen} "
- " \chapter[==texto==]{nombre del capitulo} "
- " \twocolumn[] "
### Definir nuevos comandos
Los comandos normalmente se utilizan para tareas repetitivas. Por ejemplo:
- Para ello utilizaremos el código " ==\ldots== "(el cual nos servirá a imprimir algo repetitivo "....")y el comando todo junto " ==$ \infty$== " sirve para imprimir el símbolo de infinito
|![[imagen006.jpg|250]]|![[imagen007.jpg|250]]
