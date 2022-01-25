# Manifeste du dev

## Nos valeurs

Etre developpeur au chemin du local c'est respecter un ensemble de valeurs 
communes qui font écho parmis nos utilisateurs !

### Le partage

Première de toutes ces valeurs : le partage. C'est à notre sens la valeur
principale du chemin du local. c'est avant tout partager son travail, ses rêves
et ses ambitions ! Nous voulons être plus qu'une ESN, nous voulons que nos 
actions aient un impact concrêt autour de nous : pour ça il faut les partager !

### La simplicité

La simplicité comme valeur fondamentale de notre dévellopement, nous voulons
rompre avec les processus complexes, les hiérarchies pyramidales. Nous voulons
qu'au quotidien nos programmeurs appliquent cette philosphie à leur travail,
dans l'optique de simplifier la vie de l'utilisateur.

### L'humilité

Au chemin du local nous sommes des humains, ainsi ils nous arrivent de nous
tromper, c'est pour ça que l'humilité reste essentielle. Etre humble, pour nous,
c'est avant tout être à l'écoute de nos utilisateurs, essayer de comprendre
au mieux leurs besoins et ensemble faire de grandes choses !!

### L'excellence et la qualité

Nos utilisateurs attendent de nous que nos services répondent à leurs besoins
au quotidien. Il est alors essentiel de maintenir une excellence et une
qualité opérationnel. Au chemin du local, la satisfaction de nos utilisateurs
est notre principale objectif.

## Les bonnes pratiques

### Une langue parlée unique

Dans un soucis de cohérence mais aussi de convention il est important de définir le langage utilisé dans le code.

#### Distinction entre écriture de code et écriture destiné à un publique

Afin de simplifier la compréhension, on considèrera que toute ligne et mot produit dans un fichier de code, y compris les documentations, seront considérés comme du code. 

Bien que le code doivent être écrit de façon à ce qu'il puisse être lu par d'autres développeurs, dans le cas de la langue on fera la distinction entre le *code spécifiquement destiné à être lu*, tel que les commentaires et la documentation, et *le code strict* comme la syntaxe du langage et les nom de variable.

- le code strict devra être rédigé **en anglais** 🇬🇧

- le code destiné spécifiquement à être lu sera rédigé **en français** 🇫🇷

### Le respect des conventions

Afin d'uniformiser le code de manière à toujours donné l'impression que ce dernier n'a été produit que par un unique développeurs, chacun de nous devra respecter des conventions *strictes* dans chaques languages utilisés.

Ces dernières ayant déjà été très bien rédigé, voici les conventions que nous choisissons pour :

 - Le Dart : [https://dart.dev/guides/language/effective-dart/style](https://dart.dev/guides/language/effective-dart/style)

 - Le Go : [https://go.dev/doc/effective_go](https://go.dev/doc/effective_go)

 - La JavaScript/Typescript [https://google.github.io/styleguide/tsguide.html](https://google.github.io/styleguide/tsguide.html)

 

 > Petite note sur le JavaScript : l'utilisation de Typescript est imposé dès qu'elle est possible. Cela ce justifie par le fait que Typescript rend le langage fortement typé et permet une meilleur cohérence dans le code.

De manière générale dès qu'une question se pose sur le style, nommage, ou autre question de syntaxe il en viendra de se référer aux conventions de Google.

### La documentation et les commentaires

Le code devra toujours être commenté. Toutefois, avant d'écrire un commentaire il faut s'assurer que le commentaire explique toujours le *pourquoi* et pas le *quoi*.

De très bonnes pratiques [peuvent se trouver ici](https://stackoverflow.blog/2021/07/05/best-practices-for-writing-code-comments/) et ce sont ces bonnes pratiques qui seront suivit par l'équipe.

Pour rapidement résumer l'article :

 - les commentaires ne doivent pas apparaître comme une duplication du code

 - les commentaires ne doivent pas excuser du mauvais code et il vaut mieux réécrire le code de façon à ce qu'il soit compréhensible sans commentaire plutôt que de le commenter

 - il est important de commenter le code qui peut paraître comme non évident pour un autre développeurs et qui pourrait tenter d'être simplifier

 - il faut mettre des commentaires citant les sources lorsque le code est copié de quelque part (comme par exemple Stack overflow)

 - les commentaires peuvent annoter une fonction mofier, incomplette etc.

 

Il revient donc de commenter le code au fure et a mesure qu'il est écrit, mais aussi de documenter les fonctions publiques en respectant les conventions cité plus haut.

### quelques bonnes pratiques sur l'écriture du code

Afin de s'assurer d'avoir la base de code la plus robuste et pérenne possible, il y a certaines bonnes pratiques qui peuvent être appliqué. En voici une liste non exhaustive mais qui donne déjà une bonne direction

#### Écrire du code minimaliste

Par principe, une fonction ne doit pas faire plus de 50 lignes de code (commentaires exclues). Cela permet d'aider à garder un code avec des fonctions compréhensible et qui ne font pas plusieurs tâches différentes.

#### Écrire un code testable

Chaque fonction devra être pensée avec une idée de teste derrière. Cela signifie et rejoins le fait que chaque fonction a une utilité unique puisque il faut pouvoir avoir une attente bien précise en fonction des entrées données.

### Les messages de conmit
Lea messagea de commit seront tous rédigés en Français et devront contenir au plus 70 caractères. Afin de bien indiquer à quoi correspond le commit, un smiley sera **toujours** mis sn premier caractère aelon ![la norme Gitmoj](https://gitmoji.dev/)

### utilisation de Git et GitHub

Nous avons fait le choix se GitHub pour héberger nos repository git. Même si ce choix peut être amené à évoluer avec le temps, le même principe devrait pouvoir s'appliquer. Les règles suivantes s'appliquent d'ailleurs pour l'intégralité des repository créés



#### Les branches 

Chaque projets aura au moins deux branches 

 - la branche `master` sur laquelle se trouve le code qui a été déployé où au moins validé comme stable par l'équipe de développement

 - la branche `dev` qui est la branche de travail avec toutes les fonctionnalités complétés

 
De plus nous aurons une branche par feature, afin que chaque fonctionnalités puissent être revu avant d'être fusionner sur la branche `dev`

#### Les feature

##### Définition

Pour chaque fonctionnalités ou tâche (par exemple : *créer les endpoint du chat* ou encore *créer la page de profil*, une branche **et** une issue sera créé. Ainsi, les issues pourront être attribuées et éventuellement, sur GitHub, triés dans la section projet.

##### Le review

Dès que le développeur assigné à une feature estime avoir terminé, il devra créer une pull request sur la branche dev afin que son code soit revu par un autre développeurs. Sauf cas exceptionnel, un développeur ne peut pas review sa propre feature.
