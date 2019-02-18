# React - Features et Synthaxe de base

### Single VS Multipage App

- SINGLE PAGE APP
Seulement 1 page de contenu HTML délivrée au client. 
La **page entière est généré par javascript et les composants de React**.
Optimise l’expérience utilisateur car on doit pas recharger la page à chaque fois, les choses apparaissent instantanémment.
Ici on a besoin que d’**un seul appel render au ReactDOM**.

- MULTIPAGE APP
On récupère plusieurs pages dont chaque page contient un spécifique à un chemin.
On utilise **React ici pour créer des petits widgets** (gallerie d’image...) . Ici une grande partie du code sera du HTML et CSS traditionnel et des widgets qui ne connaissent pas l’existance d’autres widgets (isolés)
Dans ce cas **on appelle plusieurs fois le render ReactDOM** en définissant la place de l’élément


### Workflow

On a besoin de nmp qui permet de gérer les paquets et les dépendances.
On a besoin d’un blundler (webpack) pour écrire du code modulaire et les scinder en plusieurs fichiers avec un tache propre.
On a aussi besoin d’un compilateur pour compiler le javascript : Babel et Preset

