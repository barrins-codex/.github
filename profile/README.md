# Barrin's Codex
Ensemble de projets destinés à étudier le jeu de cartes à collectionner **Magic: the Gathering**.

## Projets fonctionnels
### [mtgdc_aggregator](https://github.com/barrins-codex/mtgdc_aggregator)
Ce projet se base sur la popularité d'un ensemble de cartes pour générer la decklist permettant d'obtenir le score de popularité le plus élevé.

### [mtgdc_banlist](https://github.com/barrins-codex/mtgdc_banlist)
Ce projet compile les différentes banlists depuis 2015. Cela permet de maintenir un objet permettant d'utiliser la banlist le plus facilement possible sans avoir à utiliser des services comme MTGJSON ou l'API de Scryfall.

### [mtgdc_carddata](https://github.com/barrins-codex/mtgdc_carddata)
Ce projet permet de récupérer les données de MTGJSON et d'utiliser ces données pour améliorer le scrapping de MTGTOP8 avec la classe `CardDatase`. Des procédures permettent de récupérer la carte recherchée avec le début du nom de la carte.

### [mtgdc_decklists](https://github.com/barrins-codex/mtgdc_decklists)
Ce projet compile les decklists extraites de MTGTOP8 et fournit des outils pour utiliser ces decklists. Le module fournit principalement la classe `ImportDecks` qui permet de récupérer des decklists selon les critères fournis (plage de dates, nom et/ou pseudo d'une personne et tous les dérivés utilisés, command zone et decklists totales ou partielles, taille du tournoi, etc).

### [mtgdc_mlpredictions](https://github.com/barrins-codex/mtgdc_mlpredictions)
Ce projet se base sur le machine learning pour évaluer les decklists depuis le passage à 20 points de vie. L'algorithme `XGBoost` permet de comparer le nombre de terrains d'une decklists à l'entrainement effectué avec une fiabilité au-dessus de 85%.

### [mtgdc_scrapper](https://github.com/barrins-codex/mtgdc_scrapper)
Ce projet scrap MTGTOP8 et génère l'ensemble des decklists pour les utiliser dans le module `mtgdc_decklists`.

## Projets en cours de complétion
### [mtgdc_clustering](https://github.com/barrins-codex/mtgdc_clustering)
L'objectif est de réduire la donnée pour étudier plus rapidement un métagame ou l'ensemble des decklists ayant le même général par exemple. Lié au projet `mtgdc_aggregator`, cela permet de réduire le bruit et d'obtenir des versions significativement différentes d'un même deck par exemple.

### [mtgdc_parser](https://github.com/barrins-codex/mtgdc_parser)
L'objectif est d'utiliser d'attribuer un archétype à chaque deck pour définir la popularité ou la direction que prend le format par exemple.
