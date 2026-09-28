---
description: Ce document fait suite à un atelier d'équipe qui a eu lieu le 18 Avril 2024.
---

# 📔 Guide d'utilisation de Linear

### Structures et utilisation des différents éléments de Linear

_Cette section permet de mieux comprendre les différents étapes du découpage d'un projet et de mieux organiser Linear et le backlog_&#x20;

#### Projects = Epic

Définition et attributs

Les **projects** ou **epics** représentent des zones ou périmètres métier de l'application. Ce sont les zones fonctionnelles de Potentiel.&#x20;

Ces éléments vivent toujours et n'ont pas de dates de péremption. On y rattachera les fonctionnalités qui ont un impact sur ces différentes zones.&#x20;

_<mark style="color:green;">Exemple : L’abandon d’un projet lauréat</mark>_

#### Milestones = Features

Définition et attributs

&#x20;Il s'agit d'une fonctionnalité, d'un morceau du projet scopé et qui a un but.

Un milestone est borné, on a des éléments identifiés qui nous permettent de savoir quand son développement est complet (actions et conséquences associées).

Au milestone doit être associé une conception métier et un document dit de discovery contenant les définitions et les règles métier associées à la fonctionnalité.

De ce fait un milestone peut aussi être délimité dans le temps en terme de développement (rétroplanning possible).&#x20;

_<mark style="color:green;">Exemple : Demander un abandon</mark>_

#### Issues = User story&#x20;

Définition et attributs&#x20;

Ce sont des éléments fonctionnels qui composent le milestone et qui sont assez petits pour être livrés en prod sur un sprint.&#x20;

Au niveau des issues, on retrouve les comportements fonctionnels décrits dans les critères d'acceptation&#x20;

_<mark style="color:green;">Exemple : demander un abandon sans recandidature; notifier un utilisateur; ..</mark>_&#x20;

#### Tasks = Tâches techniques&#x20;

Définition et attributs

Les tâches techniques correspondent à un découpage de tâches nécéssaire au développement de l'issue. Il s'agit d'un espace dédié aux équipes techniques.

_<mark style="color:green;">Exemple : créer une query de récupération de données; tâches de cleaning; ..</mark>_



### Etapes du process de conception et de delivery&#x20;

#### **1. Backlog**

C'est une boîte à idées non étudiées et non priorisées. Toute l'équipe à accès au backlog et peut créer des élements.&#x20;

Une carte du backlog doit être compréhensible : le contexte, le besoin utilisateur et l'impact sont exprimés.&#x20;

#### **2. Conception métier**

Une carte passe en conception métier lorsqu'elle est priorisée par les équipes métier (idéalement à 1 ou 2 sprint/s de son dévelopement).&#x20;

L'étape pendant laquelle on passe du besoin à la solution fonctionnelle qui répondra au besoin exprimé grâce aux éléments réunis (itw utilisateurs, cahier des charge, ...).&#x20;

Cette étape peut prendre la forme d'atelier et d'itérations entre les équipes métier avec un soutien tech en ce qui concerne la faisabilité.&#x20;

On considère l'étape terminée une fois que toute l'équipe est alignée sur la solution, que celle-ci est découpée si besoin, avec les critères d'acceptation définis.&#x20;

#### **3. Raffinage**

_Le raffinage est une étape optionnelle, utile sur des stories plus complexes._&#x20;

Il s'agit d'un temps d'échange métier et tech qui permet un alignement final sur les cartes (solution et stories prêtes à être dev). &#x20;

#### **4. Conception tech**&#x20;

_La conception tech est optionnelle._&#x20;

Il s'agit de l'étape pendant laquelle les équipes techniques réflechissent au plan pour développer la solution.&#x20;

Cette étape permet d'ouvrir une discussion en équipe et de se mettre d'accord sur la solution technique choisie. Le résultat de cette discussion est ajouté sur la carte de la story.&#x20;

#### **5. Prêt à dev**&#x20;

Il s'agit d'un sas d'attente des stories qui sont prêtes à être développées.&#x20;

_A noter que nous allons créer une checklist pour s'assurer que tous les éléments nécéssaires sont présents dans la carte._&#x20;

#### 6. In progress

La carte est en cours de développement.&#x20;

Une carte dans cette colonne doit être assignée à une personne de l'équipe tech.&#x20;

#### 7.  To review&#x20;

Le code est prête à être revu et challenger par un autre dev.&#x20;

#### 8.  Done&#x20;

Le code est finit et sur stagging.&#x20;

#### 9.  To test

Il s'agit de l'étape de test du développement.&#x20;

_A définir qui à le rôle de testeur._&#x20;

#### 10. To release

Prête à être mis en production.&#x20;

#### 11. Delivered &#x20;

### Annexe - document de support de l'atelier&#x20;

{% file src="../../.gitbook/assets/Atelier Linear.pdf" %}
