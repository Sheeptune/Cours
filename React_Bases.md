
# React - Bases

**Qu'est ce que c'est** : Librairie Javascript qui fonctionne dans le navigateur (avantage en rapidité) pour construire des interfaces utilisateurs

**Comment ça marche** : Avec des composants (des blocs dédiés)

**Pourquoi on l'utilise** : Permet gestion et maintien de code simplifiés et vient combler certains manques (en fonctionnalité) d’une écriture plus traditionnelle avec HTML CSS et JAVASCRIPT

## Les principes de Javascript ES6 

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

- Les classes : Elles peuvent contenir des propriétés (des variables asscociées à des classes et des objets) et des methodes (des fonctions). Elles sont utilisées pour créér des objets avec des classes sour forme de plans, et sont instanciées comme tel :

```
class Person {
    name = "Max"
    call = () => {...}

const myPerson = new Person ()
myPerson.call()
console.log(myPerson.name)
```

- Extends : Les classes prennent en charge l'héritage ce qui signifie, une autre classe peut hériter de ses propriétés, ses méthodes et potentiellement ajouter de nouvelles propriétés et méthodes.

```
class Person extends Master
```

Lors de l'extension si on utilise un 2eme constructor, ne pas oublier de rajouter **super()**

```
class Human {
    constructor (){
        this.gender = 'female';
    }

    printGender {
        console.log(this.gender)
}

class Person extends Human {
    constructor (){
        super();
        this.name = 'Sheeptune';
    }

    printMyName {
    console.log(this.gender)
}

const Person = new Person;
person.printMyName();
person.printGender();
```

## Les principes de Javascript ES7 

### Classes, Propriétés et Méthodes

Avec ES7 on peut affecter une propriété directement dans sa classe sans passer par un constructor

| ES6                                    | ES7                  |
| -------------------------------------- | -------------------- |
| constructor(){this.myProperty='value'} | myProperty = 'value' |

Avec ES7 la synthaxe des méthodes est également altérée. Il faut l'imaginer une propriété qui stocke une fonction sous forme de valeur.

| ES6             | ES7                    |
| --------------- | ---------------------- |
| myMethod(){...} | myMethod = () => {...} |

Si on reprend l'exercice fait sur extend, on obtient alors :


```
class Human {
    gender = 'female';

    printGender = () => {
        console.log(this.gender)
}

class Person extends Human {
    name = 'Sheeptune';
   
    printMyName = () => {
    console.log(this.gender)
}

const Person = new Person;
person.printMyName();
person.printGender();
```


