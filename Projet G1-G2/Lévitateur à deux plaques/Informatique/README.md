# Pilotage Informatique - Prototype Double Plaque

Ce dossier contient les outils logiciels pour le contrôle du lévitateur à deux plaques (128 transducteurs). L'ajout d'une seconde plaque permet de générer des **ondes stationnaires**, offrant une stabilité et une force de lévitation supérieures au prototype précédent.

## Contenu

* **`Codes arduino mega/`** : Firmware optimisé pour l'Arduino Mega. Il gère l'envoi rapide des signaux aux deux matrices de 64 transducteurs via un mapping de ports spécifique ;
* **`Passage_Phases_python_pin.ipynb`** : Notebook de conversion. Il transforme les phases théoriques (calculées via les méthodes Optimizer ou Vortex) en séquences de bits (octets) prêtes à être injectées dans le code Arduino.

## Utilisation Rapide

1. **Calcul :** Définissez vos phases pour les 128 transducteurs dans le Notebook Python (attention à bien différencier la carte maître et esclave) ;
2. **Conversion :** Générez le "bit buffer" (le mapping prend en compte la disposition physique des deux plaques) ;
3. **Flash :** Copiez les octets générés dans la variable `patterns` du code Arduino ;
4. **Synchro :** Assurez-vous que le **pin 2** est relié au **pin 3** de l'Arduino pour la synchronisation du signal 40 kHz.
