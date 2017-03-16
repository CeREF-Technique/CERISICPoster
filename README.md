# CERISICPoster

This repository is a LaTeX package designed to help CERISIC researcher writing their A0 posters. A usage example is given in the file "poster_example.tex".

## Package Installation
To install this package you will have to download and copy it in the 'right' place. Then you will need to update the database TeX uses to find files. The place to put the file depends on your operating system. Assuming you have a standard installation, this will probably be something like this:

* Windows: "C:\Program Files\MiKTeX 2.9\tex\latex"
* Linux: "~/texmf/tex/latex/local/"
* Mac OS X: "/Users/<user name>/Library/texmf/tex/latex/local/"

To refresh the database you should open a command prompt or a terminal and type "texhash". This should work on most operating systems. In case it doesn't work for you (and you are using MikTeX), it is also possible to refresh the database with the user interface. Open the "Windows Start Menu" and search for "MikTeX Settings Admin". Then in the "General" tab, click on "Refresh FNDB" in order to update the database.

## Usage

### Load the package
In order to use the package, you will have load the package before the \begin{document} command, as below:
\usepackage{CERISICPoster}

### Before \begin{document}
This package will 
\postertitle{\textbf{Projet First HE: NAME}}
\postersubtitle{A very long and complicated subtitle}
\authors{J. {\sc Doe}\textsuperscript{1}}
\institutes{1: CERISIC}
\contact{john.doe@cerisic.be}
\industrialpartner{0.5\textwidth}{img/Cerisic.jpg}
\scientificpartner{0.5\textwidth}{img/Cerisic.jpg}

### After \begin{document}
Use the command *\makeposter* to generate the outline of the poster.

This package will also give you acces to 2 main environments.
\begin{firstcolumn}
  \section{1. Context}
\end{firstcolumn}
\begin{secondcolumn}
\end{secondcolumn}
