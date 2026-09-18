---
layout: page
title: Machine d’atelier numérisée
description: Conception et fabrication d’une machine d’atelier mêlant mécanique, CAO, impression 3D, électronique et programmation.
importance: 1
type: maker
img: assets/img/maker/machine_atelier/vue-generale.jpg
---

<a href="{{ '/assets/img/maker/machine_atelier/vue-generale.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/vue-generale.jpg' | relative_url }}"
    alt="Vue générale de la machine d'atelier"
    class="project-image"
  />
</a>

Ce projet est né d’un besoin très concret : disposer dans mon petit atelier d’une machine compacte, polyvalente, déplaçable et adaptée à ma manière de travailler.

J’ai conçu et fabriqué un établi multifonction en **profilés aluminium, avec un plateau en contreplaqué**, en intégrant progressivement plusieurs fonctions motorisées et numérisées.

L’objectif n’était pas de reproduire une machine existante, mais de concevoir un système sur mesure, évolutif et réparable, mêlant profilés aluminium, travail du bois, CAO, impression 3D, mécanique, électronique et programmation.

Le système intègre notamment un guide parallèle motorisé, une défonceuse à commande numérique et plusieurs pièces conçues sur mesure.

<a href="{{ '/assets/img/maker/machine_atelier/vue-desassemblee.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/vue-desassemblee.jpg' | relative_url }}"
    alt="Vue générale de la machine en cours d'assemblage"
    class="project-image"
  />
</a>

---

## Guide parallèle motorisé

Le guide parallèle de la scie est déplacé par deux **moteurs pas à pas NEMA 17**, associés à un système de guidage linéaire **HGR15** et à deux vis sans fin.

Des **capteurs de fin de course** permettent de sécuriser et de référencer les déplacements à chaque démarrage.

La mécanique, les supports et différentes pièces d’intégration ont été conçus en CAO puis fabriqués ou adaptés pour l’ensemble.

<a href="{{ '/assets/img/maker/machine_atelier/guide-parallele.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/guide-parallele.jpg' | relative_url }}"
    alt="Guide parallèle motorisé"
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
- des pièces réalisées à la **CNC** afin d’obtenir un positionnement précis de la visserie.

Cette partie du projet a demandé plusieurs essais afin d’obtenir un déplacement suffisamment fiable et reproductible.

<a href="{{ '/assets/img/maker/machine_atelier/defonceuse.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/defonceuse.jpg' | relative_url }}"
    alt="Installation de la défonceuse motorisée"
    class="project-image"
  />
</a>

---

## Électronique et contrôle

Pour piloter l’ensemble, j’ai adapté une **carte MKS DLC32** aux besoins spécifiques de la machine. Le système est pilotable depuis un écran tactile configuré pour mon usage, avec des drivers que j’avais déjà en stock ainsi qu’une alimentation 12 V.

Le projet mêle ainsi plusieurs domaines que j’aime faire dialoguer :

**mécanique · électronique · CAO · impression 3D · programmation**

Plutôt que de chercher une solution entièrement prête à l’emploi, j’ai adapté le matériel et le logiciel aux besoins spécifiques de la machine.

<a href="{{ '/assets/img/maker/machine_atelier/controleur.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/controleur.jpg' | relative_url }}"
    alt="Carte de contrôle et écran tactile de la machine"
    class="project-image"
  />
</a>

---

## Motorisation de la scie

Pour la motorisation de la scie sous table, j’ai préféré utiliser un **moteur à induction** plutôt qu’un **moteur universel**, principalement afin de réduire les nuisances sonores.

L’installation a été réalisée sur mesure à partir de la carcasse d’une ancienne scie sous table.

<a href="{{ '/assets/img/maker/machine_atelier/moteurac.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/machine_atelier/moteurac.jpg' | relative_url }}"
    alt="Motorisation à induction de la scie sous table"
    class="project-image"
  />
</a>

---

## Une machine pensée comme un prototype évolutif

Le projet a beaucoup évolué au fil des essais. Certaines solutions ont fonctionné immédiatement, d’autres ont nécessité plusieurs versions, des modifications de pièces ou des changements de conception.

---

## Technologies & techniques

**CAO**

Fusion 360

**Fabrication**

Impression 3D · Travail du bois · Profilés aluminium · CNC · Usinage et assemblage

**Mécanique**

NEMA 17 · HGR15 · SBR12 · Transmissions · Axes · Guidages linéaires · Fins de course

**Électronique**

MKS DLC32 · Moteurs pas à pas · Drivers · Capteurs · Câblage · Alimentation

**Programmation / contrôle**

Configuration et adaptation du système de commande
