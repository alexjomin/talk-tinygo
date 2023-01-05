# TinyGo - Ou comment j'ai mis du Go dans mon van

## Abstract

Avec mon fourgon aménagé, lorsqu'on part en vadrouille en mode off-grid, c'est capital de connaitre l'état de chargement de la batterie cellule ainsi que la consommation électrique. Aujourd'hui je suis obligé de sortir mon téléphone à tout bout de champ pour connaitre ces infos.

Victron Energy – la marque de mes panneaux solaire – met à disposition une documentation sur son protocole [VE.Direct](https://www.victronenergy.com/live/vedirect_protocol:faq) j'ai alors voulu essayer de lire les données depuis le contrôleur avec un microcontrôleur afin de pouvoir les afficher.

Alors bien évidemment de tels écrans existent déjà dans le commerce, mais pourquoi acheter lorsqu'on peut construire quelque chose pour (beaucoup) moins cher le tout en apprenant ! 

En regardant un peu les solutions qui s'offraient j'ai alors découvert le projet [TinyGo](https://tinygo.org/) qui me permettait de mettre à profit mes connaissances en Go tout en accèdant aux monde des microcontrôleur auquels je ne me suis rarement frotté dans ma carrière !

TinyGo permet du compiler du code Go pour le monde de l'embarqué sur plus de [80 microcontrollers](https://tinygo.org/docs/reference/microcontrollers/).
  
Le but de ce talk est de vous partager ce que j'ai aprris sur TinyGo et voir ce qu'on peut faire dans le cadre concret de mon fourgon  
  
## Programme

+ Présentation du projet TinyGo
+ Architecture et fonctionnemet global
+ Avantages et limitations par rapport à d'autres solutions comme Arduino et Micropython
+ Présentation du projet dans le cadre de mon fourgon
  + L'objectif et les enjeux
  + Le protocole [VE.Direct](https://www.victronenergy.com/live/vedirect_protocol:faq) et son implémentation en Go
  + Affichage des informations sur le port série et sur un écran
  + Ajout d'un bouton pour changer les écran
  + [WIP] Lecture du niveau des cuves à eaux avec l'ADC (analog to digital converter) 

## Liens

+ [Le repo de mon projet](https://github.com/alexjomin/victron-display)
+ [TinyGo](https://tinygo.org/) 

## Images

### Le prototype 
<img src="https://github.com/alexjomin/victron-display/raw/main/doc/img/hacking-v2.jpg" height="200">

### Le fourgon 
<img src="https://pbs.twimg.com/media/FXi2oLCWIAAJTZG?format=jpg&name=medium" height="200">
