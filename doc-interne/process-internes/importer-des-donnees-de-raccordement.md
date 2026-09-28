# Importer des données de raccordement

#### Etapes :&#x20;

1. Récupérer les projets qui ont choisi le CDC 2022, qui ont un identifiant de dossier de raccordement mais pas encore de date de mise en service. Requête metabase : [https://metabase.potentiel.beta.gouv.fr/question/334-recuperer-les-dossiers-de-raccordement-sans-date-de-mise-en-service](https://metabase.potentiel.beta.gouv.fr/question/334-recuperer-les-dossiers-de-raccordement-sans-date-de-mise-en-service)
2. Nettoyer le fichier : corriger le format des identifiants (ex : remplacer les espaces par des tirets si nécessaire, retirer "ENEDIS" devant l'identifiant, etc.) OU corriger les identifiants dans Potentiel avant de faire la requête et l'exporter.&#x20;
3. Envoyer le fichier aux gestionnaires de réseau. Colonnes à conserver : \[> voir le template de Julie]
4. Importer le fichier du gestionnaire de réseau avec les dates de mise en service. L'import aura les effets suivants :&#x20;

* Appliquer la date de mise en service sur le projet correspondant
* Appliquer le délai de 18 mois si la date de mise en service est dans la fourchette définie dans l'AO et la période
