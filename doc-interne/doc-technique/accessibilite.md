# Accessibilité

## Intro

* 1/4 des 15-64 ans sont en situation de handicap au sans large
* 85% des handicaps surviennent au cours de la vie
* Un handicap peut être lié au contexte (diff avec une déficience) : permament, temporaire, situationnel
* Handicap visuel (4,3% de la population active) : alternatives textuelles, mise en page redimensionnage, repères visuels, contrasts, navigation au clavier
* Auditif : contenu audio avec sous-titre
* Moteur : navigation au clavier, limite de temps pour accomplir des tâches
* Cognitif : navigation facile, phrase et mots simples, contenu sonores désactivables

[https://fr.wikipedia.org/wiki/Facile\_%C3%A0\_lire\_et\_%C3%A0\_comprendre](https://fr.wikipedia.org/wiki/Facile_%C3%A0_lire_et_%C3%A0_comprendre)

* Accessibilité numérique : droit fondamental

## Obligations légales

Obligation légale >> transparence sur l'accessibilité PUIS se mettre en conformité (test, audits…)

* Afficher sur la page d'accueil l'état d'accessibilité du site ou du service : totalement conforme : tx accessibilité 100%, partiellement confirme : tx accessibilité 50%, non conforme : < 50% ou taux non connu
* Publier une déclaration d'accessibilité donnant + de détails sur l'état d'accessibilité, donner les engagements >> document formel, structure à respecter à mettre en lien sur la page d'accueil
* Mise en conformité en 2020 pour les site du secteur public, appr mobiles et progiciels du secteur public en juin 2021
* Risque : 20 000 € d'amende par site ou app / année
* Le taux de conformité est juste un outil législatif, mais n'est pas l'accessibilité réelle

### Calcul du tx d'accessibilité

* Reco du WCAG : non obligatoires
* Chaque pays créé son référentiel, en France c'est le RGAA, reco françaises traduires en terle de lois (Réferentiel Général de l'Accessibilité pour les Administrations)
* RGAA : 106 critères retroupés en thématiques
  * 3 tests/critère, chaque test fait sur plusieurs pages
  * un test échoue >> le critère sera jugé non conforme
  * seulement 25% des tests sont automatisables
* Outils beta.gouv  : [https://dashlord.incubateur.net/#/](https://dashlord.incubateur.net/#/)
* Autre outils : lighthouse, axe, ANDI (plugin d'accessibilité), heading maps, wave
* Passe par un audit (parun cabinet externe) - environ 4000€ pour un site beta.gouv
* Utilisation du design system de l'Etat : points gagnés ??

## 10 choses à vérifier facilement sans compétences technique

* Titre des pages (balise title) : permet de se situer parmi les onglets (notamment avec un lecteur d'écran), utile pour les moteurs de recherche
  * pertinent
  * descriptif
  * différenciant (mot diff en premier pour être visible dans la barre d'onglet)
* Alternatives textuelles :
  * Permettre de comprendre le contenu (pas nécessaire de décrire l'image)
    * ex : 'recherche' plutôt que 'loupe'
  * Pas d'alt pour les images purement décoratives
* Hiérarchie de l'information (titres) :
  * Pour la navigation avec un lecteur d'écran pour survoler les titres
* Contrastes :&#x20;
  * Les couleurs ne doivent pas entraver la lecture
  * Texte blanc sur image : mettre un fond de couleur par défaut si l'image ne s'affiche pas pour rendre le texte lisible
* Personnalisation du texte (couleur, taille, police, interlignes…) :
  * Tester ce qu'il se passe quand on zoom à 200 ou 300% : vérifier que tous les textes sont agrandis, pas de texte coupé ou rogné, pas de chevauchement, formulaire utilisables, défilement horizontal non nécessaire pour lire le contenu
* Interface utilisable sans souris (clavier ou saisie vocale)
  * Tester la navigation au clavier :
    * focus visible à la navigation avec tab
    * ordre de navigation logique
    * tous les éléments interactifs sont accessibles
    * le focus ne reste pas coincé (dans une modale)
* Formulaires :
  * Utilisation des bonnes balises
  * Messages d'aide
  * Navigation au clavier
  * Les champs ont un label (et un clic sur le label active le champ)
  * Champs obligatoires indiqués (mention avec du texte et pas seulement du rouge)
  * Instructions avant le champ concerné
  * Préciser le format attendu si format spécifique (ex : date) dans le label
  * Les erreurs sont explicites (expliquer comment corriger), ex : si email mal rempli dans l'erreur donner un exemple de format attendu, préciser quel champ est concerné
* Contenus animés :
  * Contrôle du contenu en mouvement, le mettre en pause ou le cacher (exemple un carrousel)
  * Attention aux contenus clignotants
    * ex de cas : pub pour les JO de Londres avec effets clignotants >> plusieurs personnes dans le coma en Angleterre
* Info mises à jour automatiquement (ex : meteo, commentaires) : limiter la fréquence pour éviter d'avoir un effet declignotement, possibilité de limiter le nombre de mises à jour
* Audio / vidéo :
  * Sous-titrer les contenus audio/vidéo (transcript ou audio description)
  * Le son ne démarre pas seul
  * Info audio accessibles au clavier
* Structure des pages :
  * Site clair si styles désactivés ?

## Ressources&#x20;

* Beta.gouv : programme Acces, channel #domaine-accessibilité , kit accessibilité sur la doc de beta.gouv,
* fiches métier sur le site design.gouv,
* notices AccedeWeb,
* &#x20;design-accessible.fs (dédié aux designers)
* Kit accessibilité beta :
  * Accélération : [https://doc.incubateur.net/communaute/gerer-sa-startup-detat-ou-de-territoires-au-quotidien/jameliore-le-design-et-lexperience-utilisateur/accessibilite-et-rgaa/kit-accessibilite/acceleration#mettre-en-place-des-tests-automatiques](https://doc.incubateur.net/communaute/gerer-sa-startup-detat-ou-de-territoires-au-quotidien/jameliore-le-design-et-lexperience-utilisateur/accessibilite-et-rgaa/kit-accessibilite/acceleration#mettre-en-place-des-tests-automatiques)
  * consolidation : [https://doc.incubateur.net/communaute/gerer-sa-startup-detat-ou-de-territoires-au-quotidien/jameliore-le-design-et-lexperience-utilisateur/accessibilite-et-rgaa/kit-accessibilite/consolidation#tester-avec-des-utilisateurs-en-situation-de-handicap](https://doc.incubateur.net/communaute/gerer-sa-startup-detat-ou-de-territoires-au-quotidien/jameliore-le-design-et-lexperience-utilisateur/accessibilite-et-rgaa/kit-accessibilite/consolidation#tester-avec-des-utilisateurs-en-situation-de-handicap)
* Support de la formation : [https://docs.google.com/presentation/d/1J4r6-ayWmsBBJSDVMjS3oYmY1Hjkg16LfxfcfuASJ4w/edit#slide=id.gf24780b7b6\_0\_59](https://docs.google.com/presentation/d/1J4r6-ayWmsBBJSDVMjS3oYmY1Hjkg16LfxfcfuASJ4w/edit#slide=id.gf24780b7b6_0_59)
* Ressources pour les devs :&#x20;
  * Outil qui permet d'évaluer son niveau d'accessibilité : [https://wave.webaim.org/](https://wave.webaim.org/)
  * Package estlint qui permet de mettre en place des règles d'accessibilité pour lever des alertes ou des erreurs pendant la phase de codage : [https://github.com/jsx-eslint/eslint-plugin-jsx-a11y#readme](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y#readme)
  * CI mis en place par lighthouse pour automatiser la génération de rapport : [https://github.com/GoogleChrome/lighthouse-ci](https://github.com/GoogleChrome/lighthouse-ci)

&#x20;
