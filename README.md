# LXC Multi-Command Executor 

![Bash](https://img.shields.io/badge/Language-Bash-4EAA25.svg)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Status](https://img.shields.io/badge/status-Libre-orange)

Un script Bash interactif et esthétique permettant de diffuser et d'exécuter une commande simultanément sur tous les conteneurs LXC en cours d'exécution de votre serveur hôte. 

Idéal pour les administrateurs système et les passionnés d'auto-hébergement qui souhaitent automatiser la maintenance de leurs conteneurs sans avoir à s'y connecter un par un.

## Fonctionnalités

* **Exécution ciblée :** Ne cible automatiquement que les conteneurs actuellement démarrés (lxc-ls --running), évitant ainsi les erreurs de connexion.
* **Interface colorée :** Sortie console propre, indentée et colorisée pour distinguer facilement les succès des erreurs.
* **Interactif :** Vous demande la commande à exécuter au lancement du script.
* **Léger :** 100% Bash, aucune dépendance externe lourde requise.

## Prérequis

* Un hôte Linux avec **LXC** installé.
* Privilèges root ou sudo pour exécuter lxc-attach.

## Installation

1. Clonez ce dépôt ou téléchargez le script :
   git clone https://github.com/VOTRE_NOM_UTILISATEUR/lxc-commander.git
   cd lxc-commander

2. Rendez le script exécutable :
   chmod +x lxc-commander.sh

## Utilisation

Lancez simplement le script avec les privilèges administrateur :

sudo ./lxc-commander.sh

Une fois lancé, le script vous demandera de saisir la commande à envoyer. 

**Exemple d'utilisation :**
Mettre à jour tous les conteneurs basés sur Debian/Ubuntu :
> apt update && apt upgrade -y

Vérifier l'uptime de tous les conteneurs :
> uptime

## Aperçu

<img width="806" height="747" alt="image" src="https://github.com/user-attachments/assets/ce874b1d-ad39-4ac9-be53-292981a534a7" />

## Contribution

Les contributions, les problèmes (issues) et les demandes d'ajout de fonctionnalités (pull requests) sont les bienvenus ! N'hésitez pas à consulter la page des issues.

## Licence

Ce projet est libre de droit.
