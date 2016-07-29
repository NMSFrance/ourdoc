# GitHub workflow

Il y aura toujours 2 branches sur lesquelles ont ne devra jamais push directement notre travail :
- `master` qui servira pour la production,
- `dev` qui servira pour le développement.

Nous allons travailler avec les branches. Une branche devra être créée pour contextualiser le travail à réaliser, par exemple je souhaite refondre des éléments graphiques, je vais créer une branche `design-update`.

## Etapes
- Créer un branche basée sur la branche `dev` : `git checkout -b "nom de la branche"`,
- Travailler dessus en local,
- Une fois une partie ou la totalité du travail terminé, push la branche : `git push "remote" "nom de la branche"`,
- Ensuite, réaliser une pull request en comparant la branche utilisée avec la branche `dev`, le code sera review et discuté si besoin,
- Une fois validé, le code est mergé si il n'y a pas de conflit. En cas de conflit(s) c'est au développeur qui a push la branch de le/les résoudre.
- Si la branche n'est plus utile, la supprimer.

## Convention pour le commit
Préfixer les messages de commit par les mots libelles suivants :
- FEAT: nouvelle fonctionnalité,
- CHANGE: modification de code,
- FIX: correction d'un bug,
- REFACT: refactoring et structure du code (tout ce qui n'a pas d'impact sur les fonctionnalités et l'apparence du produit).

Quand un commit comporte plusieurs objectifs à la fois, choisir le libelle le plus parlant, exemple de commit message :
`CHANGE: bannière du site`

On va rester sur du français pour les tickets ainsi que les messages de commit. Le message devra être neutre et doit stipuler qu'est ce qu'il impacte. Dans l'exemple du dessus il s'agit d'une modification sur la bannière du site.

Lorsqu'un commit solutionne ou apporte une solution à quelque chose d'évoqué dans un ou plusieurs ticket(s). Optionnellement, ajouter la mention `closes #ticket-number1 #ticket-number2 ...` dans le message du commit. Sinon, il est possible de faire la même chose dans une pull request.

# Mise en production
À définir....

# Tickets
Lorqu'un bug a été découvert, il faut laisser apparaître un écrit. Pour cela on va utiliser les tickets de GitHub.

Pour déclarer un bug un ticket doit être de la forme suivante

```
URL : chemin/vers/le/bug (la page où le bug a été vu)

BROWSER : Mozilla/Chrome/IE... - Mobile/PC

REPRODUCTION : comment reproduire le bug, comment tu as été amené à le voir.

DESCRIPTION : optionnel, tu peux donner des idées sur son origine ou apporter des précisions par exemple.
```
