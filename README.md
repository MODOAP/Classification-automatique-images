# ModOAP - Classification automatique d'images 

Ce script permet de classer les images contenues dans un dossier sur un Google Drive à partir d'un modèle pré-entrainé :

Le modèle entraîné doit être importé depuis un dossier Google Drive (le modèle est obtenu grâce au script ModOAP - Classification automatique d'images - Entraînement)

Les images à classer doivent être contenues dans un dossier Google Drive
Les images sont alors copiées dans un dossier de résultats puis dans un sous-dossier nommé en fonction de la classe associée.

Ce script implémente la plateforme TensorFlow : https://www.tensorflow.org/

Il doit être lancé dans un environnement d'exécution GPU : Exécution -> Modifier le type d'exécution -> GPU

Ce carnet nécessite de synchroniser un compte Google Drive.


## Utilisation

1. Ouvrir le carnet dans l'interface Google Colab et se connecter à un compte Google Drive 

2. Lancer la première cellule et cliquer sur le lien généré pour synchroniser un compte Drive si demandé.
Cette cellule importe les bibliothèques nécessaires à l'utilisation du carnet, et connecte un compte Drive.

3. Dans la cellule "Chargement du modèle", spécifier le chemin vers le dossier Google Drive contenant le modèle entraîné et lancer la cellule. 

4. Dans la cellule suivante : 

	- Spécifier le chemin vers le dossier contenant le corpus d'images à classer
	- Spécifier le chemin vers le dossier où sauvegarder les images classées
	- Spécifier le seuil au dessus duquel associer une image à une classe (par défaut 80)
	- Lancer la cellule

5. Lancer la cellule "Visualiser la répartition des classes associées" pour générer un graphique des classes attribuées


Consulter un tutoriel sur l'utilisation générale des carnets Colab
