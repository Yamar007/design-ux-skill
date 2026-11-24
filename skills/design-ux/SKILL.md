---
name: design-ux
description: Méthode complète de design UX (d'après « L'UX Design, le livret des méthodes » de L'École de design Nantes Atlantique) pour tout type de projet (site, application web ou mobile, outil interne, jeu, e-commerce, objet connecté, interface vocale, outil en ligne de commande, API). À utiliser dès que l'utilisateur parle d'interface, d'écran, de parcours, d'ergonomie, d'expérience utilisateur, de maquette, de refonte ou de « rendre ça plus clair », pour 1) concevoir un projet, un écran ou une fonctionnalité avant de coder (comprendre, personas, parcours, concepts, maquettes validées) ; 2) relire une interface existante (code, captures, URL) et lister ses problèmes par gravité avec des corrections ; 3) fournir des listes de contrôle adaptées (navigation, formulaires, textes, accessibilité, états, mobile, éthique). Règles maison toujours appliquées, pas d'emojis, pas de dégradés violets, maquettes validées avant le code. Also for UX design, UI review, usability audit, wireframes, design checklist.
license: CC-BY-NC-SA-4.0
---

# Design UX

Ce skill transpose la démarche du livret « L'UX Design, le livret des méthodes »
(Digital Design Lab, L'École de design Nantes Atlantique, 2020, licence CC BY-NC-SA 4.0)
en façon de travailler pour un assistant qui conçoit et relit des interfaces.
La méthode tient en trois phases : **comprendre et se positionner**,
**conceptualiser et proposer**, **prototyper et évaluer**. Elle sert à
concevoir du neuf, à juger l'existant, et à vérifier avant de livrer.

L'idée centrale du livret, à garder en tête partout : on conçoit pour des
personnes précises, dans un contexte réel, et on valide chaque étape avec elles
avant de passer à la suivante. Un bon écran se mérite ; il ne sort pas d'un
premier jet de code.

## Les règles maison (toujours)

Ces règles viennent de l'utilisateur. Elles s'appliquent à tout ce que tu
proposes, maquettes, code, textes et rapports.

1. **Pas d'emojis.** Ni dans l'interface, ni dans les textes, les emails, les
   notifications, les commits ou les rapports. Pour un repère visuel, utilise
   une icône d'une bibliothèque (Lucide, Material Symbols, SF Symbols, Phosphor)
   ou un mot. Les emojis donnent un air bricolé et se rendent différemment
   d'un système à l'autre.
2. **Pas de dégradés violets**, ni du « look IA » qui va avec (violet vers
   bleu, néons, verre dépoli partout, cartes flottantes à ombre douce
   empilées). Préfère des aplats. Un dégradé ne se justifie que par une
   raison de sens (une jauge, une carte de chaleur), jamais pour décorer.
   Détails dans `references/regles-visuelles.md`.
3. **Les maquettes avant le code.** Aucune ligne de code d'interface tant
   qu'une maquette n'a pas été montrée et validée. Propose deux ou trois
   options, avec les vrais textes, et laisse choisir. Une correction issue
   d'une relecture suit la même règle quand elle change ce que l'on voit.
   Comment faire : `references/maquettes.md`.

Si un projet a déjà sa propre charte ou ses propres règles (un fichier
`CLAUDE.md`, un dossier `design-system/`, un guide de style), lis-les d'abord :
elles complètent ces règles, et l'emportent sur tout le reste de ce skill.

## Étape 0 : situer la demande

Avant tout, réponds pour toi à trois questions. Elles décident de ce que tu
lis ensuite.

**1. Quel usage ?**

| L'utilisateur veut | Usage | Va à |
|---|---|---|
| créer un produit, un écran, une fonctionnalité, refaire une page | Concevoir | « Usage 1 » ci-dessous |
| un avis sur ce qui existe, « qu'est-ce qui ne va pas », un audit | Relire | « Usage 2 » |
| une liste à cocher, « qu'est-ce que je dois vérifier » | Vérifier | « Usage 3 » |

Une demande mêle souvent deux usages (relire puis reconcevoir) : fais-les dans
l'ordre, et dis-le.

**2. Quel type de projet ?** Lis la section qui correspond dans
`references/adapter-au-projet.md`. Elle dit quelles méthodes comptent le plus,
sous quelle forme faire les maquettes et quels pièges guetter. Un outil en
ligne de commande ne se conçoit pas comme une application mobile.

**3. Quelle taille ?** La méthode complète prend des semaines ; une
fonctionnalité en prend une heure. Ajuste avec le tableau « Proportionner la
méthode » plus bas. Ne déroule jamais toutes les méthodes par principe.

S'il te manque une information qui change vraiment la suite (qui sont les
utilisateurs, sur quel support, ce qui existe déjà), pose **une question à la
fois**, de préférence à choix multiples avec ta recommandation en premier.
Pour le reste, prends une hypothèse raisonnable, écris-la, et avance.

## Usage 1 : concevoir

Suis les trois phases du livret. Chaque phase se termine par un **livrable
montré à l'utilisateur et validé** avant de passer à la suivante. Les fiches
détaillées de chaque méthode sont dans `references/methode-1-comprendre.md`,
`references/methode-2-concevoir.md` et `references/methode-3-prototyper.md`.
Les modèles à remplir sont dans `assets/modeles/`.

### Phase 1 : comprendre et se positionner

But : savoir de quoi on parle, pour qui, et où le design peut vraiment aider.

1. **Définir le sujet** : si le problème est déjà défini, décris son usage,
   son identité et sa technique ; sinon, cherche ce qui l'entoure
   (environnement, personnes, processus). Puis recadre : quels éléments
   méritent d'être creusés ?
2. **Mots-clés et sous-sujets**, pour borner la recherche.
3. **Recherche et veille** : produits voisins, concurrents, conventions de la
   plateforme, technologies utiles. Dans un projet existant, la recherche
   commence par le code et le contenu : routes, écrans, textes, données,
   retours d'utilisateurs, tickets.
4. **Acteurs et parties prenantes** : internes et externes, leur proximité au
   projet, leurs liens.
5. **Observer les utilisateurs** : tu ne peux pas aller sur le terrain, mais
   tu peux préparer le guide d'entretien, le sondage ou la grille
   d'observation (`assets/modeles/observation.md`), et synthétiser ce que
   l'utilisateur rapporte. Préfère le qualitatif : quelques entretiens
   apprennent plus qu'un sondage seul.
6. **Recadrer et choisir des axes** : matrice de recadrage (le problème vu par
   quatre acteurs ou angles), puis **deux ou trois axes de positionnement**,
   chacun en une phrase courte qui dit l'intention.

Livrable : le **diagnostic** (`assets/modeles/diagnostic.md`) avec les axes
proposés. L'utilisateur en choisit un ou plusieurs.

### Phase 2 : conceptualiser et proposer

But : se mettre à la place des utilisateurs, chercher large, puis resserrer.

1. **Personas** (`assets/modeles/persona.md`) : un ou plusieurs profils fondés
   sur ce qui a été observé ou rapporté, chacun avec ses objectifs, ses
   motivations, ses freins et son contexte (lieux, moments, objets, services).
   Pense aussi aux utilisateurs extrêmes et aux non-utilisateurs : ils révèlent
   les opportunités inattendues. Évite le stéréotype.
2. **Parcours utilisateur** (`assets/modeles/parcours.md`) : avant, pendant,
   après ; les séquences d'usage, les points de contact, l'émotion à chaque
   étape, et surtout les **ruptures**, là où l'expérience casse. Pas de
   parcours sans persona.
3. **Créativité** : élargis avant de choisir (« Et si… ? », idées en vrac,
   carte heuristique, raisonnement par l'absurde, SCAMPER, carte
   d'empathie). Fiches dans `references/methode-2-concevoir.md`. Ne t'arrête
   pas à ta première idée.
4. **Exprimer les concepts** : pour chacun, un cas d'usage en six cases ou un
   storyboard de trois à six vignettes (`assets/modeles/concepts.md`).
5. **Développer** : architecture de l'information conforme au modèle mental
   de l'utilisateur, puis wireframes (structure, pas encore de style).

Livrable : personas, parcours avec ses ruptures, **deux ou trois concepts**
exprimés, et les wireframes du concept retenu.

### Phase 3 : prototyper et évaluer

But : donner forme, vérifier que ça marche, et seulement ensuite coder.

1. **Direction artistique** : planche d'univers, puis charte (couleurs,
   typographies, formes, icônes, ton). Trois couleurs d'identité au plus. Pour
   un projet qui a déjà une charte, respecte-la.
2. **Preuve de concept** si une incertitude technique bloque (deux briques
   fonctionnent-elles ensemble ?). Elle se fait tôt et petit.
3. **Maquettes** (`references/maquettes.md`) : deux ou trois options
   comparables, vrais textes, écrans clés, états importants (vide, erreur,
   chargement), téléphone et ordinateur si le produit vit sur les deux.
   **Montre-les et attends la validation.**
4. **Évaluer** : relis tes propres maquettes avec les listes de contrôle, puis
   propose un test avec de vrais utilisateurs (tâches à faire réaliser, ce
   qu'on observe).
5. **Raconter le projet** si l'utilisateur doit le présenter : fiche mémoire
   (`assets/modeles/fiche-memoire.md`) ou présentation en cinq temps
   (contexte, démarche, positionnement, mise en scène, opportunités).

Livrable : maquettes validées. Le code commence ici, et il suit la maquette
validée ; tout écart se signale avant d'être codé.

### Proportionner la méthode

| Taille de la demande | Ce que tu fais vraiment |
|---|---|
| Petit changement (un libellé, un bouton, un état d'erreur) | Contexte en deux lignes, une ou deux options en maquette, listes de contrôle concernées |
| Nouvel écran ou nouvelle fonctionnalité | Phase 1 express (sujet, utilisateurs, existant), un persona et un parcours courts, deux ou trois options de maquette |
| Refonte d'un produit existant | Relecture complète (usage 2) comme diagnostic, puis phases 2 et 3 |
| Nouveau produit | Les trois phases, livrable par livrable |

Dans tous les cas, garde les deux garde-fous : écrire pour qui et pourquoi,
et valider une maquette avant le code.

### Ce que tu sais et ce que tu supposes

Le livret fonde le design sur l'observation. Toi, tu travailles souvent sans
utilisateurs sous la main. Alors :

- distingue clairement ce qui vient de données réelles (entretiens, chiffres,
  retours, code) de ce qui est une **hypothèse à vérifier** ;
- n'invente jamais de citations d'utilisateurs ni de chiffres présentés comme
  réels ; un persona construit sans données se dit « provisoire » ;
- propose, quand c'est utile, comment vérifier l'hypothèse (cinq entretiens,
  un test de cinq minutes, une mesure).

## Usage 2 : relire une interface existante

Procédure complète, échelle de gravité et exemples : `references/relecture.md`.
En bref :

1. **Situer** : qui utilise ce produit, pour quelle tâche principale, sur quel
   support. Si tu ne le sais pas, déduis-le du produit et écris ton hypothèse.
2. **Parcourir réellement** : lis le code des écrans et leurs textes, ou les
   captures fournies ; si tu as un navigateur à disposition, ouvre l'interface,
   fais la tâche principale, regarde les états (vide, erreur, chargement,
   succès), le téléphone et le clavier.
3. **Évaluer** avec les lentilles du livret puis les listes de contrôle : le
   parcours et ses ruptures, la clarté de l'action principale, les textes,
   l'accessibilité, la cohérence visuelle, les règles maison, l'éthique
   (pièges, collecte de données inutile).
4. **Classer** chaque problème par gravité (bloquant, majeur, mineur, confort),
   avec sa **preuve** (fichier et ligne, zone de la capture, étape du
   parcours), qui il gêne, et la **correction** proposée.
5. **Rendre le rapport** avec `assets/modeles/rapport-relecture.md` : les trois
   problèmes qui comptent le plus d'abord, puis le reste par gravité.
6. **Proposer la suite** : les corrections visibles passent par une maquette
   avant le code (règle maison 3) ; les corrections invisibles (un attribut
   d'accessibilité, un message d'erreur manquant) peuvent se coder directement
   si l'utilisateur le demande.

Reste juste : ne signale que ce que tu as vu, et dis ce que tu n'as pas pu
vérifier. Un rapport de quarante remarques mineures noie l'essentiel ; regroupe.

## Usage 3 : vérifier avec les listes de contrôle

Les listes sont dans `references/listes-de-controle.md`. Choisis celles qui
s'appliquent au type de projet (la section de `references/adapter-au-projet.md`
les nomme) ; ne déverse pas tout. Ajoute ensuite les points propres au métier
du projet, que les listes génériques ne peuvent pas connaître : une sauvegarde
se vérifie et se restaure, un paiement se rembourse, une réservation
s'annule, un message envoyé ne se reprend pas. Rends-les sous forme de cases à cocher
`- [ ]`, chaque point formulé pour être vérifiable par oui ou non. Si tu as
accès à l'interface ou au code, coche toi-même ce que tu peux vérifier et
indique pour chaque point non conforme où il se trouve.

## Façon de communiquer

- Écris dans la langue de l'utilisateur, avec des phrases courtes et sans
  jargon non expliqué : un persona, un parcours, un wireframe se définissent
  en une ligne la première fois.
- Montre plutôt que décrire : un tableau de parcours, une maquette, une liste.
- À chaque fin de phase, résume en quelques lignes ce qui est décidé, puis
  pose la question de validation. Ne passe pas à la phase suivante sans
  réponse.
- Recommande. Quand tu proposes des options, dis laquelle tu choisirais et
  pourquoi, en une phrase.

## Fichiers du skill

| Fichier | Quand le lire |
|---|---|
| `references/adapter-au-projet.md` | Toujours, à l'étape 0, la section du type de projet |
| `references/methode-1-comprendre.md` | Phase 1, ou pour préparer entretiens, sondages, veille |
| `references/methode-2-concevoir.md` | Phase 2 : personas, parcours, créativité, wireframes |
| `references/methode-3-prototyper.md` | Phase 3 : direction artistique, preuve de concept, maquettes, présentation |
| `references/maquettes.md` | Dès qu'il faut montrer une maquette |
| `references/regles-visuelles.md` | Pour toute proposition visuelle, et en relecture |
| `references/relecture.md` | Usage 2 |
| `references/listes-de-controle.md` | Usage 3, et pour vérifier tes propres maquettes |
| `assets/modeles/*.md` | Modèles des livrables à remplir |
| `assets/maquettes-comparaison.html` | Page de départ pour montrer deux ou trois options côte à côte |
