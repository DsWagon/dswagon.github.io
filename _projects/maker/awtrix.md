---
layout: page
title: AWTRIX affichage ESP32
description: Personnalisation d’un afficheur AWTRIX avec ESP32, données issues d’API et intégration domotique.
importance: 3
type: maker
img: assets/img/maker/awtrix/awtrixmeteo.jpg
---

<a href="{{ '/assets/img/maker/awtrix/awtrixmeteo.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/awtrix/awtrixmeteo.jpg' | relative_url }}"
    alt="Afficheur AWTRIX"
    class="project-image"
  />
</a>

Ce projet part d’un afficheur **AWTRIX basé sur ESP32**, que j’ai personnalisé afin d’afficher différentes informations utiles au quotidien : météo, horaires des transports, pollution de l’air ou encore présence de pollen.

Il me permet également de centraliser les informations provenant de nombreux capteurs : portes ouvertes, fuite d’eau ou, en période de canicule, indication du moment opportun pour ouvrir les fenêtres et aérer.

L’objectif était moins de fabriquer un simple écran que de faire communiquer plusieurs sources de données avec un objet physique : **API, réseau, capteurs et domotique**.

Un projet simple en apparence, mais qui nécessite de faire dialoguer plusieurs systèmes : récupération et traitement de données, appels d’API, automatisations, MQTT et logique de programmation.

---

## Données issues d’API

J’ai développé plusieurs affichages reposant sur la récupération et le traitement de données provenant de services externes.

### Météo-France et RATP

Les données de Météo-France sont récupérées et traitées afin d’afficher directement sur AWTRIX les informations météorologiques utiles.

Le même principe est utilisé avec les données liées aux transports : état des lignes de RER ou de métro, perturbations, ou encore temps d’attente avant l’arrivée du prochain bus à un arrêt.

<a href="{{ '/assets/img/maker/awtrix/meteofranceaffichage.png' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/awtrix/meteofranceaffichage.png' | relative_url }}"
    alt="Affichage de données issues d'API sur AWTRIX"
    class="project-image"
  />
</a>

---

## ESP32 et capteurs

Le système récupère également les données de différents capteurs intégrés à mon environnement domotique : température, ouverture de portes, détection de fuite d’eau ou différents états de présence.

Ces données peuvent être croisées afin de produire une information réellement utile. Par exemple, une automatisation compare les températures intérieure et extérieure pour déterminer le moment opportun pour ouvrir les fenêtres en période de forte chaleur.

AWTRIX permet ensuite de rendre ces informations immédiatement visibles, sans avoir à consulter une application ou une interface.

---

## Intégration domotique

AWTRIX est intégré à mon environnement **Home Assistant** et interagit avec différents services de mon installation domotique.

Cette intégration ne se limite pas à la configuration de Home Assistant : elle nécessite de **programmer la logique des automatisations**, de récupérer et transformer les données provenant d’API ou de capteurs, de gérer les échanges MQTT et de définir les conditions déclenchant les différents affichages et notifications.

<a href="{{ '/assets/img/maker/awtrix/ha.png' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/awtrix/ha.png' | relative_url }}"
    alt="Intégration d'AWTRIX dans Home Assistant"
    class="project-image"
  />
</a>

L’intérêt du projet est de pouvoir ajouter progressivement de nouvelles informations ou interactions sans avoir à reconstruire l’ensemble du système.

AWTRIX constitue ainsi l’une des interfaces visibles d’un écosystème plus large mêlant **capteurs, microcontrôleurs, services réseau, automatisations et programmation**.

L’ensemble s’appuie notamment sur :

**ESP32 · MQTT · Home Assistant · API · réseau · capteurs**

---

## Technologies & techniques

**Programmation / données**

API REST · récupération et traitement de données · logique conditionnelle · automatisations · intégration de services

**IoT / communication**

MQTT · réseau Wi-Fi · ESP32 · capteurs IoT

**Domotique**

Home Assistant · automatisations · intégration de capteurs et services externes
