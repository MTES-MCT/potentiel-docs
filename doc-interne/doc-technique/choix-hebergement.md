# Choix hébergement

En octobre 2020, nous démarrons le projet de migrer l'hébergement de nos services d'un VPS Ovh vers une nouvelle solution qui permettrait un meilleur déploiement continu.

Voici les différentes pistes avec leurs spécificités, avantages et inconvénients.

## Nos besoins en services

* Serveur Web
  * NodeJS/Express
  * une seule instance suffit
* Base de données
  * ex: Postgres
  * déploiement indépendant des autres services
  * backups réguliers
* Stockage de fichiers
  * Object Storage à la S3
  * bonne redondance requise
* Service de génération PDF
  * NodeJS
  * pilote libreoffice en headless pour convertir .doc en .pdf
  * à venir (pour l'instant, intégré dans serveur web)
* Service de mailing
  * NodeJS
  * appelle mailjet ou autre
  * à venir (pour l'instant, intégré dans serveur web)
* Keycloak (authentification)
  * service autonome
  * disponible sous forme d'image Docker
  * a besoin d'un accès à une base de données
* MessageBus
  * ex: RabbitMQ
  * pour faire communiquer les services entre eux
* Antivirus
  * ex: ClamAV
  * pour analyser les fichiers uploadés par les utilisateurs

## Nos besoins en environnements de déploiement

* local
  * développement sur nos machines
  * lancer tout ou partie des services
  * éviter les différences de config entre développeurs
* developpement
  * déploiement de la branche `dev@HEAD`
  * à chaque `push` sur la branche  `dev`
  * RAZ des données manuel
* staging/recette
  * déploiement de la branche `master@HEAD` (?)
  * à chaque `push` sur la branche `master` (?)
  * à chaque déploiement, restore du dernier dump de la prod
* démo
  * déploiement de la branche `master@1.2.3` (dernière release)
  * à chaque `release`de `master`
  * à chaque déploiement, restore d'un dump spécial démo
* prod
  * déploiement de la branche `master@1.2.3` (dernière release)
  * à chaque `release` de `master`&#x20;
  * données de prod

## Solution actuelle: VPS sur Ovh

Une machine VPS qui tourne sur Ubuntu, configurée entièrement à la main.

### Développement en local

* Aucune structure, les services sont démarrés en ligne de commande sur la machine (ex: node server.js)

#### Avantages

* Simplicité
* Configuration libre (le dev gère à 100%)

#### Inconvénients

* Différences d'environnement/config entre devs

### Déploiement en prod

* Connexion en ssh sur la machine
* git pull && npm run build
* migration de schéma de base, si nécessaire&#x20;

#### Avantages

* Simplicité, contrôle total

#### Inconvénients

* Travail manuel
* Le développeur est garant du savoir de déploiement (bus effect)
* Stateful: l'état de la machine détermine le mode de fonctionnement
* Le déploiement automatique nécessite un service dédié qui tourne sur la machine et qui accepte des appels pour redéploiement
* Gestion manuelle des crash

### Conclusions

* Pratique pour démarrer simplement
* Pas terrible pour bosser à plusieurs ou pour industrialiser le déploiement
* Piste pour améliorer les choses: placer les services dans des containers (dev local et déploiement)

## Paas : Clever Cloud ou Scalingo

Bases de données et certains services managés (backups automatisés, sécurisation, scaling des instances).\
Applications déployées suivant un fichier de configuration json.\
Chez Clever Cloud, on peut également déployer des conteneurs Docker.

### Développement en local

* Aucune structure
* Les services type base de données, qui sont managés en prod, doivent être lancées manuellement en local

#### Avantages

* Comme pour le VPS

#### Inconvénients

* Comme pour le VPS

### Déploiement en prod

* Pas de déploiement de bases de données, qui sont managées
* Manuel: git push sur le PaaS pour déployer une application
* Automatisé: la CI (ex: github actions) push sur le PaaS pour déployer

#### Avantages

* Automatisation aisée

#### Inconvénients

* Lock-in sur les services de bases de données
* Choix limité de bases de données / services managées
* Lock-in sur les recettes de déploiement (sauf si usage de Docker)

### Conclusions

* Apporte sérénité sur les services managés (base de données)
* Risque de différences entre devs locaux et production
* Risque de lock-in

## K8s managé : Ovh ou Scaleway

### Développement en local

**Avantages**

#### Inconvénients

### Déploiement en prod

#### Avantages

**Inconvénients**

### **Conclusions**
