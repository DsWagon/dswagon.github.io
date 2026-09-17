---
layout: page
title: AWTRIX affichage connecté ESP32
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

Ce projet part d’un afficheur **AWTRIX basé sur ESP32**, que j’ai personnalisé afin d’afficher différentes informations utiles au quotidien, la météo, les horaires des transports, la pollution de l'air ou encore la présence de pollen.
Il me sert également de récupérer de nombreux capteurs, portes ouvertes, fuite d'eau, ou en ces temps de canicules... de savoir précisément **quand** ouvrire la fenètre afin d'aérer. 

L’objectif était moins de fabriquer un simple écran que de faire communiquer plusieurs sources de données avec un objet physique : **API, réseau, capteurs et domotique**.

---

## Données issues d’API

J’ai notamment développé des affichages utilisant des données récupérées depuis différentes API.

### Météo-France

Récupération et traitement de données météorologiques afin d’afficher directement sur AWTRIX les informations utiles.

<a href="{{ '/assets/img/maker/awtrix/meteofranceaffichage.png' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/awtrix/meteofranceaffichage.png' | relative_url }}"
    alt="Affichage de données issues d'API sur AWTRIX"
    class="project-image"
  />
</a>

### RATP

Utilisation de données issues de l’API RATP pour afficher des informations liées aux transports, les problèmes sur la ligne du RER ou du métro ou encore la récupération de l'arrivée du prochain bus à un arrêt

<a href="{{ '/assets/img/maker/awtrix/affichage-api.jpg' | relative_url }}" target="_blank">
  <img
    src="{{ '/assets/img/maker/awtrix/affichage-api.jpg' | relative_url }}"
    alt="Affichage de données issues d'API sur AWTRIX"
    class="project-image"
  />
</a>

---

## ESP32 et capteurs

Le projet s’intègre également à plusieurs expérimentations autour de la récupération de **données de capteurs** me permettant de travailler sur la communication entre services réseau et affichage physique.

---

## Intégration domotique

AWTRIX est intégré à mon environnement **Home Assistant** et peut interagir avec différents services de mon installation domotique.

L’ensemble s’appuie notamment sur :

**ESP32 · MQTT · Home Assistant · API · réseau · capteurs**

L’intérêt du projet est de pouvoir ajouter progressivement de nouvelles informations ou interactions sans avoir à reconstruire l’ensemble du système.

---

## Technologies & techniques

**Microcontrôleur**

ESP32

**Programmation / données**

API REST · traitement de données · automatisation

**IoT / communication**

MQTT · réseau Wi-Fi · capteurs iOT

**Domotique**

Home Assistant

**Prototypage**

Configuration · tests · intégration · adaptation
