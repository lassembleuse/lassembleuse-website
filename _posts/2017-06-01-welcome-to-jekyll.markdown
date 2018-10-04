---
layout: post
title:  "Refonte de low tech magazine"
categories: lowtech
author: Claire
---

A la rentrée 2018, Low Tech magazine a donné un très chouette exemple de ce qu'était un site radicalement soucieux de son empreinte écologique en sortant une refonte de son site... fonctionnant à l'énergie solaire.

Pour ça, il se sont penchés aussi bien sur le hardware que sur le software. Pas grand chose à dire côté hardware (ce n'est pas notre domaine de compétences majeures), mais l'explication de ce qui a été mis en oeuvre côté software est riche d'enseignement.

Pour commencer, sans surprise, l'équipe est passée aux générateurs de sites statiques ([Pelican](https://blog.getpelican.com/), en l'occurrence, générateur écrit en python).

Une astuce que je trouve assez chouette est celle trouvée pour alléger la taille des images, l'une des source principale de poids des sites. S'inspirant de vieux modes d'impression économiques, Low Tech Mag a pris le parti (aussi pour des raisons esthétiques) de partir sur du [half-tone](https://fr.wikipedia.org/wiki/Halftoning) numérique.

Ensuite, viennent d'innombrables améliorations de configuration (du choix du système d'exploitation à la configuration d)u serveur web), avec des partis pris clairement expliqués.
