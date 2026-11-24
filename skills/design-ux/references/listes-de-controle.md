# Listes de contrôle

Chaque point se vérifie par oui ou non. Rends les listes en cases à cocher
`- [ ]`. Ne prends que celles qui s'appliquent au projet (voir
`adapter-au-projet.md`), et adapte un point plutôt que de le garder tel quel
s'il ne colle pas. Quand un point n'est pas conforme, dis où (écran, fichier
et ligne) et ce qu'il faut changer.

## Sommaire

- L1 Avant de coder
- L2 Structure et navigation
- L3 Action principale et hiérarchie
- L4 Formulaires et saisie
- L5 Textes et microcopie
- L6 États de l'interface
- L7 Accessibilité
- L8 Mobile et tactile
- L9 Visuel, cohérence et règles maison
- L10 Performance ressentie
- L11 Confiance, vie privée et éthique
- L12 Langues, formats et international
- L13 Outil en ligne de commande
- L14 API et documentation
- L15 Interface conversationnelle ou vocale
- L16 Jeu
- L17 Objet connecté et interface physique
- L18 Avant de livrer

---

## L1 Avant de coder

- [ ] On sait pour qui on conçoit (persona, même provisoire) et quelle tâche compte le plus.
- [ ] Le parcours actuel ou prévu est écrit, avec ses ruptures.
- [ ] Deux ou trois options ont été proposées en maquette.
- [ ] Une option a été validée explicitement par l'utilisateur.
- [ ] Les textes de la maquette sont les vrais textes, pas des faux textes.
- [ ] Les états importants (vide, chargement, erreur, succès) sont maquettés.
- [ ] Les hypothèses non vérifiées sont écrites comme telles.
- [ ] Le projet a ses règles propres (charte, système de design) et elles ont été lues.

## L2 Structure et navigation

- [ ] On sait toujours où l'on est (titre de page, élément de navigation actif).
- [ ] On peut revenir en arrière sans perdre ce qu'on a saisi.
- [ ] Les libellés de navigation sont les mots des utilisateurs, pas ceux de l'équipe.
- [ ] Les entrées de navigation principales sont peu nombreuses (sept au plus, idéalement moins).
- [ ] Le même élément porte le même nom partout.
- [ ] Un lien ressemble à un lien, un bouton à un bouton.
- [ ] Les adresses (URL) sont lisibles et partageables, et le bouton Retour du navigateur marche.
- [ ] Une page introuvable propose un chemin pour repartir.
- [ ] La recherche existe dès qu'il y a beaucoup de contenu.

## L3 Action principale et hiérarchie

- [ ] Chaque écran a une seule action principale, visible sans faire défiler.
- [ ] L'action principale se distingue nettement des actions secondaires.
- [ ] Les actions destructrices sont séparées et identifiables.
- [ ] Le libellé d'un bouton dit ce qu'il fait (« Réserver le créneau », pas « Valider » ni « Envoyer »).
- [ ] L'ordre de lecture suit l'ordre d'importance.
- [ ] Rien d'essentiel n'est caché dans un menu « plus » ou un survol.
- [ ] Il n'y a pas deux éléments qui se disputent l'attention au même endroit.

## L4 Formulaires et saisie

- [ ] Chaque champ a une étiquette visible, qui reste quand on tape (pas seulement un texte indicatif dans le champ).
- [ ] On ne demande que ce qui sert vraiment, et on dit pourquoi pour ce qui surprend.
- [ ] Les champs obligatoires ou facultatifs sont signalés de façon cohérente.
- [ ] Le type de clavier correspond au champ (courriel, téléphone, nombre).
- [ ] Le remplissage automatique du navigateur fonctionne (attributs `autocomplete`).
- [ ] Le format attendu est indiqué avant l'erreur, pas après.
- [ ] Les erreurs s'affichent à côté du champ, disent quoi faire, et ne vident pas le formulaire.
- [ ] Le bouton d'envoi montre qu'il travaille et ne peut pas être cliqué deux fois.
- [ ] Un long formulaire est découpé en étapes, avec la progression visible.
- [ ] On peut coller dans les champs, y compris le mot de passe.
- [ ] On peut afficher le mot de passe saisi.

## L5 Textes et microcopie

- [ ] Les phrases sont courtes, au présent, à la voix active.
- [ ] On parle à l'utilisateur de ses objectifs, pas du fonctionnement interne.
- [ ] Aucun jargon technique ni sigle non expliqué.
- [ ] Les titres disent ce qu'on trouve ou fait sur la page.
- [ ] Les messages d'erreur disent ce qui s'est passé et comment s'en sortir, sans accuser.
- [ ] Les messages de succès disent ce qui a été fait et ce qui suit.
- [ ] Le ton est le même partout (tutoiement ou vouvoiement, registre).
- [ ] Pas de point d'exclamation à chaque phrase, pas de fausse familiarité.
- [ ] Les chiffres, dates et montants sont écrits de façon lisible.
- [ ] Aucun texte de remplissage ni texte inventé présenté comme réel (avis, chiffres).

## L6 États de l'interface

- [ ] **Vide** : le premier jour, l'écran explique quoi faire et propose l'action.
- [ ] **Chargement** : l'attente est signalée ; au-delà d'une seconde, un indicateur ; au-delà de dix, une progression ou une explication.
- [ ] **Erreur** : chaque erreur possible a un message et une issue (réessayer, corriger, contacter).
- [ ] **Hors ligne** ou réseau lent : l'interface le dit et ne perd pas les données.
- [ ] **Succès** : une confirmation visible, à l'endroit où l'on regarde.
- [ ] **Partiel** : un contenu qui manque (image, nom) ne casse pas la mise en page.
- [ ] **Beaucoup de données** : listes longues, noms très longs, montants énormes restent lisibles.
- [ ] **Droits** : ce qu'on ne peut pas faire est expliqué, pas juste grisé sans raison.
- [ ] Une action importante peut être annulée, ou demande confirmation si elle ne le peut pas.

## L7 Accessibilité

Référence : WCAG 2.2 niveau AA (en France, le RGAA s'appuie dessus).

- [ ] Contraste du texte d'au moins 4,5:1 (3:1 pour le gros texte et les éléments d'interface).
- [ ] Tout se fait au clavier, dans un ordre logique, avec le focus toujours visible.
- [ ] Les images utiles ont un texte de remplacement ; les décoratives sont ignorées.
- [ ] Les boutons et liens ont un nom accessible, y compris les boutons à icône seule.
- [ ] La couleur n'est jamais la seule façon de transmettre une information.
- [ ] La structure utilise de vrais titres, listes, régions et éléments de formulaire.
- [ ] Les messages qui apparaissent (erreur, succès) sont annoncés aux lecteurs d'écran.
- [ ] Le texte agrandi à 200 % reste lisible sans défilement horizontal.
- [ ] Les animations se coupent si l'appareil demande moins de mouvement.
- [ ] Rien ne clignote plus de trois fois par seconde.
- [ ] Les limites de temps peuvent être prolongées ou désactivées.
- [ ] La langue de la page est déclarée, et celle des passages dans une autre langue aussi.
- [ ] Les cibles cliquables mesurent au moins 24 × 24 pixels (et 44 sur mobile, voir L8).

## L8 Mobile et tactile

- [ ] L'écran tient à 320 pixels de large sans défilement horizontal.
- [ ] Les cibles tactiles mesurent au moins 44 × 44 points, et sont assez espacées.
- [ ] Les actions fréquentes sont à portée du pouce.
- [ ] Rien ne dépend du survol.
- [ ] Le clavier virtuel ne cache pas le champ en cours ni le bouton d'envoi.
- [ ] Les zones de sécurité (encoche, barre de geste) sont respectées.
- [ ] Les gestes cachés ont toujours une alternative visible.
- [ ] L'interface supporte la rotation, ou la bloque volontairement.
- [ ] Le contenu reste utilisable avec la taille de texte système agrandie.

## L9 Visuel, cohérence et règles maison

- [ ] Aucun emoji, nulle part ; des icônes d'une même bibliothèque à la place.
- [ ] Aucun dégradé violet, ni « look IA » (néons, verre dépoli généralisé, cartes flottantes empilées).
- [ ] Trois couleurs d'identité au plus, plus les neutres et les couleurs d'état.
- [ ] Les couleurs, tailles et espacements viennent de jetons (variables), pas de valeurs isolées.
- [ ] Une échelle typographique courte (quatre ou cinq tailles), une ou deux familles.
- [ ] Les espacements suivent une échelle régulière (par exemple 4 ou 8 pixels).
- [ ] Les composants semblables se ressemblent (boutons, champs, cartes).
- [ ] Le mode sombre, s'il existe, est conçu et vérifié, pas seulement inversé.
- [ ] Pas d'images générées ni de photos de banque génériques qui ne montrent rien du produit.
- [ ] Les animations sont rares, courtes et servent à comprendre (pas décoratives).

## L10 Performance ressentie

- [ ] Le contenu principal apparaît vite ; le reste peut suivre.
- [ ] Chaque action a un retour en moins de 100 millisecondes (même si le résultat prend plus).
- [ ] Les squelettes ou réservations d'espace évitent que la page saute pendant le chargement.
- [ ] Les images sont dimensionnées et compressées ; les polices ne bloquent pas l'affichage.
- [ ] Les listes très longues sont paginées ou chargées au fur et à mesure.
- [ ] Rien de lourd ne se charge pour une fonction que la plupart n'utilisent pas.

## L11 Confiance, vie privée et éthique

Le livret insiste sur la dimension éthique : imaginer comment le design
pourrait être détourné, exploité ou devenir néfaste.

- [ ] Aucun piège : pas de case précochée, de faux compte à rebours, de désabonnement caché, de culpabilisation (« Non merci, je n'aime pas économiser »).
- [ ] Le prix total et les engagements sont visibles avant de s'engager.
- [ ] On ne collecte que les données nécessaires, et l'on dit à quoi elles servent.
- [ ] Le consentement (cookies, notifications) est libre : refuser est aussi simple qu'accepter.
- [ ] Supprimer son compte et ses données est possible et trouvable.
- [ ] Les notifications sont utiles et réglables.
- [ ] Les chiffres, avis et témoignages affichés sont réels.
- [ ] On a imaginé les usages malveillants (harcèlement, fraude, triche) et prévu de quoi les limiter.
- [ ] Les publics fragiles (enfants, personnes âgées, en difficulté) ne sont pas mis en danger.

## L12 Langues, formats et international

- [ ] Aucun texte n'est écrit en dur dans le code de l'interface ; tout passe par les fichiers de traduction.
- [ ] La mise en page supporte des textes 30 à 40 % plus longs (l'allemand, le français) et les langues de droite à gauche si elles sont visées.
- [ ] Dates, heures, nombres, devises suivent la langue et le pays de l'utilisateur.
- [ ] Les pluriels sont gérés correctement (y compris zéro et un).
- [ ] Les noms, adresses et numéros acceptent les formats étrangers.
- [ ] Les fuseaux horaires sont gérés pour tout ce qui est daté.

## L13 Outil en ligne de commande

- [ ] `--help` et `-h` fonctionnent sur la commande et chaque sous-commande, avec des exemples.
- [ ] Les noms de commandes et d'options sont prévisibles et cohérents entre eux.
- [ ] Les erreurs disent ce qui a échoué, pourquoi, et quoi taper pour corriger.
- [ ] Le code de sortie vaut 0 en cas de succès, autre chose en cas d'échec.
- [ ] Les messages vont sur la sortie d'erreur, les résultats sur la sortie standard.
- [ ] Une sortie exploitable par un script existe (par exemple `--json`).
- [ ] Les couleurs se désactivent (variable `NO_COLOR`, sortie redirigée) et ne portent jamais seules une information.
- [ ] Les actions destructrices demandent confirmation, avec une option pour l'automatiser (`--yes`) et un mode d'essai (`--dry-run`).
- [ ] Les tâches longues montrent une progression et s'interrompent proprement (Ctrl+C).
- [ ] Rien n'attend une saisie quand l'outil tourne sans terminal interactif.
- [ ] Aucun emoji dans les sorties (règle maison, et lisibilité dans les journaux).

## L14 API et documentation

- [ ] Un premier appel réussi est possible en quelques minutes à partir de la page « démarrer ».
- [ ] Les noms (ressources, champs, paramètres) suivent une seule convention.
- [ ] Chaque erreur a un code stable, un message clair et, si possible, un lien vers la documentation.
- [ ] Chaque point d'accès a un exemple de requête et de réponse copiable, y compris d'erreur.
- [ ] Les limites (quotas, tailles, pagination) sont documentées et signalées dans les réponses.
- [ ] Les changements cassants sont versionnés et annoncés à l'avance.
- [ ] L'authentification est expliquée pas à pas, sans exposer de secret dans les exemples.

## L15 Interface conversationnelle ou vocale

- [ ] Le premier message dit ce que l'assistant sait faire, en une ou deux phrases.
- [ ] Les incompréhensions proposent des exemples de formulation ou des choix.
- [ ] Une action importante est confirmée avant d'être faite.
- [ ] On peut annuler, recommencer, ou parler à un humain à tout moment.
- [ ] Les réponses vocales sont courtes ; les listes vocales ont trois éléments au plus.
- [ ] Le ton est sobre ; pas de fausse émotion ni d'emojis.
- [ ] Les erreurs ne bouclent jamais (au bout de deux échecs, une autre voie est proposée).

## L16 Jeu

- [ ] La règle se comprend en jouant, en moins d'une minute.
- [ ] L'écran de départ tient dans la plus petite fenêtre visée, bouton « Jouer » compris.
- [ ] Les informations vitales (vies, temps, score) se voient sans quitter l'action des yeux.
- [ ] Chaque perte est visible et compréhensible au moment où elle arrive.
- [ ] La difficulté monte progressivement ; perdre paraît juste.
- [ ] La pause existe et se déclenche seule quand la fenêtre perd la main.
- [ ] Le son est coupé par défaut ou facile à couper.
- [ ] Les commandes marchent au doigt, à la souris et au clavier si le jeu est sur le web.
- [ ] Les effets rapides se coupent si l'appareil demande moins de mouvement.
- [ ] Le score est vérifié côté serveur s'il y a un classement.

## L17 Objet connecté et interface physique

- [ ] L'état de l'objet (allumé, connecté, occupé, en panne) se voit de loin.
- [ ] Chaque action a un retour immédiat (son, lumière, vibration).
- [ ] L'usage tient compte du contexte réel (gants, lumière forte, bruit, debout).
- [ ] L'objet fonctionne en mode dégradé sans réseau, et le dit.
- [ ] L'installation se fait sans manuel, ou avec un manuel d'une page.
- [ ] Une erreur indique une action concrète (« Rapprochez l'objet de la box »).
- [ ] Les réglages essentiels ne sont pas réservés à l'application.

## L18 Avant de livrer

- [ ] Ce qui est construit correspond à la maquette validée ; les écarts ont été annoncés et acceptés.
- [ ] La tâche principale a été faite de bout en bout sur le support le plus contraint (petit écran, clavier seul).
- [ ] Les états vides, d'erreur et de chargement ont été vus en vrai.
- [ ] Les textes ont été relus en situation, dans toutes les langues livrées.
- [ ] Les listes L7 (accessibilité) et L9 (règles maison) passent.
- [ ] Au moins une personne qui n'a pas conçu le produit a essayé la tâche principale, ou un test est prévu.
- [ ] Les hypothèses restées non vérifiées sont listées pour la suite.
