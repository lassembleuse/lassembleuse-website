---
layout: post
title:  "Faire tourner un site web à l'énergie solaire"
categories: lowtech
author: Claire
---

A la rentrée 2018, Low Tech magazine a donné un très bel exemple de ce qu'était un site radicalement soucieux de son empreinte écologique en sortant une refonte de son site... fonctionnant à l'énergie solaire.

<!--more-->

Pour arriver à un tel résultat, l'équipe technique s'est penchée aussi bien sur le hardware (quel matériel utiliser pour héberger le site ? Comment l'alimenter par énergie solaire ?) que sur le software (comment faire en sorte que le site consomme le moins possible, afin que l'énergie solaire suffise à le rendre disponible ?).

Pour en savoir plus sur la partie hardware, qui n'est pas notre domaine d'expertise, nous vous invitons à creuser [les](http://www.lowtechmagazine.com/2015/10/how-to-build-a-low-tech-internet.html) [articles](https://homebrewserver.club/low-tech-website-howto.html) rendant compte de l'expérience.

Côté software, ce qui a été mis en oeuvre  est riche d'enseignement et source d'inspiration pour une agence comme l'assembeuse. Revue des quelques points clés qui m'ont le plus marquée.

## Passage à un site statique

Pour commencer, sans surprise, l'équipe est passée aux générateurs de sites statiques. Le générateur ici utilisé est [Pelican](https://blog.getpelican.com/), écrit en python.

Le passage à un site statique a été un préalable indispensable pour alléger considérablement le socle du site (pas de base de données, échanges avec le serveur web réduits au strict minimum...). C'est notamment ce qui a permis au site d'être hébergé sur un simple rapsberry pi (mini ordinateur de la taille d'une boîte d'allumette).

## Le moins d'encre possible pour les images

Une astuce que je trouve très bien pensée est celle qui permet d'alléger les images (les images étant l'une des sources principales de poids des sites). S'inspirant de vieux modes d'impression économiques, qui permettaient d'utiliser le moins d'encre possible, Low Tech Mag a pris le parti de convertir ses images en un [half-tone](https://fr.wikipedia.org/wiki/Halftoning) numérique. Et le résultat se tient aussi esthétiquement !

## Faire presque autant avec beaucoup moins

Au delà de la prouesse technique, ce qui me paraît le plus intéressant est ce que la proposition de Low tech magazine traduit de radicalement différent en termes d'offre de service. Ici, nous avons une organisation qui prend acte de la difficulté futur plus que probable à maintenir le niveau d'énergie permettant à des milliards de sites très gourmands de rester en ligne. Il se place donc dans la logique délibérée d'offrir non pas plus en restant à niveau de consommation énergétique constant, mais de consommer aussi peu que possible (bien moins qu'actuellement) quitte à ce que ça implique un service un poil dégradé.

En effet, si le serveur est alimenté à l'énergie solaire (et même s'il se trouve dans une région plutôt ensoleillée), alors il est quasi certain que le site connaîtra des moments d'interruption, lorsque la météo sera de façon prolongée peu clémente.

C'est notamment en anticipation de ces moments d'interruption de service, et afin de les matérialiser, que le site affiche le niveau de la batterie qui l'alimente.

## Interruption volontaire du confort

A ma connaissance, il y a très peu d'organisations qui, en anticipation des difficultés à venir, font le choix de réduire volontairement le niveau de confort et l'étendue de leurs services.

Pour apporter un peu de mesure, il faut tout de même noter que le [site originel](https://www.lowtechmagazine.com/) du magazine est toujours en ligne à côté de sa version solaire. La démonstration est donc incomplète et la démarche reste encore du domaine de la note d'intention.

Malgré tout, est-ce que l'initiative de Low Tech magazine pourrait être le début d'un mouvement visant, de la part des producteurs, à réduire délibérément la [commodité](http://www.internetactu.net/a-lire-ailleurs/la-tyrannie-de-la-commodite/) à laquelle nous sommes habitués, avant qu'elle ne soit brutalement plus possible ?

___

**Le résultat** : [solar.lowtechmagazine.com](https://solar.lowtechmagazine.com/)

Plus d'infos sur les procédés et la technique :
- [How to Build a Low-tech Internet](http://www.lowtechmagazine.com/2015/10/how-to-build-a-low-tech-internet.html) : contexte général de l'initiative
- [How to build a Low-Tech website: Software & Hardware](https://homebrewserver.club/low-tech-website-howto.html) : explication technique de la part des prestataire
