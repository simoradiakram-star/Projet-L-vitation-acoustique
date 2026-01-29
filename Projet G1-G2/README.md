# 📁 Nos Prototypes

Ce répertoire contient la documentation technique, les fichiers de conception (STL) et les spécifications matérielles des trois itérations de lévitateurs développées durant le projet.

## 1. TinyLev (Prototype de Validation)

Le **TinyLev** est un lévitateur à ondes stationnaires fixes.

* **Objectif** : Valider les principes fondamentaux de la lévitation acoustique et tester la chaîne d'amplification.
* **Caractéristique** : Utilise deux supports imprimés en 3D suivant une courbe prédéfinie pour focaliser les ultrasons au centre.

## 2. Lévitateur à Simple Plaque (Monoplaque)

Ce prototype marque le passage au contrôle dynamique via une matrice unique de **8x8 transducteurs**.

* **Capacités** : Permet de tester les algorithmes de calcul de phase (**Optimizer** et **Vortex**).
* **Limites** : Bien qu'il valide la création de pièges acoustiques, la force de lévitation reste limitée par l'absence d'une source d'opposition, rendant le piégeage d'objets lourds complexe.

## 3. Lévitateur à Double Plaque (Bi-plaques)

Version la plus aboutie du projet, elle intègre deux matrices de transducteurs placées face à face.

* **Fonctionnement** : Génère des ondes stationnaires contrôlées par la synchronisation des deux plaques.
* **Avantages** :
* Augmentation considérable de la **force de piégeage**.
* **Stabilité supérieure** permettant la manipulation de liquides ou de plusieurs particules simultanément.
* Contrôle précis du déplacement vertical par déphasage relatif des deux matrices.
* `/Specs` : Fiches techniques des transducteurs 40 kHz utilisés.
