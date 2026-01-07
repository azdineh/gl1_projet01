# Random Letter Generator (Python)

Ce script Python génère aléatoirement des lettres jusqu’à ce que la lettre **"w"** soit sélectionnée.

## 📌 Description

Le programme utilise les modules standards `random` et `string` pour :
- Générer des lettres aléatoires (majuscules et minuscules)
- Afficher chaque lettre générée
- Arrêter l’exécution lorsque la lettre **"w"** est tirée

## 🧠 Fonctionnement

1. Importation des modules nécessaires :
   - `random` : pour le choix aléatoire
   - `string` : pour accéder à l’alphabet

2. Récupération de toutes les lettres :
   - `string.ascii_letters` contient les lettres de `a` à `z` et de `A` à `Z`

3. Boucle `while` :
   - Le programme continue tant que la lettre générée n’est pas `"w"`
   - À chaque itération, une lettre est choisie aléatoirement et affichée

## 🧪 Code source

```python
import random
import string

letters = string.ascii_letters
c = ""

while c != "w":
    c = random.choice(letters)
    print(f"La lettre choisie est {c}")
