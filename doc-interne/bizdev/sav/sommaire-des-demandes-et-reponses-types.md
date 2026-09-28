# Sommaire des demandes et réponses types

### [Aller à : User DREAL](sommaire-des-demandes-et-reponses-types.md#user-dreal)

### [Aller à : User Porteur de projet](sommaire-des-demandes-et-reponses-types.md#user-porteur-de-projet)

## <mark style="color:green;">Users (tous personas)</mark>

#### :interrobang:<mark style="color:yellow;">J'ai reçu un lien d'invitation mais je n'ai pas activé mon compte dans les temps (30 jours)</mark>

* Si le lien reçu par email n'est plus utilisable, l'utilisateur doit se rendre directement dans Potentiel > "m'identifier" > "mot de passe oublié" pour créer son mot de passe
* Si l'utilisateur ne reçoit pas le mail de réinitialisation du mot de passe
  * Regarder dans mailjet si le mail a été délivré, si oui inviter l'utilisateur à regarder ses spams, les bien dérouler les mails reçus (dans une seule "conversation" sur gmail)
  * Demander à un développeur de vérifier si l'utilisateur a validé son email depuis la console admin de Keycloak. Le cas échéant on peut valider l'email directement depuis cette console admin.
  * En dernier recours demander à un dev de lui créer un mot de passe temporaire depuis la console keycloak (cocher la case "temporary" ainsi l'utilisateur devra changer son mot de passe à sa première connexion)



#### &#x20;

## <mark style="color:green;">User DREAL</mark>

Messages & réponses types

| Problème                                                                                                                                                                              | Actions préalables                                                                                                                                                          | Réponse(s) à apporter                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| [Je ne sais pas comment m'inscrire sur Potentiel](sommaire-des-demandes-et-reponses-types.md#je-ne-sais-pas-comment-minscrire-sur-potentiel-en-tant-que-dreal)                        |                                                                                                                                                                             | Nous prenons en charge l'inscription depuis notre espace "Admin"                                                                   |
| [Mon compte a un accès "porteur de projet", comment le modifier ? ](sommaire-des-demandes-et-reponses-types.md#mon-compte-potentiel-a-un-acces-porteur-de-projet-comment-le-modifier) | <ul><li>Vérifier l'origine de l'inscription (en autonomie ou via intervention de l'équipe Potentiel ?)</li><li>Modifier la catégorie de ses accès (de PP à DREAL)</li></ul> | <ul><li>Lui redemander par mail de se déconnecter puis de se reconnecter afin que les changements soient pris en compte.</li></ul> |

#### :interrobang:<mark style="color:yellow;">Je ne sais pas comment m'inscrire sur Potentiel</mark>&#x20;



#### :interrobang:<mark style="color:yellow;">Mon compte Potentiel a un accès "porteur de projet", comment le modifier ?</mark>

1. Si le contact s'est inscrit au préalable depuis l'URL  : [https://auth.potentiel.beta.gouv.fr/auth/realms/Potentiel/login-actions/registration?client\_id=potentiel-web\&tab\_id=zwOGzCvLX9M](https://auth.potentiel.beta.gouv.fr/auth/realms/Potentiel/login-actions/registration?client_id=potentiel-web\&tab_id=zwOGzCvLX9M)
2. Basculer ses accès de " porteur de projets " à " DREAL " depuis [https://staging.potentiel.incubateur.net/](https://staging.potentiel.incubateur.net/)
3. Lui redemander par mail de se déconnecter puis de se reconnecter afin que les changements soient pris en compte.

## <mark style="color:green;">User Porteur de projet</mark>

Messages & réponses types

| Problème                                                                                                                                                                                  | Actions préalables                                                                                                                                                 | Réponse(s) à apporter                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Mentions manquantes ("IP" ou "FP")](sommaire-des-demandes-et-reponses-types.md#il-ny-a-pas-la-mention-financement-ou-investissement-participatif-sur-mon-projet.)                        | <ul><li>Ecrire un mail à la CRE </li></ul>                                                                                                                         | <ul><li>Confirmer la modification effectuée sur son compte Potentiel</li><li>Infirmer</li></ul>                                                                                                                                                           |
| [Pas d'accès au compte suite  changement de producteur ](sommaire-des-demandes-et-reponses-types.md#je-suis-le-nouveau-producteur-du-projet-mais-je-nai-pas-acces-au-projet)              | <ul><li>Vérifier : nom du projet / adresse mail / nom du représentant légal </li><li>(Ecrire à la DREAL concernée)</li></ul>                                       | <ul><li>Modifier les accès depuis le compte Admin</li></ul>                                                                                                                                                                                               |
| Pas d'accès à mon projet                                                                                                                                                                  | <ul><li>Vérifier : nom du projet / adresse mail / nom du représentant légal</li><li>Chercher le projet dans la barre de recherche "Projets" de Potentiel</li></ul> | <ul><li>Si le projet n'apparait toujours pas malgré les informations ci-contre + le n°CRE ou le prix --> vérifier si le projet ne fait pas partie des projets historiques (CRE4) non importés. </li><li>Si oui, se rapprocher de Julie Beelmeon</li></ul> |
| [Suis-je obligé.e de remplir les étapes du projet sur Potentiel ?](sommaire-des-demandes-et-reponses-types.md#suis-je-oblige.e-de-remplir-les-etapes-du-projet-sur-potentiel)             |                                                                                                                                                                    | <ul><li>Répondre le texte ci-dessous</li></ul>                                                                                                                                                                                                            |
| [Je ne retrouve pas mon projet avec le n° CRE, le tarif ou le nom du projet](sommaire-des-demandes-et-reponses-types.md#suis-je-oblige.e-de-remplir-les-etapes-du-projet-sur-potentiel-1) | <ul><li>Vérifier si les informations fournies sont correctes</li><li>Si correctes, chercher le n° d'identifiant du projet dans Potentiel</li></ul>                 | <ul><li>Communiquer par mail au PP le lien direct du projet (contenant l'identifiant)</li></ul>                                                                                                                                                           |

#### :interrobang:<mark style="color:yellow;">Il n'y a pas la mention "Financement" ou "Investissement Participatif" sur mon projet.</mark>

TO DO :&#x20;

1. Ecrire un mail à la CRE pour savoir si la pièce "FP" ou "IP" figure bien dans le projet.
2. Si oui, effectuer les modifications manuelles dans Potentiel (si peu de projets) ou par réimport (si nombreux projets à importer)\
   2.2. Faire la modification dans Potentiel et répondre au porteur :

> _" Bonjour Monsieur / Madame XXXX,_&#x20;
>
> _Après vérifications des pièces de votre dossier, nous vous confirmons que la mention FP ou IP y figure bien. Par conséquent, nous avons fait la modification sur votre compte Potentiel afin qu'elle apparaisse dès à présent._
>
> _Bien cordialement,_
>
> _L'équipe Potentiel"._

3\. Si non, répondre au porteur de projet :&#x20;

> _Bonjour Monsieur / Madame XXXX,_&#x20;
>
> _Après vérifications des pièces de votre dossier, la mention FP ou IP ne peut être apposée._\
> _Si vous le souhaitez, nous vous invitons à faire une demande de recours depuis votre projet concerné._
>
> _Bien cordialement,_
>
> _L'équipe Potentiel"._



#### :interrobang:<mark style="color:yellow;">Je suis le nouveau producteur du projet mais je n'ai pas accès au projet</mark>&#x20;

1. S'assurer que le changement a eu lieu avant de donner accès\
   \> Demander au nouveau producteur l'adresse mail à changer \
   \>Demander au porteur le nom du nouveau représentant légal&#x20;
2. Si besoin : faire une demande de vérification auprès de la DREAL concernée

#### :interrobang:<mark style="color:yellow;">Suis-je obligé.e de remplir les étapes du projet sur Potentiel ?</mark>

_L'utilisation de la plateforme Potentiel n'est pas imposée pour l'ensemble des étapes du projet, seulement celles prévues par les cahiers des charges. Cependant, en passant par Potentiel vous vous assurez que le traitement de vos demandes est simplifié, vous facilitez effectivement le suivi de vos projets par l'administration, et bientôt par d'autres acteurs impliqués dans la vie des projets._

#### :interrobang:<mark style="color:yellow;">Je ne retrouve pas mon projet avec le n° CRE, le tarif ou le nom du projet</mark>

_Bonjour, je vous partage ici les liens vers les 2 projets concernés (contenant leur identifiant sur Potentiel) :_ \
\
_https://potentiel.beta.gouv.fr/projet/ (identifiant Potentiel)_

_Pouvez-vous me confirmer que cela fonctionne et que vous retrouvez bien vos projets dans votre portail porteur de projets ?_\
\
_Cordialement,_

