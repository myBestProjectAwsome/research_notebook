Un carnet de recherche personnel documentant l'apprentissage systématique des mathématiques fondamentales, avec un focus sur la logique, l'algèbre, l'analyse et leurs applications en cryptologie.

## 📚 Contenu

Ce cahier couvre les domaines suivants :

- **Logique et raisonnements** : assertions, quantificateurs, méthodes de preuve
- **Nombres complexes** : forme trigonométrique/exponentielle, racines n-ièmes
- **Nombres réels** : axiomes, densité de ℚ, borne supérieure
- **Suites numériques** : convergence, limites, théorèmes de convergence
- **Arithmétique** : PGCD, Bézout, nombres premiers, congruences, Fermat
- **Ensembles et applications** : injection/surjection/bijection, dénombrement
- **Limites et fonctions continues** : continuité, théorème des valeurs intermédiaires
- **Dérivées** : théorème de Rolle, accroissements finis
- **Groupes** : sous-groupes, morphismes, groupes cycliques
- **Polynômes** : division euclidienne, irréductibilité, éléments simples
- **Formulaire synthétique** : résumé des formules clés par chapitre

## 🎯 Objectif

Construire une référence personnelle structurée pour :
- Maîtriser les fondations mathématiques nécessaires en cryptologie
- Documenter exercices et solutions de manière systématique
- Créer un support de révision visuel et hiérarchisé

## 📂 Structure du dépôt

```
research_book.tex          # fichier maître : assemble le document via \input
preamble.tex                # packages, couleurs, environnements, commandes personnalisées
frontmatter/
  titlepage.tex              # page de titre
  introduction.tex            # introduction générale
chapters/
  01-logique.tex
  02-nombres-complexes.tex
  03-nombres-reels.tex
  04-suites.tex
  05-arithmetique.tex
  06-ensembles-applications.tex
  07-limites-continuite.tex
  08-derivees.tex
  09-groupes.tex
  10-polynomes.tex
  11-conclusion.tex
  12-formulaire.tex
research_book.pdf           # PDF compilé, versionné pour consultation rapide
```

## 🔧 Compilation

```
latexmk -pdf research_book.tex
```

Le fichier `.latexmkrc` redirige automatiquement tous les fichiers de compilation (`.aux`, `.log`, `.toc`, ...) vers un dossier `build/` ignoré par git, afin de garder la racine du dépôt propre.
