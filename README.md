# Introduction aux conditions en C

## Introduction

Cet exercice vous permettra de vous familiariser avec les structures conditionnelles `if` et `else` en C. Ces structures sont fondamentales en programmation car elles permettent à votre programme de prendre des décisions et d'exécuter différentes portions de code selon certaines conditions. Vous apprendrez également à interagir avec l'utilisateur en récupérant des entrées via la fonction `scanf()`.

## Exercice

### Partie 1 : Comparaison simple

Créez un programme C qui :

1. Déclare deux variables entières `a` et `b`
2. Initialise `a` avec la valeur 10 et `b` avec la valeur 5
3. Compare ces deux variables et affiche un message indiquant :
   - Si `a` est plus grand que `b`
   - Si `a` est égal à `b`
   - Si `a` est plus petit que `b`

Voici un exemple de structure pour commencer :

```c
#include <stdio.h>

int main() {
    int a = 10;
    int b = 5;

    // Votre code de comparaison ici

    return 0;
}
```

### Partie 2 : Test de nombre

Modifiez votre programme pour :

1. Demander à l'utilisateur d'entrer un nombre entier via la fonction `scanf()`
2. Stocker ce nombre dans une nouvelle variable `nombre_utilisateur`
3. Vérifier si ce nombre est :
   - Positif (> 0)
   - Négatif (< 0)
   - Nul (== 0)
4. Afficher le résultat du test

### Partie 3 : Condition multiple

Étendez votre programme pour tester si le nombre entré par l'utilisateur est :

1. Pair ou impair
2. Divisible par 3 (indice : utilisez l'opérateur modulo `%`)
3. Affichez un message combinant ces deux informations

## Résultat attendu

Selon les valeurs utilisées, votre programme doit afficher des résultats similaires à ceux-ci :

```
Partie 1 : Comparaison entre a et b
a est plus grand que b

Partie 2 : Test du nombre
Veuillez entrer un nombre entier : 15
Le nombre 15 est positif

Partie 3 : Tests supplémentaires
Le nombre 15 est impair et divisible par 3
```

Ou encore :

```
Partie 1 : Comparaison entre a et b
a est plus grand que b

Partie 2 : Test du nombre
Veuillez entrer un nombre entier : -4
Le nombre -4 est négatif

Partie 3 : Tests supplémentaires
Le nombre -4 est pair et non divisible par 3
```

## Astuces

- En C, on utilise `==` pour tester l'égalité (et non pas `=` qui est l'opérateur d'affectation)
- Pour tester si un nombre est pair, vérifiez si le reste de la division par 2 est égal à 0 : `nombre % 2 == 0`
- Pour tester si un nombre est divisible par 3, vérifiez si le reste de la division par 3 est égal à 0 : `nombre % 3 == 0`
- La fonction `scanf("%d", &variable)` permet de lire un entier depuis l'entrée standard et de le stocker dans la variable spécifiée

## Pour aller plus loin

Si vous souhaitez approfondir les structures conditionnelles en C, vous pourriez explorer :

- L'opérateur ternaire `condition ? valeur_si_vrai : valeur_si_faux`
- Les structures `switch-case` qui peuvent remplacer certaines cascades de `if-else`
- Les opérateurs logiques `&&` (ET), `||` (OU) et `!` (NON) pour combiner plusieurs conditions

---

_N'oubliez pas que la pratique est essentielle ! Essayez de modifier les valeurs et de créer vos propres tests pour mieux comprendre le fonctionnement des conditions._
