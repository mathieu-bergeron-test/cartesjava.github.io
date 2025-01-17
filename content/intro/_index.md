---
title: "Introduction"
weight: 10
bookNumbering: false
---

{{% pageTitle %}}


> Dans ce manuel, nous proposons une approche pour enseigner la programmation
> avec des cartes à jouer.  Les étudiant·e·s seront invité·es à réaliser une
> procédure informatique avec des cartes, avant de programmer cette procédure
> en Java et, puis de valider leur code à l'aide d'un logiciel créé
> spécifiquement pour accompagner ce manuel.
>
> Nous utilisons ensuite cette approche pour expliquer les notions d'efficacité
> (complexité des algorithmes) et de structure de données (en particulier les
> listes, les arbres et les mappages).

## À qui s'adresse ce manuel&nbsp;?

L'approche développée dans ce manuel cible des étudiant·e·s ayant déjà suivi un
cours d'introduction à la programmation, mais qui pourraient éprouver certaines
difficultés à&nbsp;:

* Imaginer les étapes exactes d'une procédure informatique.
* Imaginer comment les données du programme sont organisées en mémoire.
* Réfléchir à l’efficacité du programme.
* Distinguer les notions d'interface (ce que le programme doit faire) et d'implantation (comment le programme le fait).

Comme les exemples de code sont en Java, il est préférable d'avoir une certaine familiarité avec ce langage (ou avec un langage similaire comme C#).




## Pourquoi utiliser des cartes à jouer&nbsp;?

L'idée est d'utiliser un médium physique pour expliquer des notions de
programmation, afin de répondre à différents styles d'apprentissage (visuel,
kinesthésique) et d'encourager les étudiant·e·s à bien comprendre le déroulement
d'une procédure informatique avant même de commencer à la programmer.

Les cartes à jouer sont avantageuses parce qu'elles sont accessibles
et peu coûteuses.  P.&nbsp;ex. il est facile de se procurer des
cartes surdimensionnées pour expliquer des notions informatiques
devant la classe de façon très visuelle.

<center>
<table>
<tr>
<td>
<img class="small-figure" src="/approche/trier/trier_par_numero03.jpg" /><br>&nbsp;
</td>
<td style="text-align:right;">
<img class="small-figure" src="/approche/trier/trier_par_numero02.jpg" />
<br>
Crédit photo&nbsp;: Mikael Tardif
</td>
</table>
</center>


Un autre avantage est qu'on peut vérifier la compréhension des étudiant·e·s dès
la période de théorie, sans même avoir besoin d'ordinateurs. Dans l'exemple
ci-dessous, on spécifie visuellement une opération à effectuer sur une liste de
cartes. Cette opération consiste à déplacer une carte (identifiée par un marqueur) au début de 
liste, ce qui nécessite en retour de décaler certaines cartes vers la droite.

<center>
<table>
<tr>
<th>&nbsp;</th>
<th>Énoncé visuel
</th>
<th>Manipulations sur la table
</th>
</tr>

<tr>

<th>
Opération à réaliser
</th>

<td>
<video autoplay loop mute controls="false" style="width:300px;">
    <source src="decaler_objectif_animation.mp4" type="video/mp4"/>
    <source src="decaler_objectif_animation.webm" type="video/webm"/>
</video>
</td>

<td>
<video autoplay loop mute controls="false" style="width:300px;">
    <source src="decaler_objectif.mp4" type="video/mp4"/>
    <source src="decaler_objectif.webm" type="video/webm"/>
</video>
</td>
</tr>

</table>
</center>

On peut demander aux étudiant·e·s d'effectuer cette opération avec des vraies cartes, 
permettant ainsi à l'enseignant·e de vérifier que l'énoncé a bien été compris (c.-à-d. l'interface, ou ce que le programme doit faire).

On peut ensuite présenter une procédure afin de réaliser l'opération (c.-à-d. l'implantation, ou comment le
programme doit le faire). Dans l'exemple ci-dessous, on utilise une procédure qui parcourt la liste du début vers la fin (ce qui correspond au genre de boucle que les étudiant·e·s ont probablement déjà appris).
Encore une fois, les étudiant·e·s pourront réaliser la procédure sur la table, avec de vraies cartes, et
ainsi s'assurer de comprendre ce qu'il faut programmer avant même d'écrire les premières lignes de code.

<center>
<table>
<tr>
<th>&nbsp;</th>
<th>Énoncé visuel
</th>
<th>Manipulations sur la table
</th>
</tr>

<th>
Procédure à suivre
</th>

<td>
<video autoplay loop mute controls="false" style="width:300px;">
    <source src="decaler_procedure_animation.mp4" type="video/mp4"/>
    <source src="decaler_procedure_animation.webm" type="video/webm"/>
</video>
</td>

<td>
<video autoplay loop mute controls="false" style="width:300px;">
    <source src="decaler_procedure.mp4" type="video/mp4"/>
    <source src="decaler_procedure.webm" type="video/webm"/>
</video>
</td>
</tr>
</table>
</center>

Finalement, à noter les animations ci-haut sont tirées de l'outil de validation qui 
accompagne ce manuel. Grâce à cet outil, les étudiant·e·s peuvent valider 
leur programme, en particulier&nbsp;: 

* Visualiser les étapes d'exécution de leur code.
* Vérifier que leur code arrive au bon résultat.


## Expliquer l'efficacité des algorithmes avec des cartes

Une fois les étudiant·e·s habitué·es à réaliser des procédures avec les cartes à
jouer, on peut passer à expliquer la notion d'efficacité (complexité des
algorithmes), c.-à-d. comment différentes procédures informatiques peuvent
accomplir la même opération (arriver au même résultat), tout en nécessitant un
nombre d'étapes significativement différent.

On distingue ainsi entre les procédures naïves (souvent plus faciles à
comprendre, mais peu efficaces) et les  procédures efficaces (souvent plus
difficiles à comprendre, mais plus rapides à réaliser).  P.&nbsp;ex. pour une
liste de 10 cartes, ordonner les cartes avec une procédure naïve de tri nécessitera une centaine étapes, alors
qu'une procédure efficace de tri arrivera au même résultat en une trentaine d'étapes.

En effectuant diverses procédures sur la table, avec des vraies cartes à jouer, les étudiant·e·s 
gagnent une compréhension très intuitive de la notion d'efficacité informatique: 
les procédures naïves se révèlent rapidement comme longues et ennuyantes à réaliser!


## Expliquer les structures de données avec des cartes

Finalement, on peut aussi se servir de cartes à jouer afin de visualiser
l'organisation des données dans un programme
informatique, ce qui est particulièrement intéressant utile pour expliquer 
comment une structure de données, comme une liste,
peut être implantée de différentes façons dans un langage de programmation.

En s'appuyant sur la notion d'efficacité, on peut aussi expliquer les 
avantages et inconvénients de ces différentes implantations.
P.&nbsp;ex. une liste implantée par
références (liste chaînée) sera moins efficace qu'une liste implantée par
tableau au moment de visiter une valeur mémorisée au milieu de la liste.
Par contre, la liste par référence utilisera moins d'espace en mémoire. 

On peut visualiser ce dernier point assez concrètement avec des cartes à jouer,
surtout si on utilise des cartes blanches (ou le verso de cartes) pour
visualiser l'espace mémoire vide (c.-à-d. l'espace occupé par le programme, mais
dans lequel le programme n'a pas encore mémorisé de valeur).  Une procédure
utilisant beaucoup d'espace mémoire va tout simplement nécessiter plus d'espace
sur la table&nbsp;!

## Plan du manuel

<table>

<tr>
<th>
{{% link "/approche" "Chapitre 1" %}}
</th>

<td> 

Nous présentons l'approche de façon plus détaillée, y compris en survolant
les fonctionnalités de l'outil de validation qui accompagne ce manuel.
Nous discutons des langages et notations que nous utilisons (Java, JSON, diagrammes de classe et graphe d'objets).
Nous donnons des exemples du type de visualisation avec des cartes à jouer que notre approche supporte.
</td>
</tr>

<tr>
<th>
{{% link "/modelisation" "Chapitre 2" %}}
</th>

<td>
Nous donnons des exemples de modélisation de données
qui cadrent bien avec l'approche que nous développons.
En particulier, nous considérons les notions d'objet, de tableau d'objets
et de graphe d'objets.
À travers ce chapitre, nous discutons aussi des limitations
de la visualisation avec des cartes à jouer.
</td>
</tr>

<tr>
<th>
<span class="disabled">Chapitre 3</span>
<!-- {{% link "/efficacite" "Chapitre 3" %}} -->
</th>

<td>
Nous présentons la notion d'efficacité de façon intuitive, sans entrer
dans les détails mathématiques (ce que nous réservons pour l'Annexe 1).
Nous distinguons les notions de performance (une mesure de temps d'exécution) et d'efficacité (une mesure
du nombre d'étapes qu'une procédure nécessite).
Nous différencions aussi l'efficacité en termes de temps (nombre d'étapes) et d'espace mémoire
et donnons quelques exemples du compromis bien connu entre temps et mémoire (on peut souvent réduire le
nombre d'étapes à exécuter si on accepte d'utiliser plus d'espace mémoire).

</td>
</tr>

<tr>
<th>
<span class="disabled">Chapitre 4</span>
<!--{{% link "/listes" "Chapitre 4" %}}-->
</th>

<td>
Nous présentons notre première structure de données&nbsp;: la liste. 
Nous présentons l'interface d'une liste (c.-à-d. quelles opérations une liste doit accomplir), ainsi
que quatre implantations différentes&nbsp;: liste naïve, liste par tableau, liste chaînée simple et liste chaînée double.
Présenter d'abord une implantation naïve nous permet à la fois de bien expliquer l'interface de la liste, mais
aussi d'obtenir un point de comparaison utile pour réfléchir à l'efficacité des différents types de liste.
</td>
</tr>

<tr>
<th>
<span class="disabled">Chapitre 5</span>
<!--{{% link "/arbres" "Chapitre 5" %}}-->
</th>

<td>
Nous présentons la notion d'arbre, une structure de données omniprésente en informatique.
Nous implanterons un arbre générique, ainsi qu'un arbre binaire de recherche.
</td>
</tr>

<tr>
<th>
<span class="disabled">Chapitre 6</span>
<!--{{% link "/mappages" "Chapitre 6" %}}-->
</th>

<td>
Nous présentons notre deuxième structure de données&nbsp;: le mappage.
Nous présentons l'interface d'un mappage,
que trois implantations différentes&nbsp;: mappage naïf, mappage par hachage et mappage par arbre.
Encore une fois, présenter d'abord une implantation naïve permet de bien expliquer l'interface et
d'obtenir un point de comparaison pour réfléchir à l'efficacité des différents types de mappage.
</td>
</tr>

<tr>
<th>
<span class="disabled">Conclusion</span>
<!--{{% link "/conclusion" "Conclusion" %}}-->
</th>

<td>
En guise de conclusion, nous donnons nos impressions sur l'utilisation de notre approche en classe et discutons
d'améliorations et extensions possibles à l'approche.
</td>
</tr>

<tr>
<th>
{{% link "/bibliographie" "Bibliographie" %}}
</th>

<td>
Références bibliographiques.
</td>
</tr>
</table>

## Annexes

<table>



<tr>
<th style="white-space:nowrap;">
{{% link "/annexe_grand_o" "Annexe 1" %}}
</th>

<td>
La notation grand O est présentée de façon plus mathématique.
</td>
</tr>

<tr>
<th style="white-space:nowrap;">
{{% link "/annexe_acceder_exemples" "Annexe 2" %}}
</th>

<td>
Nous expliquons comment accéder aux exemples utilisés dans ce manuel.
</td>
</tr>

<tr>
<th style="white-space:nowrap;">
{{% link "/annexe_programmer_exemple" "Annexe 3" %}}
</th>

<td>
Nous expliquons comment ajouter un nouvel exemple à l'outil de validation.
</td>
</tr>

<tr>
<th style="white-space:nowrap;">
{{% link "/annexe_modifier_manuel" "Annexe 4" %}}
</th>

<td>
Nous expliquons comment adapter ce manuel, ou encore comment suggérer une modification à la version actuelle.
</td>
</tr>


<tr>
<th style="white-space:nowrap;">
{{% link "/annexe_ateliers" "Annexe 5" %}}
</th>

<td>
Nous présentons quatre exemples d'atelier qui utilisent l'approche développée dans ce manuel.
</td>
</tr>

<tr>
<th style="white-space:nowrap;">
{{% link "/annexe_bilans" "Annexe 6" %}}
</th>

<td>
Cet annexe archive les bilans rédigés lors du développement de ce manuel (avril 2022 à février 2023).
</td>
</tr>



</table>
