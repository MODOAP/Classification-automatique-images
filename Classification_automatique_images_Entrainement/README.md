# ModOAP - Classification automatique d'images - Entraînement

Ce carnet permet d'entraîner un modèle à la classification automatique d'images, à partir de données d'entraînement (images + annotations) sur un Google Drive.

Le modèle entraîné peut ensuite être sauvegardé dans un dossier Google Drive.

Il pourra être importé pour être utilisé dans le script ModOAP - Classification automatique d'images - Prédictions.

Ce script implémente la plateforme TensorFlow : https://www.tensorflow.org/

Ce script doit être lancé dans un environnement d'exécution GPU : Exécution -> Modifier le type d'exécution -> GPU

Ce carnet nécessite de synchroniser un compte Google Drive.


## Utilisation

1. Ouvrir le carnet dans l'interface Google Colab [![Open In Colab](colab.svg)](https://colab.research.google.com/github/paulbin501/t1/blob/main/t1.ipynb) et se connecter à un compte Google Drive ?????????????????????

2. Lancer la première cellule et cliquer sur le lien généré pour synchroniser un compte Drive si demandé.
Cette cellule importe les bibliothèques nécessaires à l'utilisation du carnet, et connecte un compte Drive.

3. Dans la cellule Entraînement sur un corpus :
	- Spécifier le chemin vers le dossier contenant le corpus d'entraînement
	- Spécifier le nombre d'époques pour l'entraînement (nombre d'itérations)
	- Spécifier les prétraitements dans le champ "preprocess". Les effets des prétraitements sont décrits dans le script.
	- Lancer la cellule

4. Lancer la cellule "Visualisation de l'entraînement" pour évaluer la qualité du modèle

5. Relancer l'entraînement avec la deuxième cellule en modifiant les paramètres si besoin

6. Sauvegarder le modèle avec la dernière cellule en spécifiant un dossier de sortie sur le drive

Consulter un tutoriel sur l'utilisation générale des carnets Colab (?????????????????????????)

