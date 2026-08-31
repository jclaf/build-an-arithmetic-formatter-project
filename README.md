# Arithmetic Arranger

Ce projet contient une fonction Python `arithmetic_arranger` conçue pour formater des problèmes d'arithmétique (additions et soustractions) côte à côte, de manière similaire à une feuille d'exercices scolaire. Cette fonction fait partie des projets proposés par la formation *Scientific Computing with Python* de freeCodeCamp.

## Fonctionnalités

* **Mise en page propre :** Aligne les nombres et les opérateurs verticalement pour jusqu'à 5 problèmes simultanés.
* **Affichage optionnel des résultats :** Permet d'inclure ou non les réponses calculées en bas des colonnes.
* **Gestion rigoureuse des erreurs :** Valide les entrées et renvoie des messages d'erreur explicites en cas de non-conformité.

## Règles de validation et erreurs possibles

La fonction vérifie les critères suivants et retourne une chaîne d'erreur si l'un d'eux n'est pas respecté :
* **Trop de problèmes :** Maximum 5 problèmes autorisés (`Error: Too many problems.`).
* **Opérateurs valides :** Seuls les opérateurs `+` et `-` sont acceptés (`Error: Operator must be '+' or '-'`).
* **Chiffres uniquement :** Les opérandes doivent contenir exclusivement des chiffres (`Error: Numbers must only contain digits.`).
* **Longueur des nombres :** Chaque nombre ne peut pas dépasser 4 chiffres (`Error: Numbers cannot be more than four digits.`).

## Utilisation

Voici des exemples d'utilisation de la fonction :

```python
# Affichage simple de deux problèmes
print(arithmetic_arranger(["3801 - 2", "123 + 49"]))

# Affichage de quatre problèmes
print(arithmetic_arranger(["24 + 8215", "3801 - 2", "45 + 43", "123 + 49"]))

# Affichage avec les résultats inclus (show_answers=True)
print(arithmetic_arranger(["3 + 855", "988 + 40"], True))
