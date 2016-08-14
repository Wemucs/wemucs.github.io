---
layout: post
title:  "Le développeur et l'ingénierie logicielle"
date:   2016-02-22 15:32:00 +0200
categories: developpement
author: che
---

**Etre un développeur, ce n'est pas juste pisser du code. Non. L'architecture de l'applicatif est bien plus importante et la conception fera la différence entre un bon et mauvais développeur.**

Julien Dollon a tout résumé en un seul tweet :
<blockquote class="twitter-tweet" data-lang="en"><p lang="fr" dir="ltr">Mon conseil a ceux qui veulent apprendre l&#39;ingenierie logiciel: ne travaillez pas pour des gens qui n&#39;heriteront pas de la dette technique.</p>&mdash; JD (@OffTheWake) <a href="https://twitter.com/OffTheWake/status/693609343338450944">January 31, 2016</a></blockquote> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

Alors, voyons un peu ce qui paraît essentiel pour progresser dans le développement et l'ingénierie logicielle plus généralement.

## Les bases
Peu importe votre âge, que vous ayez fait de longues études dans une école prestigieuse ou non : vous devez maîtriser vos bases. J'entends par là :

* Savoir développer sans framework ni librairie
* Connaitre la programmation orientée objet
* Etre à l'aise avec une base de données
* Avoir des notions de réseau
* S'intéresser au hardware

Oui, parce que si vous maîtrisez vos bases, vous comprendrez que tous les langages manipulent des données qui passent leur temps à transiter entre unités de calcul et de stockage.

**Un bon développeur doit pouvoir changer de plateforme ou de langage très rapidement**, s’imprégner d’une nouvelle base de données ou même d’un nouveau protocole en très peu de temps. A chaque fois, ce n'est que question de logique et d'implémentation.

## La curiosité
L'intégrisme mène au côté obscur. Et puis, vous risquez de finir votre carrière à bosser sur des projets fait en ASP 2.0 ou en PHP 4. Chacun son truc mais ce qui fait la beauté du monde, c'est **la diversité**.

Il est vraiment important d'être à l'aise avec un environnement et un langage. Vous coderez plus vite et vous contournerez les pièges. De l'autre côté, être ouvert sera votre plus grande force. Le PHP ou le Java ne sont pas les seuls : vous pourriez être surpris par la simplicité et la rapidité de Python et du Go, ou même des outils Unix/Linux codés en C.

Si vous avez un peu de temps, n'hésitez pas à vous amusez à développer de tous petits applicatifs pour découvrir un nouveau langage. Après tout, les histoires d'amour sont souvent inattendues !

## La dette technique
On entre un peu plus dans le vif du sujet. Maîtriser ses bases, c'est bien. Connaître plusieurs langages et être à l'aise avec des frameworks, c'est mieux. Imaginer un logiciel pour qu'il soit encore en prod dans 10 ans, c'est la réussite !

#### Projets courts et absence de maintenance
Un certain nombre de développeurs bossent sur des projets assez courts (entre 3 mois et 1 an) sans en assumer la maintenance. Au final, c'est soit un autre développeur qui reprendra les spaghettis pour le debugger ou essayer d'y ajouter une fonctionnalité.

Alors ça peut être super cool :

* on peut changer souvent de techno / librairies / frameworks
* on peut sortir du concret très vite
* on peut plus facilement contribuer à l'open source avec de nouveaux projets

Mais vous allez inévitablement contribuer à la plus grande frustration du développeur : reprendre du code qui a plusieurs années écrit par quelqu'un d'autre… Au final, soit vous ferez un hack, soit vous ferez une librairie à part sur un patron de conception différent, **augmentant la dette technique**.

![Shitty code](/assets/images/le-developpeur-et-lingenierie-logicielle/65748811.jpg)

#### Projets longs et dédiés
De l'autre côté, si vous travaillez chez un éditeur ou un "client final", vous aurez sans doute l'opportunité de travailler sur des projets qui resteront en production durant des années, voir des dizaines d'années. Et là, la vision que vous allez avoir est quelque peu différente.

Je ne vais pas revenir sur ce qu'est la dette technique. [Julien l'a très bien décrit dans son article](http://blog.dollon.net/la-dette-technique/), que je vous invite à lire à la suite.

Ne pas créer de dette technique involontaire et contrôler la volontaire, ce sera votre plus grande mission. Et pour cela, pas de magie : c'est **l'expérience** qui parlera. Les vieux ne sont pas tous des cons et ils vous donneront souvent de précieux conseils !
La plus grande réussite, c'est de pouvoir ajouter des fonctionnalités dans 10 ans à votre projet en suivant la même conception de départ avec toutes les briques déjà en place.

Quelques petites remarques en vrac :

* Bien nommer ses variables, fonctions et classes : elles doivent s'auto-décrire sans commentaire, représenter la réalité sans confusion
* La POO, ce n'est pas automatique : le fonctionnel permet de découpler plus facilement les briques
* Les micro-services, c'est bien, mais il faut faire attention de ne pas devoir gérer 50 bases de projets différents
* Les tests unitaires et fonctionnels sont aussi importants que l'implémentation
* Les librairies externes, oui, mais elles ne doivent pas devenir un poids si elles deviennent trop couplées à votre projet
* Et j'en passe !

## Réflection vs tête baissée

Dans une vie de développeur, on rencontre à la fois des projets simples, répétitifs et un peu bateau. Ce qui nous motive réellement, ce sont les **défis complexes** à résoudre et heureusement, on en rencontre très souvent.

Démarrer à coder tout de suite, c'est foncer tête baissée et créer des fondations fragiles. Au final, vous commencez à poser des briques pour construire votre maison sans en avoir dessiné le plan précis.

* Comprenez les besoins métiers, et mettez-vous à la place des utilisateurs. Passez beaucoup de temps avec eux pour tout expliciter et les avertir de ce que vous pourrez et ne pourrez pas faire
* Faites une étude sur l'architecture et les technologies possibles : prenez un papier, un crayon et représentez-les
* Soyez impartial de votre décision : mettez les points positifs en regard des négatifs pour chaque possibilité
* Demandez d'autres avis que le votre en organisant des brainstorming. **C'est en équipe que l'on avance le plus**, vous mettrez sans doute en évidence des points que vous aviez oublié et il faut savoir reconnaitre que vous n'aviez pas la meilleure solution !

## Se remettre en question
Il ne faut pas seulement avoir l'impression de faire du bon travail, il est important de s'en assurer. La définition d'un "bon" travail va varier énormément en fonction des contextes et en fonction des attentes. Cependant, au fur et à mesure de l'avancé de vos projets, **faites un point sur ce que vous venez de créer** : mettez en avant les points forts avec en perspective les parties faibles.

![Continuous Improvement Cycle](/assets/images/le-developpeur-et-lingenierie-logicielle/continuous-improvement-cycle.gif)

Il est évident qu'avec le recul, après mise en production et sans doute les premiers bugs ou comportements non voulus, ou même simplement la difficulté de faire évoluer vos outils, vous pourrez réellement voir ce qui a cloché et comment l'éviter à l'avenir. C'est ça le travail d'un développeur et d'un ingénieur en général : aller de l'avant en étant lucide sur le passé.

Oh, et surtout **pas de vanité**. Utilisez des métriques qui veulent vraiment dire quelque chose, n'essayez pas de cacher la vilaine classe FileUtils qui devient un cauchemar : il faut savoir être sincère dans ces moments là.

## En résumé…
Il faut de tout pour faire un monde ! Si vous préférez changer de projets tous les 4 matins, être à l'affut de toutes les nouveautés, alors restez comme vous êtes et soyez des précurseurs !

A l'inverse, si vous désirez vraiment entrer dans de la conception logicielle, la pure et dure, alors je vous conseille fortement de travailler sur des projets au long court. Cela ne vous empêchera pas de vous éclatez, mais vous allez pouvoir vraiment réfléchir à ce qu'est un bon logiciel et ce qui ne l'est pas.

Et puis, si vous le pouvez, **bossez avec des pointures** dans le domaine. Apprenez sur le tas avec des séniors qui ont des années de dev dans les baskets. Ils seront sans doute de précieux conseils, même si votre première Pull Request aura sans doute 3 commentaires par ligne !

![Self merged](/assets/images/le-developpeur-et-lingenierie-logicielle/57772588.jpg)
