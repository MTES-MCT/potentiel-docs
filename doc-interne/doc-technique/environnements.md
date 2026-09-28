---
description: >-
  Cette page présente les différents environnements sur lesquels l'application
  est hébergée
---

# Environnements

Potentiel est déployé sur différents environnements, qui ont chacun un objectif bien précis

### Local

Cet environnement est réservé à chaque développeur travaillant sur le projet. \
Il permet de faire les développements sur un environnement sans risque d'altérer la donnée.

La base de donnée de cet environnement est falsifié, afin d'éviter l'accès à des vrais données projets en cas de perte / vol de l'ordinateur. À noter qu'en tant qu' e présenter des vrais données projets.

Il dispose d'un système de connexion simplifié qui ne nécessite pas de renseigner de mot de passe mais uniquement une adresse email d'un compte utilisateur pour se connecter avec son compte. cf [Broken link](/broken/pages/BC9yyh9aZL3ZeBoU7hvB "mention")

Pour installer et utiliser cet environnement, il faut suivre [cette documentation](https://github.com/MTES-MCT/potentiel#d%C3%A9veloppement-en-local).



### Development&#x20;

Url d'accès : [https://potentiel-dev.osc-fr1.scalingo.io](https://potentiel-dev.osc-fr1.scalingo.io)

### Demo&#x20;

Url d'accès : [https://potentiel-demo.osc-fr1.scalingo.io](https://potentiel-demo.osc-fr1.scalingo.io)

Cet environnement est dédié à la démonstration de l'outil, que ce soit à des fins commerciales ou démonstratives.&#x20;

La base de donnée de cet environnement est falsifié, afin d'éviter de présenter des vrais données projets.

Il dispose d'un système de connexion simplifié qui ne nécessite pas de renseigner de mot de passe mais uniquement une adresse email d'un compte utilisateur pour se connecter avec son compte. cf [Broken link](/broken/pages/BC9yyh9aZL3ZeBoU7hvB "mention")

Point sur les comptes utilisateurs ici : [https://app.gitbook.com/o/-MK-0FmJqDoeueXN0j8\_/s/-MK-AcePIxK4Pogbnu\_I/\~/changes/978/process-internes/comptes-demo-+-staging](../process-internes/comptes-demo-+-staging.md)

### Staging

Url d'accès : [https://potentiel-staging.osc-fr1.scalingo.io](https://potentiel-staging.osc-fr1.scalingo.io)

Cet environnement sert essentiellement à faire des tests.&#x20;

La base de donnée de cet environnement est falsifié, afin d'éviter de présenter des vrais données projets.

Il dispose d'un système de connexion simplifié qui ne nécessite pas de renseigner de mot de passe mais uniquement une adresse email d'un compte utilisateur pour se connecter avec son compte.

Point sur les comptes utilisateurs ici : [https://app.gitbook.com/o/-MK-0FmJqDoeueXN0j8\_/s/-MK-AcePIxK4Pogbnu\_I/\~/changes/978/process-internes/comptes-demo-+-staging](../process-internes/comptes-demo-+-staging.md)

Lien des fichiers ["Tests métier"](https://drive.google.com/drive/u/0/folders/1bc8piCo2FocqWkMtH3C6Zj-1lKZbSQHz) sur le drive avec un Dashboard global + les fichiers de tests par fonctionnalités

### [Production](https://potentiel.beta.gouv.fr/)

Cet environnement est celui utilisé par nos utilisateurs.&#x20;

Afin de pouvoir se connecter sur cet environnement, il est nécessaire que vous ayez un compte. Pour obtenir celà, il faudra passer par la console de Keycloak (cf [documentation](https://github.com/MTES-MCT/potentiel/blob/master/docs/KEYCLOAK.md)).
