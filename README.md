# Nos conventions
Ce repo n'aura que ce README.md. Il sert de guide des bonnes pratiques pour notre workflow sur GitHub. Ce document est amené à évoluer.

## GitHub workflow

Il y aura toujours 2 branches sur lesquelles ont ne devra jamais push directement notre travail :
- `master` qui servira pour la production,
- `dev` qui servira pour le développement.

Nous allons travailler avec les branches. Une branche devra être créée pour contextualiser le travail à réaliser, par exemple je souhaite refondre des éléments graphiques, je vais créer une branche `design-update`.

### Etapes
- Créer un branche basée sur la branche `dev` : `git checkout -b "nom de la branche"`,
- Travailler dessus en local,
- Une fois une partie ou la totalité du travail terminé, push la branche : `git push "remote" "nom de la branche"`,
- Ensuite, réaliser une pull request en comparant la branche utilisée avec la branche `dev`, le code sera review et discuté si besoin,
- Une fois validé, le code est mergé si il n'y a pas de conflit. En cas de conflit(s) c'est au développeur qui a push la branch de le/les résoudre.
- Si la branche n'est plus utile, la supprimer.

### Convention pour le commit
Préfixer les messages de commit par les mots libellés suivants :
- FEAT: nouvelle fonctionnalité,
- CHANGE: modification de code,
- FIX: correction d'un bug,
- REFACT: refactoring.

Quand un commit comporte plusieurs objectifs à la fois, choisir le libelle le plus parlant, exemple de commit message :
`CHANGE: modifie la bannière du site`

On va rester sur du français pour les tickets ainsi que les messages de commit. Le message devra être neutre et au présent, il doit répondre à la question : _qu'est ce que fait ce commit ?_

Lorsqu'un commit solutionne ou apporte une solution à quelque chose d'évoqué dans un ou plusieurs ticket(s). Optionnellement, ajouter la mention `closes #ticket-number1 #ticket-number2 ...` dans le message du commit. Sinon, il est possible de faire la même chose dans une pull request.

## Mise en production

## Tickets

## Code
