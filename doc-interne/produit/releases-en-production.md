# 💻 Releases en production

### 2.24 - 12/06/24

* Modification d'un paragraphe dans le modèle de réponse lors de l'instruction du changement d'actionnariat pour l'AO CRE4 BAT P13
* En tant que DREAL, je dois pouvoir donner accès à Potentiel aux utilisateurs PP sur les projets de ma région au même titre que la DGEC
* Info box à destination des DREAL dans le cas d'un changement de puissance à la hausse non prévu aux CDC
* Affichage du nombre de raccordement par gestionnaire de réseau
* Téléchargement des pièces-jointes harmonisé

Non visible pour le moment : main-levée, ORE, et autres évolutions techniques

### 3.23 - 27/05/24

* Achèvement (transmission par le porteur, modification par DGEC et DREAL, notification DREAL lors de la transmission)
* Formatage "Code Potentiel" dans les courriers de réponse abandon et le modèle de mise en demeure GF
* Filtrer les GF en attente et les GF à traiter par type d'AO
* Gestionnaire de réseau : amélioration de la page liste (notamment ajout d'une barre de recherche)

### 3.22 - 30/04/24

* Migration garanties financières
* Bug sur les raccordements
* Puissance :&#x20;
  * changements à la hausse hors ratios du CDC à instruire par la DGEC&#x20;
  * changement de puissance plafonné par la puissance max de la famille du projet
* UX :&#x20;
  * clarification parcours d'inscription porteur (par formulaire) vs. autres partenaires (par email)
  * suppression de l'item "contrat d'achat" de la frise
* tech : migration backup fichiers outscale, migration domaine "recours" (partie back seulement), étude faisabilité ORE, formattage des dates sur le front, etc.

### 3.21 - 27/02/24

* step 1 import candidats biométhane + correctifs courriers
* wording bouton "notifier les candidats"
* abandon avec recandidature accordés et en attente de preuve de recandidature : ajouter un lien depuis le détail de l'abandon vers le centre de tâches

### 3.20 - 19/02/24

* Sélectionner une preuve de recandidature  (porteur) : ajout des l'AO, période et numéro CRE en plus du nom du projet dans le menu déroulant.
* Import candidats : ajout de l'option "4. Lauréat d'une autre période" (avec premières candidature, abandon classique ou abandon avec recandidature)
* Export de la liste des lauréats : correction bug : affichage nom candidat
* Garanties financières legacy :&#x20;
  * En cas de recours accordé, le porteur doit soumettre un nouveau dépôt de GF (pour validation)
  * Ajout de champs pour le type et la date d'échéance dans les formulaires d'enregistrement de GF (dgec, dreal) et dé dépôt de GF (porteur)
  * GF avec date d'échéance et sans type : ajout de la mention "type de garanties financières à renseigner" pour dgec et dreal
* Nouvelles périodes : PPE2 Sol 5, PPE2 Bâtiment 6
* Mise à jour du logo du Mnistère sur les pages de Potentiel + mails keycloak

### 3.19 - 15/02/24

* \[Dette technique] migration de raccordement
* Modification du texte de l'infobox sur le formulaire de transmission/mise à jour d'une DCR
* \[GF Legacy] Les porteurs peuvent ajouter l'attestation de constitution de GF déjà soumises à la CRE à la candidature
* \[GF Legacy] les dreals sont notifiées en cas de GF enregistrées
* \[bug] téléchargement de la liste des lauréats à notifier corrigé

### 3.18 - 09/02/24

* \[règles métier] mises à jour pour la validation des colonnes du fichier de candidats importé Ce qui change est listé dans "les critères d'acceptation" à tester de cette carte : https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/rectoi54FBz4CalAT?blocks=hide&#x20;
* \[wording] mis à jour et harmonisé : info changement de CDC nécessaire pour accéder aux fonctionnalités de modification de projet (alerte page projet + formulaires de modification)&#x20;
* \[règle métier] Modifications permises avec CDC initial lorsque celui-ci le permet (CRE4 Bâtiment 13, CRE4 ZNI 6).&#x20;
* \[règle métier] Formulaire de correction d'un projet (admin) : ajout d'un champ sur l'actionnariat : financement collectif / gouvernance partagée.&#x20;
* \[règle métier] Volume réservé : afficher sur la page du projet son appartenance à un volume réservé ou non si sa puissance est inférieure ou égale à la puissance max du volume.&#x20;
* \[règle métier] Volume réservé : ajout d'une phrase dans l'attestation de désignation pour les prochaines notifications.&#x20;
* \[Mise en page] Affichage des alertes sur les seuils de puissance des CDC 2022&#x20;
* \[règle métier] Changement email réf pour les courriers des AO Eolien&#x20;
* \[règle métier] Ajout de la période 6 PPE2 Eolien
* Mise à jour logo Marianne sur les attestations de désignation + courriers de réponse DGEC
* Import de l'historique d'abandon (première candidature, abandon classique ou abandon avec recandidature) avec le fichier de candidat

Autres réalisations du sprint : migration de raccordement vers la nouvelle version de l'app

### **3.17 - 24/01/2024**&#x20;

**Produit / métier :**

* La CRE a accès aux abandons
* Filtrer les abandons par preuve de recandidature transmise / en attente
* correction "loupé" : CRE4 Sol P6 a accès aux abandons avec recandidature
* Afficher date envoi preuve recandidature + email porteur

**Dette technique :**

* Gestion des permissions d'accès aux fonctionnalités, gestion des accès aux ressource (nouveau socle)
* Corrections erreurs de build nextjs
* Gestion des routes dans l'app nextjs
* Convention de code
* Filtrer les erreurs sentry
* Filtrage des abandons par rôle
* Pas de props anonymes dans les composants nextjs



### **3.16 - 18/01/2024**&#x20;

**Évolution produit/métier :**

* Ajout d'un titre pour les pages nextjs (abandon, tâches) : le titre est visible sur l'onglet
* Amélioration affichage des abandons sous forme de timeline
* Mise à jour template page demande pour ajouter une infobox à droite du formulaire
* Page projet : accès au formulaire abandon seulement si pas d'abandon en cours et si le CDC le permet
* Abandons triés par date de mise à jour pour les porteurs
* Liens vers les CDC : url vers les pages génériques de la CRE par AO
* Modifications de puissance bloquées par le plafond du volume réservé
* Notifier les Dreals lors d'une modification de puissance enregistrée permise par le CDC 2022
* Wording : "information enregistrée" remplace "information validée"
* Changement de puissance : application des ratios des CDC 2022
* Changement de puissance : explications et justificatifs requis pour toute demande hors ratio (y compris pour le CDC 2022)

**Évolutions techniques :**

* Renommer nom package application SSR
* Exporter props depuis les composants (vs utilisation du type utilitaire Parameters)
* Pluralisation des routes nextjs
* Refactos divers

**Corrections de bugs :**

* Abandon inaccessible pour le projet FIGPIG1351
* Correction manuelle de la puissance du projet Qarson
* Correction lien vers le centre de tâches (accès depuis page projet, page demande...)



### **3.15 - 20/12/2023**

* Passage de la partie abandon dans l'application next avec utilisation direct des composants dsfr
* Pouvoir transmettre la preuve de recandidature
* Ajout de la fonctionnalité "centre des taches" pour transmission de la preuve de recandidature + confirmaiton d'abandon
* AO PPE2 Batiment 1 => Correction lien CDC
* Maj colonnes export ademe
* Création de page d'erreurs personnalisés (dsfr)



### **3.14 - 21/11/2023**

* Impression de la page projet
* Modification du texte automatique dans le courrier de réponse pour les demandes d'abandon classiques pour les périodes à partir de PPE2 bat T5, sol T4, neutre T1 et éolien T4
* Info sur la page d'un délai : ne pas instruire les délais dont l'application est automatique (CDC 2022 et covid)
* Accès des DREAL aux demandes de recours et annulation abandon



### **3.13 - 15/11/2023**

* Notification de la DGEC par email (sur le mail générique aopv) si un projet perd les 18 mois suite à l'ajout d'une nouvelle date de MeS hors intervalle
* En cas de saisie d'une nouvelle DCR sur un projet qui avait déjà bénéficié du délai CDC 2022 de 18 mois, retirer ce délai dans l'attente de la date de mise en service du nouveau dossier
* Correction des délais accordés : feature masquée
* Période 5 eolien disponible
