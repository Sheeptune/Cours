
# React - Bases

QUOI : Librairie Javascript qui fonctionne dans le navigateur (avantage en rapidité) pour construire des interfaces utilisateurs
COMMENT : Avec des composants (des blocs dédiés)
POURQUOI :  Permet gestion et maintien de code simplifiés et vient combler certains manques (en fonctionnalité) d’une écriture plus traditionnelle avec HTML CSS et JAVASCRIPT

## Les principes de Javascript ES2015

- Let : qui remplace var, elle peuvent changer et on peut les assigner plusieurs fois
- Const : pour les variables qui ne changent pas et qu’on assigne qu’une fois (ne recevra jamais une nouvelle valeur)
- Les fonctions fléchées : **function myFnc ( ) {** est remplacé par **const myFnc = ( ) => {** qui permet d’éviter les erreurs à l’usage de this (par conservation du contexte)
- Les exports et les imports : default si un seul export, avec const si plusieurs choses à exporter (attention à ne pas oublier l'usage des accolades pour les éléments nommés)
```
export default person
import person from ‘./person.js’
export const clean = () =>
import {clean} from ‘./utility.js’
```

- Les classes : Elles peuvent contenir des propriétés (des variables) et des methodes (des fonctions). Elle est instancié comme tel :

