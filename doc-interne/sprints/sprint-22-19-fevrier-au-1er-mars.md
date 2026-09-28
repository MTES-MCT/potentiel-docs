# 🏃‍♂️ Sprint 22 - 19 février au 1er mars

## 🎯 Objectifs

Objectifs du sprint :&#x20;

* Démarrage de la migration des garanties financières
* Création backlog Ops&#x20;



## 🏝️ Absences

* Sylvain du 23 au 26 février
* Hubert du 23 au 26 février
* Mathieu off le mercredi 21 février

## 🔎 Rétrospective

Rétrospective ce jeudi 22 février

Lien vers la rétrospective :

**Actions prises suite à la rétrospective :**&#x20;

* &#x20;

**Bonnes pratiques suite à la rétrospective :** &#x20;

*

## 🎉 Démo

Ordre du jour pour la démo :&#x20;

<details>

<summary>BIZ DEV</summary>

1. **Conception métier**
   * **Changement de puissance liés aux famille**
     * Listing des règles
     * Production d’un CR
     * Echange avec A\&T pour validation de la conception métier
     * Bloquer un changement de puissance en fonction des familles, des AO et Périodes d'appartenance des projets : lister les règles métier [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/rec9Ik3HZ9Qwjb7ID?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/rec9Ik3HZ9Qwjb7ID?blocks=hide)
     * Document CDC par AO & Périodeshttps://docs.google.com/spreadsheets/d/1DjFfO7blksUQLtxp0aNSuOAck4W2ZSlJF8CApWvLNF0/edit#gid=552833603
     * Document de CR [https://docs.google.com/document/d/1hSNBYFZkvDLNkmNTPSSgS1qtAxi\_97efL7lvJQMGxAU/edit](https://docs.google.com/document/d/1hSNBYFZkvDLNkmNTPSSgS1qtAxi_97efL7lvJQMGxAU/edit)
     * Règles Métier CDC 2022 [https://docs.google.com/document/d/1xmNiWTBtMhJWzRi0elSyIRRT3dDsKlRP0rrnwRac93E/edit](https://docs.google.com/document/d/1xmNiWTBtMhJWzRi0elSyIRRT3dDsKlRP0rrnwRac93E/edit)
   * **Modification d’un courrier d’instruction https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwZ5cGuW9v5FJb7B/recGF7xm0oTAnosSi?blocks=hide**&#x20;
2. **Lors du remaniement, le ministère de la Transition énergétique a été supprimé. Le logo et le nom du ministère ont été modifiés et doivent être mis à jour** [https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwqL1BlXOKbon168/recHmYleJ5mwdSk46?blocks=hide](https://airtable.com/apphLwfLi4vad9EAq/tbl8Xmi9jiTVtLxVp/viwqL1BlXOKbon168/recHmYleJ5mwdSk46?blocks=hide)
3.  **Participation au Webinaire Beta.gouv**

    Prez objectifs année 2024 par Beta.Gouv / DINUM

    * Restructuration de BETA / DINUM
    * Bcp d’échecs sur les transferts de SE
    * Utilisation de l’outil Tchap qui remplacera Mattermost
4. **Sécurité**
   * Prise de RDV avec Julien Dauphant, directeur technique de la DINUM
   * RDV Sécurité ⇒ Discussion prévue en raffinage sur les échanges avec Julien Dauphant de BETA et Tristan de la fabrique pour affiner les réponses avec l’équipe DEV
   * 2 meetings avec Tristan
     * Avec toute l’équipe ⇒ Rappel de nos obligations
     * Avec Tiphany ⇒ Explicatif de la méthode à utiliser pour atteindre l’homologation en sécurité
5. **Présentations Potentiel / Fonctionnalités**
   * **Echange DREAL sur la fonctionnalité Abandon**
     * Préparation de l’échange DREAL sur le besoin : export des données dans l’abandon
     * Présentation DREAL de la fonctionnalité ABANDON et recueil des questions et besoins + Debrief pour échange avec Tiphany [https://docs.google.com/document/d/1SfyXXY7iwe5F7-3fExEW2DFRZSbkymyDgRfWtWMWGLo/edit](https://docs.google.com/document/d/1SfyXXY7iwe5F7-3fExEW2DFRZSbkymyDgRfWtWMWGLo/edit)
   * **Guillaume de 4BDD, service budget des EnR**
     * Il a entendu parler de Potentiel, échange avec Violaine et souhaite avoir accès aux stats de la plateforme
     * On lui présente Potentiel d’un point de vue Macro (la prez) puis rapidement une Démo de l’outils ETQ PP, DREAL + Tableau de bord Admin
     * N’a pas besoins d’avoir accès au détail des projets ni aux instructions
     * A besoin d’avoir accès aux données suivantes :
       * Puissance, Tarifs et Date d’achèvement des projets
       * Accès à un outil qui lui donne les résultats ci-dessous en live sans avoir à passer par un intermédiaire (important pour lui)
     * Tiphany va lui envoyer un extrait de l’export pour voir si ça convient, mais il va y manquer la date d’achèvement des projets.
6. **Support**
   * Crisp
   * Email
   * Tél avec Samsolar qui souhaitait savoir si ils pouvaient changer de puissance en étant au-dessus du seuil max de sa Famille d'appartenance
   * Echange avec Tiphany pour gérer plusieurs pbqs d’instruction DREAL
     *   Changement de puissance non autorisé dans la fourchette du CDC mais prévu au CDC :

         _Par dérogation, les modifications à la baisse de la Puissance installée qui seraient imposées soit_

         _par une décision de l’Etat dans le cadre de la procédure d’autorisation mentionnée au 3.3.3 pour_

         _la première période et la troisième période de candidature, ou par une décision de justice_

         _concernant l’autorisation mentionnée au 3.3.3 pour l’ensemble des périodes de candidature, sont_

         _acceptées. Elles doivent faire l’objet d’une information au Préfet." (mention rappelée dans le courrier d'accord)_
     * Bug sur le changement d’actionnaire qui était avant soumis à une instruction DREAL
     * Bug sur la fourchette de changement de puissance d’un projet

</details>
