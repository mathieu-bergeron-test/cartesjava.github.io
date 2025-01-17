---
title: "Annexe 3: programmer un nouvel exemple"
bookCollapseSection: false
bookNumbering: false
weight: 200
---

{{% pageTitle %}}

## Préalables

* JDK 11 ou plus récent (testé jusqu'à JDK18)
* Git
* Eclipse

## Cloner les sources

Dans un GitBash (ou à la console en Linux ou Mac)&nbsp;:

```bash
$ git clone https://github.com/cartesjava/ca.ntro.cards.git
```

## Créer un nouveau projet

Pour créer une nouvelle visualisation avec les cartes&nbsp;:

```bash
$ sh scripts/new_project.sh MonProjet mon_projet
```

Pour créer un nouveau validateur&nbsp;:


```bash
$ sh scripts/new_validator.sh MesModeles mes_modeles
```

## Créer et importer les projets Eclipse

Générer les projets Eclipse avec&nbsp;:

```bash
$ sh gradlew eclipse
```

Importer les projets en Eclipse. 

## Modifier la visualisation avec les cartes

S'inspirer des projets `shift_procedure` et `fibonacci_procedure`.

Dans le projet `mon_projet_procedure`, modifier le paquet `models`.

Renommer au besoin la classe `MonProjetCardsModel`.

Implanter les méthodes marquées d'un `TODO` et que l'outil de validation utilise&nbsp;:

* `copyDataFrom`&nbsp;: copier les données d'un autre modèle.
* `compareToSolution`&nbsp;: valider si le modèle courant est une solution.
* `updateViewDataImpl`&nbsp;: afficher les cartes correspondant au modèle courant.
* `initializeAsTestCase`&nbsp;: données de départ d'un cas de test.

Finalement, modifier aussi  `test_cases.MonProjetTestCaseDatabase`, en particulier&nbsp;:

* `describeTestCasesToGenerate`&nbsp;: faire la liste des cas de tests à générer.


## Ajouter des modèles à un validateur

Dans le projet `validator_mes_modeles`, modifier le paquet `models`.

S'inspirer de `Model01` et `Model01SuperClass` pour voir comment créer un nouveau modèle.

Ne pas oublier d'implanter la méthode `copyDataFrom` qui est utilisée par l'outil copier un modèle.

