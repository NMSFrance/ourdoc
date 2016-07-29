# Code
Ici tu vas voir comment tout le monde devra développer. Le but n'est pas de t'ennuyer mais de garder un code homogène qui rend les choses plus simples pour débugger !

## General
Applicable à tous les langages

### Indentation
Deux espaces. Attention à ne pas mettre de tab space, il s'agit bien de 2 espaces.
```
// Bien
block
  block
    block
      block
        ...

// Pas bien
block
    block
        block
            ...
```

### Constantes
Doivent être écrites en MAJUSCULE snake_case
```
FOOBAR // <- ceci est une constante
FOO_BAR // <- ceci est une constante
Foo_BAR // <- ceci n'est pas une constante
foobar // <- ceci n'est pas une constante
```

### Variables
Doivent être écrites en minuscule camelCase
```
foobar // <- ceci est une variable
fooBar // <- ceci est une variable
foor_bar // <- ceci n'est pas une variable
Foobar // <- ceci n'est pas une variable
```

### Objets
Doivent être écrits en CamelCase
```
Foobar // <- ceci est une objet
FooBar // <- ceci est une objet
fooBar // <- ceci n'est pas une objet
Foo_Bar // <- ceci n'est pas une objet
```

### Fonctions et méthodes
Doivent être écrites en minuscule camelCase. Le block doit être espacé d'un espace.
```
// Pas bon
function a(){
}

// Bon
function a() {
}
```

### Affectation et opérations
Les opérateurs doivent toujours être espacés, sauf pour les parenthèses.
```
a = 1 // Bon
a = b + (1 - 2) // Bon
a = b+1 // Pas bon
```

### Bloques et conditions ternaires
Les bloques en ligne sont permis et recommandés que si ils font moins de 100 caractères (columns). Sinon, écrire les conditions en bloque. Les conditions ternaires s'appliquent à cette règle.
```
for(;;) sayHi() // Bon
a = (isTrue()) ? 'yes' : 'no' // Bon

// Bon
if(thisFonctionIsReallyReallyLong() && thisIsAnotherReallyLongFunction()) {
  return true
} else {
  return false
}

// Pas bon, c'est trop long pour le inline
if(thisFonctionIsReallyReallyLong() && thisIsAnotherReallyLongFunction()) return true
else return false

// Bon
if(isTrue()) return true
else return false
```

### Commentaires
Un commentaire sur une ligne doit pas exceder plus de 100 caractères (columns), sinon, un bloque de commentaire doi être préféré.
```
// short com <- Good
// this is a very very very very very very very very very very very very very very very very very very very very long com <- Bad

/*
 * this is a very very very very very very very very very very
 * very very very very very very very very very very very very
 * very very very long com <- Good
 */
```
Ne jamais push du code commenté. Ce code doit être supprimé.
```
// a = 1 <- doit être supprimé
```

## PHP

## TypeScript

