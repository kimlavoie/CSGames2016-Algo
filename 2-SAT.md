# 2-SAT

Votre tâche est de résoudre le problème 2-SAT, qui consiste à vérifier si une expression logique peut être satisfaite 
(être évaluée à "vrai"), pour des clauses d'au plus deux arguments (variables).

Une expression valide pour le problème 2-SAT doit contenir des paires de variables pouvant être inversées (avec le 
symbole ¬) et séparées par un ou logique (avec le symbole ∨ ). Ces paires doivent être séparées par des et logique 
(avec le symbole ∧ ).

Voici un exemple d'expression valide pour le problème 2-SAT:
- (x ∨ y) ∧ (y ∨ ¬z) ∧ (x ∨ z) 

Votre algorithme doit déterminer s'il est possible d'assigner des valeurs logiques aux variable pour que l'expression 
soit évaluée à "vrai".

Dans l'exemple ci-haut, il est possible de le faire en assignant les valeurs suivantes:
- x = vrai
- y = vrai
- z = faux

Ce qui s'évalue de la façon suivante:

1. (vrai ou vrai) et (vrai ou non faux) et (vrai ou faux)
2. vrai et vrai et vrai
3. vrai

Le programme doit donc exprimer que l'expression est satisfiable.
