# Adapter la méthode au type de projet

La démarche reste la même partout (comprendre, concevoir, prototyper, valider
avant de construire). Ce qui change : les méthodes qui pèsent le plus, la forme
des maquettes, les pièges, et les listes de contrôle à appliquer. Lis la
section du projet en cours ; si le projet en mêle plusieurs (une application
mobile avec paiement), combine les sections.

Les listes de contrôle citées (L1, L2…) sont dans `listes-de-controle.md`.
Toutes les sections incluent d'office L1 (avant de coder), L9 (visuel et
règles maison) et L18 (avant de livrer).

## Sommaire

1. Site vitrine, page d'accueil de produit, portfolio
2. Application web : logiciel en ligne, outil métier, tableau de bord
3. Application mobile
4. Commerce en ligne, réservation, paiement
5. Outil interne, back-office, administration
6. Service public, démarche administrative, long formulaire
7. Jeu
8. Application de bureau
9. Produit connecté, objet physique, borne, écran embarqué
10. Interface conversationnelle ou vocale
11. Outil en ligne de commande, outil pour développeurs
12. API, SDK et leur documentation
13. Si le type n'est pas dans la liste

---

## 1. Site vitrine, page d'accueil de produit, portfolio

- **Priorités** : comprendre en cinq secondes ce que c'est, pour qui, et quoi
  faire ensuite ; la confiance ; la vitesse de chargement ; le référencement.
- **Méthodes clés** : veille (concurrents, conventions du secteur), axes de
  positionnement, direction artistique, hiérarchie de la page.
- **Maquettes** : la page entière en HTML statique, téléphone et ordinateur,
  avec les vrais textes ; deux ou trois directions qui diffèrent vraiment
  (structure, ton, image), pas trois teintes de la même.
- **Pièges** : le texte creux (« Des solutions innovantes pour votre
  réussite »), les chiffres et avis inventés, les animations qui retardent la
  lecture, le carrousel en haut de page.
- **Listes** : L2, L3, L5, L7, L8, L10, L11, L12.

## 2. Application web : logiciel en ligne, outil métier, tableau de bord

- **Priorités** : la tâche principale en peu d'étapes ; la densité
  d'information juste ; les états (vide, chargement, erreur) ; la cohérence
  d'un écran à l'autre ; le clavier pour les usages répétés.
- **Méthodes clés** : observation et entretiens (les usages réels diffèrent
  des usages prévus), personas, parcours, architecture de l'information,
  wireframes.
- **Maquettes** : les écrans de la tâche principale, avec données réalistes
  (des noms, montants et dates plausibles, pas « Lorem ipsum »), l'état vide
  du premier jour et un état d'erreur.
- **Pièges** : copier la structure de la base de données dans l'interface ;
  le tableau de bord rempli de chiffres que personne ne regarde ; les
  paramètres partout.
- **Listes** : L2 à L7, L10, L11 ; L8 si l'outil sert aussi sur téléphone.
- **Tableaux de bord** : une question par graphique ; le chiffre le plus
  important en premier ; la comparaison qui donne du sens (par rapport à
  quoi ?) ; pas de graphique circulaire au-delà de quelques parts.

## 3. Application mobile

- **Priorités** : le pouce (zones atteignables, cibles d'au moins 44 à 48
  points), la lecture en mouvement, les interruptions (appel, perte de
  réseau), les conventions de la plateforme, les notifications utiles et
  rares.
- **Méthodes clés** : parcours (avant, pendant, après, souvent hors de
  l'application), observation en contexte réel, preuve de concept si une
  fonction du téléphone est en jeu (caméra, localisation, paiement).
- **Maquettes** : écrans à la taille d'un téléphone (390 × 844 par exemple),
  avec la barre de navigation réelle ; pour une application native, respecter
  les guides d'Apple (Human Interface Guidelines) et de Google (Material
  Design) plutôt que d'inventer des composants.
- **Pièges** : réduire un site d'ordinateur ; demander toutes les
  permissions au premier lancement ; l'écran d'accueil en cinq diapositives
  avant de pouvoir faire quoi que ce soit.
- **Listes** : L2 à L8, L10, L11, L12.

## 4. Commerce en ligne, réservation, paiement

- **Priorités** : la confiance (prix total clair, frais visibles tôt,
  conditions d'annulation), un tunnel court, la commande sans compte, la
  récupération d'erreur de paiement, la confirmation rassurante.
- **Méthodes clés** : parcours détaillé du tunnel (chaque abandon est une
  rupture), entretiens sur les hésitations d'achat, veille des concurrents.
- **Maquettes** : chaque étape du tunnel, plus l'erreur de carte refusée et
  la page de confirmation.
- **Pièges** : les pièges commerciaux (case précochée, compte à rebours
  factice, désinscription cachée), les frais qui apparaissent à la dernière
  étape.
- **Listes** : L3, L4, L5, L6, L7, L8, L11 (en entier), L12.

## 5. Outil interne, back-office, administration

- **Priorités** : la productivité des usages répétés, l'efficacité au
  clavier, la recherche et les filtres, les actions groupées, la prévention
  des erreurs coûteuses (confirmation, annulation possible), la traçabilité.
- **Méthodes clés** : observer les gens au travail (contournements, fichiers
  à côté, post-it) ; cartographie des parties prenantes (qui dépend des
  données saisies ici ?).
- **Maquettes** : écrans denses mais ordonnés, avec de vraies quantités de
  données (cent lignes, pas trois).
- **Pièges** : croire que « c'est interne, l'ergonomie compte moins » ; une
  minute perdue cent fois par jour coûte cher.
- **Listes** : L2 à L7, L10, L11 (journal des actions, droits).

## 6. Service public, démarche administrative, long formulaire

- **Priorités** : la langue simple, l'accessibilité exigée par la loi
  (en France, le RGAA, aligné sur les WCAG), une question par écran pour les
  démarches complexes, l'enregistrement en cours de route, la liste des
  pièces à préparer avant de commencer.
- **Méthodes clés** : entretiens avec des publics variés (âgés, éloignés du
  numérique, en situation de handicap), parcours de bout en bout (y compris
  le courrier et le guichet).
- **Maquettes** : chaque étape, l'écran de récapitulatif et celui de fin
  (« et maintenant ? »). Les systèmes de design publics existent : en France,
  le Système de Design de l'État (DSFR) ; s'il s'applique, utilise-le.
- **Pièges** : le jargon administratif, les sigles, les délais d'expiration
  de session silencieux.
- **Listes** : L2 à L7 (L7 en entier), L8, L11, L12.

## 7. Jeu

- **Priorités** : comprendre la règle en jouant, la difficulté juste et
  équitable, le retour immédiat de chaque geste, la pause, le son coupé par
  défaut là où on joue en public, l'accessibilité (couleurs, mouvement,
  commandes).
- **Méthodes clés** : test de jeu le plus tôt possible (un prototype brut vaut
  mieux qu'une maquette), parcours d'une partie (avant, pendant, après),
  personas de joueurs (occasionnel, compétitif).
- **Maquettes** : l'écran de départ, une partie en cours, la fin de partie,
  dans la plus petite fenêtre visée ; puis un prototype jouable.
- **Pièges** : l'écran de départ trop chargé qui cache le bouton « Jouer » sur
  un petit écran ; la perte qui paraît injuste ; une information vitale (vies,
  temps) qu'on ne voit pas en jouant.
- **Listes** : L3, L5, L6, L7, L8, L10, L16.

## 8. Application de bureau

- **Priorités** : les conventions du système (menus, raccourcis, fenêtres
  redimensionnables, glisser-déposer), le travail long et le multi-fenêtres,
  l'enregistrement et l'annulation.
- **Maquettes** : à plusieurs tailles de fenêtre, avec le menu et les
  raccourcis affichés.
- **Pièges** : une interface web posée telle quelle dans une fenêtre, sans
  raccourcis ni menus.
- **Listes** : L2 à L7, L10, L12.

## 9. Produit connecté, objet physique, borne, écran embarqué

- **Priorités** : le contexte d'usage physique (lumière, bruit, gants, debout,
  pressé), le retour multisensoriel (son, vibration, lumière), l'état visible
  de l'objet, la panne et la reprise, l'installation.
- **Méthodes clés** : ethnographie sur le lieu d'usage, maquette tangible et
  preuve de concept (voir `methode-3-prototyper.md`), design fiction pour un
  usage nouveau.
- **Maquettes** : storyboard d'usage, schéma des états de l'objet, maquette
  de l'écran à sa taille et à sa distance de lecture réelles.
- **Pièges** : un écran tactile minuscule pour une tâche fréquente ; un objet
  dont on ne sait pas s'il est allumé, connecté ou en panne.
- **Listes** : L5, L6, L7, L11, L17.

## 10. Interface conversationnelle ou vocale

- **Priorités** : dire ce que l'assistant sait faire, comprendre les
  formulations variées, confirmer avant une action importante, rattraper
  l'incompréhension avec élégance, laisser parler à un humain.
- **Méthodes clés** : entretiens et collecte des vraies formulations, parcours
  par intention, scénarios de dialogue incluant les échecs.
- **Maquettes** : des scripts de dialogue (chemin nominal, incompréhension,
  hors sujet, annulation), pas des écrans.
- **Pièges** : la fausse personnalité envahissante, les réponses trop longues
  à l'oral, l'impasse sans sortie.
- **Listes** : L5, L6, L11, L15.

## 11. Outil en ligne de commande, outil pour développeurs

- **Priorités** : une aide claire (`--help`), des noms de commandes et
  d'options prévisibles, des erreurs qui disent quoi faire, des codes de
  sortie corrects, un affichage lisible par un humain et exploitable par un
  script (option de sortie JSON), la confirmation des actions destructrices,
  la progression des tâches longues.
- **Méthodes clés** : observation (lire les scripts et les historiques des
  utilisateurs), veille des conventions (POSIX, GNU, guides publiés comme
  « Command Line Interface Guidelines »), architecture des commandes.
- **Maquettes** : des transcriptions de terminal (ce que l'on tape, ce qui
  s'affiche), pour le cas nominal, l'erreur et l'aide.
- **Pièges** : des couleurs comme seule information, l'absence de mode non
  interactif, des messages illisibles dans un fichier de journal.
- **Listes** : L5, L6, L11, L13.

## 12. API, SDK et leur documentation

- **Priorités** : le premier appel réussi en quelques minutes, des noms
  cohérents, des erreurs explicites et stables, des exemples copiables, la
  gestion des versions et des changements cassants.
- **Méthodes clés** : persona du développeur (débutant, intégrateur pressé,
  expert), parcours « de la découverte au premier appel en production »,
  architecture de l'information de la documentation.
- **Maquettes** : exemples de requêtes et de réponses, y compris d'erreur, et
  la page « démarrer » de la documentation.
- **Listes** : L5, L6, L11, L14.

## 13. Si le type n'est pas dans la liste

Pose-toi les questions qui différencient les sections ci-dessus : sur quel
support, dans quel contexte physique, à quelle fréquence, avec quel niveau
d'expertise, et quelle est la tâche dont tout dépend ? Prends la section la
plus proche, et dis à l'utilisateur ce que tu as transposé.
