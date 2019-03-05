# TP3 Gestion des paquets

## Commandes de base
Pour mettre à jour l'index du dépôt : apt update
Pour mettre à jour les paquets : apt upgrade

Un historique de la commande apt se trouve dans /var/log/apt/history.log
Pour afficher la dernière modification : tail -n 25 /var/log/apt/history.log
Chaque modification est indiquée sur 5 lignes.

Il existe des différences entres dpkg et apt.
Pour compter le nombre de paquets installés :
* Avec apt : apt list --installed | wc -l
* Avec dpkg : dpkg -l | wc -l

Pour compter le nombre de paquet disponible en mis à jour : apt list --upgradable | wc -l

Afin de ne pas avoir a taper les commandes de MAJ, nous pouvons créer un alias.
Exemple : alias maj="sudo apt update && sudo apt upgrade"

Le paquet fortune permete d'afficher des citations depuis une base de données.
## Installation d'un paquet par PPA

## Création de dépôt personnalisé
