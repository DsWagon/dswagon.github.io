---
layout: page
title: Machine d’atelier numérisée
description: Conception et fabrication d’une machine d’atelier mêlant mécanique, CAO, impression 3D, électronique et programmation.
importance: 1
type: maker
img: assets/img/maker/machine_atelier/vue-generale.jpg
---

---

<a href="{{ '/assets/img/maker/machine_atelier/vue-generale.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/vue-generale.jpg' | relative_url }}"
    alt="Vue générale de la machine d'atelier"
    class="project-image"
  />
</a>

Ce projet est né d’un besoin très concret : disposer dans mon petit atelier d’une machine compacte, polyvalente, déplacable et adaptée à ma manière de travailler.

J’ai conçu et fabriqué un établi multifonction en **profilés aluminium, contreplaquée pour le dessus**, en intégrant progressivement plusieurs fonctions motorisées et numérisées.

L’objectif n’était pas de reproduire une machine existante, mais de concevoir un système sur mesure, évolutif et réparable, mêlant profilés aluminium, travail du bois, CAO, impression 3D, mécanique, électronique et programmation.
L’objectif était de créer un système compact, polyvalent et évolutif, intégrant notamment un guide parallèle motorisé, une défonceuse à commande numérique et plusieurs pièces conçues sur mesure.

<a href="{{ '/assets/img/maker/machine_atelier/vue-desassemblee.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/vue-desassemblee.jpg' | relative_url }}"
    alt="Vue générale assemblage"
    class="project-image"
  />
</a>

---

## Guide parallèle motorisé

Le guide parallèle de la scie est déplacé par deux **moteur pas à pas NEMA 17** associé à un système de guidage linéaire **HGR15** et deux vis sans fin.
Des **capteurs de fin de course** permettent de sécuriser et référencer les déplacements à chaque démarrage.

La mécanique, les supports et différentes pièces d’intégration ont été conçus en CAO puis fabriqués ou adaptés pour l’ensemble.

<a href="{{ '/assets/img/maker/machine_atelier/guide-parallele.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/guide-parallele.jpg' | relative_url }}"
    alt="Guide parallèle"
    class="project-image"
  />
</a>


---

## Défonceuse motorisée

Une défonceuse est intégrée sous l’établi avec un système permettant de contrôler numériquement sa montée et sa descente.

Le mécanisme utilise notamment :

- un moteur **NEMA 17** ;
- des guidages linéaires ;
- une vis de transmission ;
- des pièces réalisées à la **CNC** afin d'avoir un excellent positionnement de la visserie

Cette partie du projet a demandé plusieurs essais afin d’obtenir un déplacement suffisamment fiable et reproductible.

<a href="{{ '/assets/img/maker/machine_atelier/defonceuse.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/defonceuse.jpg' | relative_url }}"
    alt="Installation défonceuse"
    class="project-image"
  />
</a>

---

## Électronique et contrôle


Pour piloter l’ensemble, j’ai détourné une **carte MKS DLC32**, initialement destinée à des applications d'impression 3D. Le tout est pilotable via un écran tactile modifié pour mes besoins, avec des drivers que j'avais en stock ainsi q'une alimentation 12V.

Le projet mêle ainsi plusieurs domaines que j’aime faire dialoguer :

**mécanique · électronique · CAO · impression 3D · programmation**

Plutôt que de chercher une solution entièrement prête à l’emploi, j’ai adapté le matériel et le logiciel aux besoins spécifiques de la machine.

<a href="{{ '/assets/img/maker/machine_atelier/controleur.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/controleur.jpg' | relative_url }}"
    alt="Carte et écran controllant la machine"
    class="project-image"
  />
</a>

---

## Motorisation de la scie

Pour la motorisation de la scie sous table j'ai préféré utilisé un **moteur à induction** plutôt qu'un **moteur universel** essentiellement pour réduire les nuisances sonores. Ici, l'installation est sur-mesure sur la carcasse d'une vieille scie sous table.

<a href="{{ '/assets/img/maker/machine_atelier/moteurac.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/moteurac.jpg' | relative_url }}"
    alt="Moteur induction, moins de bruit"
    class="project-image"
  />
</a>



---

## Une machine pensée comme un prototype évolutif

Le projet a beaucoup évolué au fil des essais. Certaines solutions ont fonctionné immédiatement, d’autres ont nécessité plusieurs versions, modifications de pièces ou changements de conception.

---

## Technologies & techniques

**CAO**
Fusion 360

**Fabrication**
Impression 3D · Travail du bois · Profilés aluminium · Usinage et assemblage

**Mécanique**
NEMA 17 · HGR15 · SBR12 · transmissions · axes · guidages linéaires · fins de course

**Électronique**
MKS DLC32 · moteurs pas à pas · drivers · capteurs · câblage · alimentation

**Programmation / contrôle**
Configuration et adaptation du système de commande

---
