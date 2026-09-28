# Faire des requêtes Metabase

## Recherche dans un json

* S'il y a des apostrophes dans la champ recherché il faut l'échapper avec un `'`&#x20;
  * ex : `"details"->>'Numéro de l''autorisation d''urbanisme' as "autorisation-urbanisme"`

## Manipuler des dates

* Passer d'un timestamp à une date : \`CAST(to\_timestamp(("valueDate" / 1000)) AS date)\`

## Faire des requêtes sur les données d'utilisation

Table [sur ce lien](https://metabase.potentiel.beta.gouv.fr/question#eyJkYXRhc2V0X3F1ZXJ5Ijp7InR5cGUiOiJuYXRpdmUiLCJuYXRpdmUiOnsicXVlcnkiOiJzZWxlY3QgKiBmcm9tIFwic3RhdGlzdGlxdWVzVXRpbGlzYXRpb25cIjsiLCJ0ZW1wbGF0ZS10YWdzIjp7fX0sImRhdGFiYXNlIjoyfSwiZGlzcGxheSI6InRhYmxlIiwicGFyYW1ldGVycyI6W10sInZpc3VhbGl6YXRpb25fc2V0dGluZ3MiOnt9fQ==)

Type de données : 'projetConsulté', 'connexionUtilisateur'. Ex dans la requête : `where type = 'connexionUtilisateur'`

Pour avoir des stats en fonction de la date il faut utiliser la fonction `DATE`. Par exemple : `where date > DATE('2022-11-20')`

Pour accéder aux `données` de la statistique (le rôle de l'utilisateur par exemple) : `données->'utilisateur'->>'role'`

Pour le type 'projetConsulté' on a des détails sur le projet dans données > projet > AppelOffreId, FamilleId, PériodeId ... Ex : `données->'projet'->>'appelOffreId'` par exemple.
