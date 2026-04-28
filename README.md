# DS2-

Projet DS2 : Industrialisation et Automatisation du Déploiement Continu
Membres du Groupe :
Amdouni Sleh
Kbayer Feres

Description du Projet :
Ce projet consiste en la mise en place d'une infrastructure complète de conteneurisation et d'automatisation pour un mini-site web. L'objectif est de passer d'un développement "artisanal" à une architecture industrielle en utilisant Docker pour l'environnement et GitHub Actions pour la pipeline CI/CD.

Fonctionnalités : 

Dockerisation : Création d'une image optimisée basée sur nginx:alpine.
Orchestration : Utilisation de Docker Compose pour gérer les services.
Pipeline CI/CD : Automatisation des tests et du build à chaque push ou Pull Request.
Sécurité : Scan de vulnérabilités et règles de protection de la branche main.

Prérequis :
Pour faire tourner ce projet localement, vous devez avoir installé :
Docker (v20.10+)
Docker Compose (v2.0+)
Git

Installation et Lancement local
Cloner le dépôt :

Bash

git clone [LIEN_DU_DEPOT]
cd [NOM_DU_DOSSIER]
Lancer le projet avec Docker Compose :

Bash

docker-compose up -d
Le site sera accessible sur : http://localhost:8080 


Structure du Projet :
Dockerfile : Configuration de l'image Docker (image de base légère).
docker-compose.yml : Définition des services (Web et bonus).
.dockerignore : Exclusion des fichiers inutiles (.git, node_modules, etc.).
.github/workflows/ci.yml : Workflow automatisé (Tests -> Build -> Scan).

Pipeline CI/CD (GitHub Actions)
La pipeline se déclenche automatiquement sur les branches main et develop :

Tests : Validation des fichiers HTML/CSS.
Build : Construction de l'image Docker pour vérifier l'absence d'erreurs.
Security Scan (Bonus) : Analyse des vulnérabilités de l'image.

                                       Projet réalisé dans le cadre du module Problem Solving - Avril 2026.
