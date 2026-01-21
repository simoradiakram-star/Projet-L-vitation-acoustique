# Prototype 1 : Lévitateur à Simple Plaque

Ce prototype constitue la phase 2 du projet. Il utilise une seule surface émissive (8x8 transducteurs) pour générer la lévitation.

## Organisation des dossiers

### 📁 Electronique
Ce dossier contient les documents nécessaires à l'assemblage physique :
* **Schémas** : Plans du PCB pour la matrice unique et sa carte de puissance.
* **Montage** : Instructions pour relier la matrice à l'Arduino et à l'alimentation.

### 📁 Informatique
Ce dossier regroupe les programmes de pilotage :
* **Génération de phases** : Scripts pour créer les fichiers de configuration des pièges (focalisation simple ou vortex).
* **Code Arduino** : Le firmware à téléverser pour contrôler les 64 transducteurs de la plaque.

### 📁 Physique théorique
* **Modèles** : Documents expliquant le principe de lévitation avec une seule source .

---
## Objectif
Valider le fonctionnement du matériel et tester les premiers déplacements d'objets légers (billes de polystyrène).
