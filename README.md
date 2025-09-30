Ce répertoire contient les fichiers nécessaires à la génération d'un rapport en Latex.

Le fichier principal du document est `main.tex`. En principe, il ne devrait pas être modifié. Les fichiers à éditer sont :
1. `preambule.tex`, qui contient les informations relatives au titre et aux auteurs du document.
2. `paper.tex`, qui renferme le corps du document.
3. `appendix.tex`, qui inclut les annexes.
4. `bib.bib`, qui est le fichier contenant les références bibliographiques.


# Installation

Si le fichier `run_pdflatex` n'est pas exécutable : `chmod +x run_pdflatex`

# Utilisation

`run_pdflatex` est le script bash permettant de générer le PDF à partir des sources Latex - en principe, il devrait installer les paquets nécessaires, au moins sur Ubuntu.

Pour générer le rapport PDF `main.pdf` : `./run_pdflatex`

Pour générer le rapport à chaque modification du fichier `tex` : `ls *.tex | entr ./run_pdflatex` (génère une erreur pour l'instant)

