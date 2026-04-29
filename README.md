# Serveur Web multi-applications (sujet 4)

## Présentation du projet
Ce projet porte sur la conception et la mise en place d'une infrastructure serveur sécurisée permettant la cohabitation de plusieurs services web sur une adresse IP unique. L'objectif principal est de démontrer la maîtrise de l'architecture Reverse Proxy et de la gestion des certificats de sécurité.

Membres :
- **Oscar VIVIEN** : Administrateur Système & Réseaux, Responsable Infrastructure
- **Florent FOLLIARD** : Intégrateur Système & Responsable Documentation

## Cahier des charges
Le cahier des charges impose les contraintes techniques suivantes :
* Déploiement d'un serveur sur un OS différent du client en tant que point d'entrée unique.
* Configuration de Nginx pour gérer plusieurs noms de domaine (Virtual Hosts).
* Hébergement d'un site.
* Hébergement d'une application Node.js.
* Sécurisation de l'ensemble des services via le protocole HTTPS.

## Étapes de réalisation
Le projet a été mené selon les phases suivantes :
1.  **Environnement** : Installation et mise à jour du système d'exploitation Ubuntu.
2.  **Services Web** : Installation et configuration de la pile LEMP (Nginx, PHP-FPM, MariaDB).
3. **Site Wordpress** : Déploiement du site et configuration du serveur interne
4.  **Application Node.js** : Déploiement de l'application et configuration du serveur interne.
5.  **Architecture Réseau** : Configuration des Virtual Hosts Nginx pour l'aiguillage du trafic.
6.  **Reverse Proxy** : Liaison des requêtes externes vers l'application Node.js interne sur le port 80.
7.  **Sécurité** : Génération de certificats SSL auto-signés via OpenSSL et configuration des protocoles TLS.
8.  **Validation** : Tests de résolution DNS locale, tests de connectivité et debug des erreurs de configuration (502 Bad Gateway, Erreurs 500,..)

## Outils et Technologies
* **Système d'exploitation** : Ubuntu Server sur VMware, Windows 11 (Client)
* **Serveur Web / Reverse Proxy** : Nginx
* **Langages & Runtime** : PHP 8.3, JavaScript (Node.js)
* **Base de données** : MariaDB
* **Outils de sécurité** : OpenSSL
* **Utilitaires de test** : cURL, UFW

## Documentation complémentaire
Pour toute information relative à l'administration du serveur, à la maintenance des services ou à l'ajout de nouveaux sous-domaines, veuillez vous référer au fichier détaillé :
> **[Documentation_livrable.docx](./Documentation_livrable.docx)**
