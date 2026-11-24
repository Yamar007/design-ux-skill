# Phase 1 : comprendre et se positionner

Ces méthodes définissent le contexte, les parties prenantes et les questions
que le design va traiter. Elles élargissent le terrain, cherchent les
opportunités, et priorisent les besoins concrets. Elles se terminent par des
axes de positionnement.

Chaque fiche donne : le but, la façon de faire, ce que tu peux faire toi-même
en tant qu'assistant, et les pièges. Les durées indiquées sont celles d'un
atelier humain, pour te donner l'ordre de grandeur.

## Sommaire

1. Comprendre l'écosystème : définition du sujet, mots-clés, recherche primaire, acteurs initiaux
2. Veille artistique et technologique
3. Cartographie des parties prenantes
4. Observer les parties prenantes : sondage, ethnographie, entretien
5. Opportunités de design et axes de positionnement : matrice de recadrage

---

## 1. Comprendre l'écosystème

Premiers pas du projet : avoir la vue d'ensemble pour définir le sujet et la
problématique, et poser une base de connaissances. Cible tes recherches pour ne
pas te perdre dans des domaines qui ne concernent pas le projet.

### Définition du sujet (environ une heure)

- **Le problème est-il déjà défini ?**
  - Oui : décris-le selon trois angles, **usage** (qui fait quoi, quand),
    **identité** (ce que le produit représente, son ton, sa marque),
    **technique** (plateforme, contraintes, données).
  - Non : cherche ce qui est relié au sujet, l'environnement, les personnes
    impliquées, les processus utilisés.
- **Brainstorming** : tout ce qui vient à l'esprit sur le sujet, sans trier.
- **Recadrage** : quels éléments méritent d'être creusés ensuite ?

Assistant : écris ces trois blocs dans le diagnostic. Dans un projet existant,
remplis « technique » en lisant le code (stack, routes, modèles de données)
plutôt qu'en le demandant.

### Mots-clés (environ une heure)

Découpe le sujet principal en sous-sujets, puis en sujets spécifiques, et
relie-les (liste en cascade ou carte mentale). Exemple : « voyage d'affaires »
donne « affaires » (employés, entreprises) et « voyage » (destination,
transport), qui se rejoignent en « moyens de transport des employés ».

But : borner le projet, décider ce qu'on traite et ce qu'on laisse.

### Recherche primaire (environ deux heures)

Recueillir assez d'informations pour comprendre le défi de design : identifier
le sujet, collecter les données existantes, comparer. Puis, avec un esprit
ouvert : suspendre son jugement, viser la quantité, imaginer, rebondir sur les
idées des autres.

Assistant : produits concurrents et voisins, conventions de la plateforme
(guides officiels d'Apple, de Google, du W3C), articles et études si tu peux
chercher en ligne. Cite tes sources et date-les.

### Acteurs initiaux (environ une heure)

Les personnes ou organisations directement impliquées ou associées au projet,
et leurs relations. Fais deux listes : **acteurs internes** (équipe, direction,
support, développeurs) et **acteurs externes** (utilisateurs, clients,
partenaires, régulateurs, concurrents).

---

## 2. Veille artistique et technologique

La veille surveille un environnement pour s'adapter à ses changements. Les
connaissances personnelles sont limitées ; la veille les élargit et doit
devenir systématique. Source et date chaque trouvaille.

- **Veille artistique** : construire un imaginaire commun sur le sujet en
  explorant d'autres domaines par analogie (cinéma, musique, architecture,
  jeux, édition) et en reliant les trouvailles.
- **Veille technologique** : les innovations existantes et leur
  fonctionnement, pour repérer les briques techniques utiles au projet.

Le processus en cinq étapes :

1. **Recherche passive** : la culture générale qu'on entretient avant le
   projet (flux d'actualité, magazines, expositions). Elle évite d'être pris
   de court par un sujet inconnu.
2. **Recherche globale** : à réception du brief, accumuler beaucoup
   d'informations, explorer le champ des possibles, repérer mots-clés et
   experts.
3. **Recherche active** : contacter les personnes clés, faire des recherches
   ciblées (recherche booléenne, bases scientifiques). Plus courte que la
   globale ; elle dégage les tendances du marché et des usages.
4. **Analyse** : trier, hiérarchiser, synthétiser ; donner du sens à la masse
   (carnet, planche univers, planche tendance, carte heuristique).
5. **Représentation** : choisir le support pour partager (présentation,
   croquis, vidéo). C'est ce qui permet aux parties prenantes de s'approprier
   le projet.

Assistant : rends une synthèse courte, par exemple un tableau « référence,
ce qu'elle fait bien, ce qu'on en retient, source ». Dis clairement si tu n'as
pas pu chercher en ligne et que la veille repose sur tes connaissances.

---

## 3. Cartographie des parties prenantes (environ une heure)

Une partie prenante est toute personne ou entité qui travaille, sert ou
intervient dans le projet. La cartographier assure qu'on les implique tout au
long du projet et fait comprendre les jeux d'acteurs. Bien cibler qui sont les
utilisateurs est la première étape avant de comprendre leurs besoins, leurs
contextes, leurs compétences et leurs habitudes.

1. Identifier les parties prenantes.
2. Échanger avec les principales personnes concernées.
3. Les placer en cercles concentriques selon leur proximité au projet (au
   centre, ceux qui le portent ; puis les sources, les plateformes, les
   fournisseurs).
4. Tracer les liens entre elles et qualifier chaque lien (ce qui circule :
   argent, données, demandes, contenu).

Revois la carte régulièrement : elle évolue avec le projet.

Assistant : une carte en liste imbriquée ou un schéma Mermaid suffit. Pour un
outil interne, les parties prenantes cachées comptent beaucoup (le support qui
répond aux questions, le service juridique, l'équipe qui maintient).

---

## 4. Observer les parties prenantes

Comprendre le contexte avant de concevoir : sur le terrain, en échangeant avec
les usagers, on comprend leur identité et leurs besoins. Choisis une ou
plusieurs des trois méthodes selon le projet. Privilégie le qualitatif : plus
long, mais il donne des réponses fines. Piège : ne te fier qu'aux sondages, qui
ne donnent pas une observation complète.

### Sondage (30 à 60 minutes à préparer)

Un formulaire diffusé à un large panel, souvent anonyme, avec des questions de
plusieurs types (ouvertes, fermées, choix multiple, échelle). Il donne vite
une vue générale des habitudes et opinions.

Assistant : rédige le questionnaire (`assets/modeles/observation.md`) ;
questions neutres, une idée par question, échelles cohérentes, une ou deux
questions ouvertes à la fin. Puis analyse les réponses que l'utilisateur
rapporte.

### Ethnographie (plusieurs jours)

Observer le terrain, les utilisateurs, leurs interactions et le contexte
d'usage réel, et poser des questions rapides et précises. Variantes :
échantillon d'expérience, journaux de bord, photos personnelles, sonde
culturelle. Posture bienveillante, sans préjugés, attentive aux attitudes,
croyances, pratiques, besoins et émotions.

Assistant : prépare une grille d'observation (moments et lieux ; objets,
outils, services ; activités et interactions ; ce qui frustre) et aide à la
dépouiller. Dans un produit numérique, l'équivalent proche : les
enregistrements de sessions, les tickets du support, les avis.

### Entretien (30 à 60 minutes par personne)

Entretien qualitatif, de préférence en personne, pour recueillir perception,
opinion, expérience. Il humanise et vérifie les données collectées autrement,
et fait naître des hypothèses.

Assistant : rédige le guide (questions ouvertes sur des situations vécues,
« racontez-moi la dernière fois que… », jamais « aimeriez-vous que… »). À la
synthèse, relève les **phrases clés** des personnes interrogées, exactement
telles qu'elles ont été dites, avec leur auteur.

---

## 5. Opportunités de design et axes de positionnement

Valider les opportunités où le design apporte une vraie valeur, puis en tirer
des axes. Un axe de positionnement est une direction de travail née du
croisement des recherches et de la veille : une reformulation de la
problématique initiale, plus fine et centrée sur l'usager, qui ouvre des
pistes de solutions.

- La problématique n'est pas forcément une question.
- Elle doit être comprise par tous les acteurs.
- Un axe tient en **une phrase courte** qui dit l'intention du designer.
- On en crée le plus souvent **deux ou trois**, pour aborder le problème sous
  des angles différents.
- Piège : rester bloqué sur la première idée.

### Matrice de recadrage (environ une heure)

Le problème au centre, entouré de quatre points de vue. Pour chacun : ce que
la veille en dit, ce que l'observation a montré, et l'acteur sur lequel il se
concentre. Se mettre dans la tête de chaque acteur fait imaginer les problèmes
qu'il rencontre, et prendre du recul.

Variante en triangle : **résultats** (ce qu'on veut obtenir), **moyens** (ce
qu'on a), **usages** (ce que les gens font).

Exemples d'axes, pour une problématique comme « maintenir le lien social de
personnes isolées » :

1. « Un geste par jour » : un rituel très simple qui crée un contact quotidien.
2. « La famille en relais » : rendre visible aux proches qui a besoin d'eux.

Assistant : présente la matrice dans le diagnostic, puis les axes avec, pour
chacun, ce qu'il privilégie et ce qu'il sacrifie. Recommande-en un.
