---
description: Cf. Definition of ready
---

# Conceptions métier et technique (obsolète)

## Règles

* Les sujets doivent être préparés au maximum en amont, en terme de conceptions métier et technique.
* Toute carte planifiée dans un sprint qui doit être développée est a minima au statut "conception technique" et idéalement au statut "prêt à développer".
* Pour les cartes au statut "conception métier" dans un sprint, l'attente à la fin du sprint n'est pas sur le développement de la fonctionnalité mais sur la finalisation de sa conception métier.



## Rôles&#x20;

Ces rôles sont affectés pour chaque sujet / epic dans Airtable priorisé dans la roadmap.

<figure><img src="../../../.gitbook/assets/image (21).png" alt="" width="375"><figcaption></figcaption></figure>

*   **Référent métier** :&#x20;

    * Il porte les besoins métier et enjeux sur un sujet, il est responsable notamment de sa priorisation.
    * Il décrit en détails les besoins des utilisateurs pour la réalisation des fonctionnalités dans Potentiel par l'équipe technique avec l'aide du facilitateur tech.
    * Il présente les besoins utilisateurs à l'équipe et répond aux questions de l'équipe.
    * Il valide que les fonctionnalités développées par l'équipe technique répondent bien aux besoins utilisateurs qu'il a décrit.
    * Il s'assure avec le chargé de déploiement de la communication aux utilisateurs sur les fonctionnalités une fois déployées en Production.


* **Facilitateur tech** :&#x20;
  * Il aide le référent métier à décrire en détails les besoins utilisateurs pour la réalisation des fonctionnalités dans Potentiel par l'équipe technique.
  * Il facilite les échanges avec l'équipe technique notamment sur la présentation des besoins utilisateurs par le référent métier.
  * Il est responsable avec l'équipe technique et la représente lors de la planification du sujet (complexité, planification dans les sprints).
  * Il s'assure avec l'équipe technique que les fonctionnalités développées ont été présentées au référent métier et que tout est prêt pour que le référent métier puisse les valider.&#x20;
  * Il s'assure avec l'équipe technique du déploiement des fonctionnalités en Production.

## Préparation d'une carte en "conception métier"

Pour une carte en "conception métier" ci-après les informations qui sont attendues d'être décrites dans les propriétés d'une carte sous Airtable :

* [ ] "**Priorité métier**" : Estimation de la priorité métier (bloquante, haute, moyenne, basse). Les cartes de "priorité métier" bloquantes et hautes sont indispensables pour la réalisation d'un epic / sujet fonctionnel.
* [ ] "**Rôle(s) concerné(s) dans Potentiel**" : Choisir le(s) rôle(s) utilisateur(s) concerné(s) dans Potentiel parmi la liste.
* [ ] "**Besoin utilisateur (En tant que...)**" : Le besoin utilisateur est détaillé dans la carte sous le format suivant :

&#x20;   **En tant que** \[QUI - utilisateur], &#x20;

&#x20;   **je veux** \[QUOI - description de son besoin]&#x20;

&#x20;   **afin de** \[POURQUOI - objectif à atteindre]

_Exemple :_&#x20;

_**En tant** que porteur de projet_&#x20;

_**Je veux** renouveler une garantie financière sur un projet en cas de changement de producteur, une décision du producteur, une garantie financière obsolète_&#x20;

_**Afin que** la garantie financière soit conforme au cahier des charges jusqu’à l'achèvement du projet._

* [ ] "**Règles métier**" : Détailler les règles métier qui sont à respecter ou à contrôler lors du développement de la fonctionnalité.

_Exemple "Règles métier" :_&#x20;

* _Dépôt de la demande de raccordement si son projet est retenu et s’il ne l’a pas déjà fait_
* _Le Candidat dont l’offre a été retenue dépose sa demande de raccordement dans les trois (3) mois suivant la Date de désignation_&#x20;

- [ ] "**Etapes du parcours utilisateur (UX)**" : A remplir uniquement si l'expérience utilisateur est modifiée dans Potentiel.

_Exemple "Etapes du parcours utilisateur (UX)"_ _:_&#x20;

1. _Cliquer sur le lien "Modifier"_
2. _Saisir la référence du dossier de raccordement du projet_
3. _Téléverser l'accusé de réception de la DCR_
4. _Saisir la date de l'accusé de réception_
5. _Cliquer sur le bouton "Modifier"_



## Revue d'une carte en "conception métier"

La revue d'une carte au statut en "conception métier" avec l'équipe se fait lors d'un atelier de conception métier ou lors de la planification du sprint si peu de complexité.

Ci-après les propriétés d'une carte Airtable qui sont revues et complétées :&#x20;

* [ ] "**Priorité métier**"
* [ ] "**Rôle(s) concerné(s) dans Potentiel**"
* [ ] "**Besoin utilisateur (En tant que...)**"
* [ ] "**Règles métier**"&#x20;
* [ ] "**Etapes du parcours utilisateur (UX)**" : A remplir uniquement si l'expérience utilisateur est modifiée dans Potentiel.
* [ ] "**Impacts sur les autres fonctionnalités**" : A remplir uniquement si impacts sur d'autres fonctionnalités dans Potentiel.

_Exemple "Impacts sur les autres fonctionnalités"_ _:_&#x20;

* _Import des données de raccordement : revoir l'application auto des 18 mois selon la règle ci-dessus >> nouvelle US à prévoir_
* _Vérifier les projets qui ont saisi plusieurs identifiants dans le même champ_

- [ ] "**Tests à effectuer pour valider la fonctionnalité**" : Décrire les tests à effectuer pour valider la fonctionnalité.

_Exemple "Tests à effectuer pour valider la fonctionnalité"_ _:_ &#x20;

_Scenarios à tester :_

* [ ] _Ajout DCR, ajout PTF, modification date de qualification > vérifier que les deux fichiers sont toujours téléchargeables_
* [ ] _Ajout DCR, ajout PTF, modification fichier > vérifier que les deux fichiers sont toujours téléchargeables_
* [ ] _Ajout DCR, ajout PTF, modification ref dossier > vérifier que les deux fichiers sont toujours téléchargeables_
* [ ] _Ajout PTF puis modification fichier PTF et date de signature > vérifier que le fichier est bien téléchargeable_
* [ ] _Ajout PTF puis modification date de signature (et fichier identique) > vérifier que le fichier est bien téléchargeable_

## Passage d'une carte "conception métier" à "conception technique"

Une carte dans Airtable peut être passée du statut "conception métier" au statut "conception technique" si elle respecte les conditions suivantes :

* [ ] La carte a été revue et validée avec le référent métier.
* [ ] Les propriétés "Besoin utilisateur (En tant que...)" et "Règles métier" ont été validées, et éventuellement "Etapes du parcours utilisateur (UX)" si l'expérience utilisateur est modifiée dans Potentiel.
* [ ] La carte a été présentée à l'équipe et revue lors d'un atelier de conception métier ou lors de la planification du sprint si peu de complexité.&#x20;
* [ ] Les propriétés "Tests à effectuer pour valider la fonctionnalité" et "Impacts sur les autres fonctionnalités" (si besoin) ont été complétées.
* [ ] Toutes les questions ont pu être posées par l'équipe lors d'un atelier de conception métier ou lors de la planification du sprint si peu de complexité.



## Préparation d'une carte en "conception technique"

Pour une carte en "conception technique" ci-après les informations qui sont attendues d'être décrites dans les propriétés d'une carte sous Airtable :

* [ ] "**Complexité technique**" : Estimation macro de la complexité de la carte en taille de t-shirt (S, M, L, XL)
* [ ] "**Conception technique**" : les détails techniques pour la réalisation de la carte.&#x20;

Pour une carte en "conception technique" ci-après les activités qui doivent être réalisées pour la conception technique :

* [ ] Si impact sur l'expérience utilisateur, la propriété "Etapes du parcours utilisateur (UX)" est renseignée dans la carte sous Airtable, une étude sur l'expérience utilisateur (UX) est faite.
* [ ] Le diagramme d'activité est fait.

Si la carte est prête techniquement, elle peut être passée du statut "conception technique" au statut "prêt à développer".



##

