# Prototype 2 : Lévitateur à Simple Plaque (Monoplaque)

Ce prototype constitue la deuxième phase du projet. Il marque le passage d'une géométrie fixe à un système dynamique piloté par logiciel, utilisant une matrice plane de **8x8 transducteurs**.

## Raison d'être

L'objectif de ce prototype était de s'affranchir des contraintes physiques du TinyLev pour explorer la manipulation logicielle. Il a servi de banc d'essai pour :

* L'implémentation de la **modulation de phase** individuelle pour chaque transducteur ;
* La création de pièges acoustiques (points de pression) par calcul algorithmique ;
* La mise en place d'une architecture électronique capable de gérer 64 transducteurs.

## Fonctionnalités

* **Contrôle Dynamique** : Capacité à modifier la position du piège acoustique sans déplacer physiquement les transducteurs ;
* **Algorithmes Avancés** : Test et validation des méthodes **Optimizer** et **Vortex** ;
* **Interface Arduino/Python** : Liaison entre les scripts de calcul de phase (Python) et l'exécution matérielle (Arduino Mega).

## Limites

* **Force de lévitation** : En l'absence d'une plaque opposée pour créer des ondes stationnaires parfaites, la force de piégeage reste relativement faible (pression de radiation seule).
* **Stabilité** : Les objets sont sensibles à toute intervention autour de la plaque, notamment par manque de force de lévitation.

## Évolution : Vers le Prototype 3 (Double Plaque)

Pour pallier le manque de puissance et de stabilité, l'étape suivante consiste à ajouter une seconde plaque identique en vis-à-vis. Cette configuration permettra de créer des **ondes stationnaires** beaucoup plus puissantes, autorisant la lévitation de liquides et une manipulation multi-particules.

---

## 📂 Organisation des dossiers

### 📁 Electronique

Ce dossier contient les documents nécessaires à l'assemblage physique :

* **Schémas** : Diagrammes de câblage de la matrice et des drivers.
* **Montage** : Instructions pour l'interfaçage entre l'Arduino Mega et le shield de puissance.

### 📁 Informatique

Ce dossier regroupe les programmes de pilotage :

* **Génération de phases** : Scripts Python pour transformer des coordonnées (x, y, z) en signaux.
* **Code Arduino** : Firmware optimisé pour l'envoi rapide des données aux transducteurs.

### 📁 Physique théorique

* **Modèles** : Explications sur le potentiel de Gorkov et la pression de radiation.
* **Calcul des phases** : Détails mathématiques sur les fonctions de coût et les méthodes d'optimisation.

---

*Note : Pour une vue d'ensemble du projet, référez-vous à la documentation technique à la racine du dépôt.*
