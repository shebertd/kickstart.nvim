# Préférences de développement

- Privilégier la simplicité : la complexité est un coût à éviter et à réduire.
- Choisir la solution la plus directe et lisible qui réponde correctement au besoin.
- Limiter les abstractions aux cas où elles résolvent un problème concret. Éviter les couches, wrappers, généralisations et refactorisations spéculatives.
- Ne pas appliquer le « Clean Code » comme une obligation d’abstraire. La duplication n’est pas automatiquement un problème si l’abstraction qui l’éliminerait rend le code plus complexe.
- Garder ensemble le flux principal d’une opération quand cela en facilite la compréhension et le débogage. Ne pas découper une fonction uniquement pour la rendre plus courte ; extraire une fonction pour une raison concrète, comme la réutilisation ou un sous-problème clairement distinct.
- Avant d’introduire une classe ou du polymorphisme, vérifier si une condition explicite suffit. Choisir le mécanisme le plus simple qui exprime clairement les variations réellement nécessaires.
- Envisager d’intégrer une fonction appelée à un seul endroit si cela réduit les signatures et facilite le suivi du flux ; la conserver séparée si elle clarifie un sous-problème distinct.
- Favoriser la localité du comportement : rendre autant que possible évident ce que fait un élément en lisant son code et son contexte proche. Éviter les effets implicites ou dispersés difficiles à retrouver, tout en pesant ce choix face à la réutilisation et à la séparation des responsabilités.
- Limiter le nombre de concepts, classes, interfaces et types introduits. Ajouter une nouvelle notion seulement si elle clarifie réellement le modèle ou répond à un besoin avéré.
- Préférer le Data-Oriented Design lorsque cela clarifie les données, leur organisation et les opérations qui les transforment. Ne pas en faire une règle dogmatique.
- Limiter les dépendances. En ajouter une seulement si son bénéfice concret justifie son coût de maintenance et sa complexité.
- Tester en priorité le comportement observable et les interfaces stables, notamment avec des tests d’intégration lorsqu’ils représentent mieux l’usage réel. Garder les tests unitaires ciblés et éviter de figer inutilement les détails d’implémentation.
- Préserver le comportement existant et faire le changement le plus ciblé qui résout le problème.

Ces préférences s’inspirent des essais [Codin' Dirty](https://htmx.org/essays/codin-dirty/), [Prefer If Statements To Polymorphism](https://htmx.org/essays/prefer-if-statements/) et [Locality of Behaviour](https://htmx.org/essays/locality-of-behaviour/), sans en faire des règles absolues.
