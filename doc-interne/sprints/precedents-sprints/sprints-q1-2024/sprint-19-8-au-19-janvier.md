# 🏃‍♂️ Sprint 19 - 8 au 19 janvier

## 🎯 Objectifs

Objectifs du sprint :&#x20;

* Finaliser le refactoring suite à la migration d'abandon pour recandidature
* Pouvoir différencier sur Potentiel les projets ayant fourni ou non une preuve de recandidature suite à la validation de leur demande d'abandon pour recandidature
* Lister les pré-requis techniques pour AO biométhane sur nouveau socle (notification en mai)

Le comite d'investissement aura lieu le mardi 16 janvier.

## 🛟 Support

Interlocuteurs pour les demandes de support :&#x20;

* Hubert

## 🏝️ Absences

* Hanaë absente demain matin
* Julien absent le 11 janvier
* Sylvain absent du 12 au 15 janvier
* Tiphany en déplacement le 18 janvier

## 🔎 Rétrospective

Lien vers la rétrospective : [https://miro.com/app/board/uXjVNclZGK4=/?share\_link\_id=162759456272](https://miro.com/app/board/uXjVNclZGK4=/?share_link_id=162759456272)

**Actions prises suite à la rétrospective :**&#x20;

* Ajouter météo équipe au niveau de chaque sprint ✅
* Infra : création tickets Sylvain / Hubert
* Ajouter exemples pour les règles métier ✅

**Bonnes pratiques suite à la rétrospective :** &#x20;

* Documenter les process dev (wip) et dans la mesure du possible automatiser
* CONCEPTION - Expliciter les règles métier avec des exemples concret => ajout d'un champ "exemples"
* TESTS - Définition scénario de test dans la carte  (conception métier) + répartition test
* TESTS - Communiquer sur ce qui est couvert par les tests automatisés + points d'attention (démo ou point dédié)
* MEP - Mise en Prod lundi d'après semaine démo
* MEP - Dissocier démo / planif ?
* MIGRATION - Migration d'une fonctionnalité métier : revalider les règles migrées + checklist

## 🎉 Démo

Ordre du jour pour la démo :&#x20;

<details>

<summary>BIZ DEV</summary>

1. **Conception métier & échanges**
   * Vérifier que les bons AO et périodes ont accès aux CDC modificatifs du 30/07/2021
   * Certains projets issus d’AO et périodes doivent choisir des CDC modificatifs pour faire des demandes
   *   Projets qui n’ont pas accès aux CDC 2021 ne doivent pas avoir à changer de CDC pour faire des demandes

       ⇒ Appliquer ensuite une règle temporelle pour appliquer l’obligation de choisir un CDC pour faire des demandes sur Potentiel ?

       Désignation après le 30/07/2021 ?
   * Amélioration du Wording sur la page de changement de CDC
   * Projets en volume réservé
2. **Comité d'investissement**
   * Review Delphine
   * Relance DREAL pour Verbatim CI
   * Stats pour le CI
     *   Quel est le nombre de connexion moyenne par rôle et par jour ou par mois

         [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwRbSf84YqDol1fn/recxZZgiTpjH7SulZ?blocks=hidehttps://docs.google.com/spreadsheets/d/1n\_bVmi3tD7w-3Srk6DIetEok51r7n-qahX2ZDQMEWok/edit#gid=953218482](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwRbSf84YqDol1fn/recxZZgiTpjH7SulZ?blocks=hidehttps://docs.google.com/spreadsheets/d/1n_bVmi3tD7w-3Srk6DIetEok51r7n-qahX2ZDQMEWok/edit#gid=953218482)
     *   Temps moyen de réponse aux demandes

         [https://docs.google.com/spreadsheets/d/1WZSmV99pPOXWkzSbWn8jfK7LcB6Eta5OPIhRBz1IKmc/edit#gid=1146830503](https://docs.google.com/spreadsheets/d/1WZSmV99pPOXWkzSbWn8jfK7LcB6Eta5OPIhRBz1IKmc/edit#gid=1146830503)
   * Point CI
     * Maj slides CI avec les bons chiffres suite à rectification des projets avec des puissance problématiques
     * Prez
     * Distribution des rôles
   * Répétition CI Team Potentiel
   * Répétition du CI avec la fabrique
     * Enlever ou minimiser la partie changement de stack technique
     * Ne pas laisser le choix sur les voies pour Potentiel ⇒ On veut être une plateforme
3.  **TESTS**

    *   Wording “Information enregistrée” au lieu de “information validée”

        ⇒ J’ai testé ETQ DGEC, DREAL et PP (avec test du flow d’une demande)
    *   Ordonner par date de mise à jour desc (du plus récent au plus ancien) les abandons pour les porteurs

        ⇒ J’ai testé ETQ DGEC & DREAL
    *   Modifier les URL de redirection vers les CDC sur les pages projets

        ⇒ J’ai testé ETQ DGEC chaque AO 1 fois, avec famille et CDC au hasard dont ceux (initial, 30/07/21 et 30/08/22)
    * Testing sur le formulaire dédié à ADMIN DGEC pour faire des corrections sur les projets, on pour générer l’attestation de désignation
      *   Problématique des projets ayant une puissance “hors norme”

          ⇒ réglé avec le formulaire disponible sur la page projet

          ⇒ Stats à jour sur la partie puissance pour le CI
      * Testing et CR sur le formulaire de rectification d’un projet pour étudier le besoin avec A\&T (voir blocage) [https://docs.google.com/document/d/141tJiMSxIp2DbGlcOtZ-jQa5PtC5lEMOLd1hhDuBB7I/edit](https://docs.google.com/document/d/141tJiMSxIp2DbGlcOtZ-jQa5PtC5lEMOLd1hhDuBB7I/edit)
    * Bloquer un changement de puissance au-delà du plafond pour les projets en volumes réservés

    [https://drive.google.com/drive/u/0/folders/1WsLRoh-ixo-Il1xk28nEB3ZvUJ4067pj](https://drive.google.com/drive/u/0/folders/1WsLRoh-ixo-Il1xk28nEB3ZvUJ4067pj)

    *   Appliquer les ratio de changement de puissance du CDC 2022 - En cours

        CR : Identification de 6 problématiques, dont 2 qui empêche la MEP & création de 2 cartes [https://docs.google.com/document/d/1A0uf4ceyeGCQlX8\_UrHkKpXErPPBpMSbdVerjny4t1Q/edit](https://docs.google.com/document/d/1A0uf4ceyeGCQlX8_UrHkKpXErPPBpMSbdVerjny4t1Q/edit)
    * Prévoir une notification à la DREAL concernée lors de la validation de l'info de puissance fourchette CDC2022 par le PP [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/recbYpOWLc9k6CTx9?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/recbYpOWLc9k6CTx9?blocks=hide)
    *
    * Champs obligatoires lors du dépôt d'une demande de changement de puissance [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/rec5efNg0YbGnzFJy?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/rec5efNg0YbGnzFJy?blocks=hide)
    * Appliquer les ratio de changement de puissance du CDC 2022 [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/recdcGTGLqdlHy8Vf?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwgdXRqhQy6K6lzP/recdcGTGLqdlHy8Vf?blocks=hide)
4.  **Identification et création de cartes pour 2 bugs**

    Bug N°1 : Lorsque je suis connecté ETQ PP sur Staging et que je clique sur mon nom en haut de la page Potentiel je suis renvoyé sur Keycloak (CF. PJ) [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/recZPfcGgQJngRlU9?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/recZPfcGgQJngRlU9?blocks=hide) Bug N°2 : Le lien vers le centre des tâches bug et renvoie vers une erreur 404 dans certains cas [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/reczKQhR9U3jmTAAE?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/reczKQhR9U3jmTAAE?blocks=hide)
5. **Support PP**
   * Accès PP Pbq de connexion PP (avec le Bug d’il y a 1 an sur les users déconnectés de leurs projets)
   * Retour PP sur pbq de communication tardive autour d’abandon pour recandidature
   * Ajout email DREAL dans destinataires Newsletter
6. **Maj du guide d’utilisation**
   * La partie transmission d’une preuve de recandidature [https://docs.potentiel.beta.gouv.fr/guide-dutilisation/gestion-de-mon-projet-sur-potentiel/faire-une-demande-sur-potentiel/demande-dabandon-avec-recandidature#id-5.-fourniture-de-la-preuve-de-recandidature-sur-potentiel-1](https://docs.potentiel.beta.gouv.fr/guide-dutilisation/gestion-de-mon-projet-sur-potentiel/faire-une-demande-sur-potentiel/demande-dabandon-avec-recandidature#id-5.-fourniture-de-la-preuve-de-recandidature-sur-potentiel-1)
   * Le centre des tâches [https://docs.potentiel.beta.gouv.fr/guide-dutilisation/gestion-de-mon-projet-sur-potentiel/mettre-a-jour-mon-projet/le-centre-des-taches](https://docs.potentiel.beta.gouv.fr/guide-dutilisation/gestion-de-mon-projet-sur-potentiel/mettre-a-jour-mon-projet/le-centre-des-taches)
   * Maj du temps d’instruction aux demandes [https://docs.potentiel.beta.gouv.fr/nos-realisations-communes/evolution-du-temps-moyen-de-reponse-aux-demandes](https://docs.potentiel.beta.gouv.fr/nos-realisations-communes/evolution-du-temps-moyen-de-reponse-aux-demandes)
7. **Communication - Vœux 2024 en cours**

</details>
