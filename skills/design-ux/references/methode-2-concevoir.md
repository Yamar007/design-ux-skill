# Phase 2 : conceptualiser et proposer

Une fois le contexte compris, ces méthodes créent de l'empathie entre les
parties prenantes et l'équipe, encouragent des solutions créatives, et
affinent le travail jusqu'à des propositions concrètes.

## Sommaire

1. Persona augmenté : synthèse, analyse, modélisation
2. Parcours utilisateur (journey map)
3. Techniques de créativité : génération de concepts, Crazy 8, brainstorming, carnet de croquis, carte heuristique, carte d'empathie, cas d'usage en six cases
4. Expression des concepts : storyboard en dessins, photos ou vidéo
5. Développement des concepts : wireframes, architecture de l'information

---

## 1. Persona augmenté

Un persona est la carte d'identité d'un utilisateur type, fondée sur des
contextes, comportements et habitudes **observés**. Il pose le contexte
d'utilisation, fait émerger un besoin auquel le projet répond, humanise la
cible, sert à tester des scénarios et facilite la communication.

- Un persona est propre à un projet : il ne se réutilise pas tel quel.
- Piège : le stéréotype. Crée plusieurs personas différents.
- Conseil d'expert du livret : en plus des utilisateurs habituels, modélise
  des **non-utilisateurs convaincus** et des **utilisateurs extrêmes** qui
  détournent les usages. Leurs motivations ouvrent des opportunités
  inattendues.

### Synthèse (environ une heure)

Trier les données brutes (photos, vidéos, enregistrements, notes) pour en
faire une synthèse exploitable : qui sont les usagers, dans quelles
situations, leurs buts, comportements, croyances, expertises, freins, ce qu'il
faut éviter. Organise les observations en trois rubriques : **moments et
lieux** ; **objets, outils, services** ; **activités, interactions,
processus**.

### Analyse (environ 30 minutes)

Repérer les comportements semblables (activités, attitudes, aptitudes,
motivations, compétences) et regrouper les personnes en profils. Ce filtrage
évite de bâtir un persona sur une seule personne observée ou sur un cliché.

La fiche d'analyse a deux colonnes :

- **Profil** : objectifs (ce qu'il cherche à accomplir), motivations (pourquoi),
  influences (ce qui inspire ses décisions), besoins (ce qu'il lui faut pour
  atteindre ses objectifs), souhaits (ce qu'il voudrait en plus ou à la
  place), problèmes (ce qui le gêne).
- **Contexte** : activité (tâches effectuées), lieux, moments (périodes,
  horaires, durée, fréquence), personnes présentes, objets utilisés, services
  utilisés (de la marque ou non).

### Modélisation (environ 45 minutes)

Pour chaque groupe, une fiche synthétique lisible d'un coup d'œil : au minimum
un prénom, un âge, un environnement, les buts, les comportements observés, les
facilités et difficultés, les points de friction. Une phrase à la première
personne aide à entrer en empathie, à condition qu'elle vienne d'un entretien
réel ou soit marquée comme imaginée.

Assistant : modèle `assets/modeles/persona.md`. Pas de photo inventée ni de
visage généré ; un prénom et un contexte suffisent. Marque « provisoire » un
persona construit sans données réelles.

---

## 2. Parcours utilisateur (environ une heure)

Le parcours rassemble les informations collectées et les analyse : il met en
valeur les points à améliorer pour une expérience donnée et sert à décliner
des concepts qui répondent aux opportunités trouvées. Ne crée pas de parcours
sans persona.

C'est un grand tableau, souvent illustré. Identifie d'abord le **pendant** de
l'expérience et la structure d'ensemble, avant de plonger dans les détails.

Lignes du tableau :

- **Moments** : avant, pendant, après.
- **Séquences d'usage** : les étapes numérotées.
- **Points de contact** : où et avec quoi la personne interagit.
- **Acteurs** : qui intervient à chaque étape.
- **Émotion** : une note de 1 à 5 par étape, qui dessine une courbe.
- **Ruptures** : les étapes où la courbe plonge ou où la personne abandonne.
- **Recommandations** : ce qu'on propose pour chaque rupture.

Trois niveaux de profondeur, du plus large au plus fin : **macro** (les trois
grands moments), **séquences** (les étapes de chaque moment), **micro** (le
scénario détaillé d'une étape). On peut ainsi mesurer l'effet d'une idée sur
une séquence, puis sur toute l'expérience.

Usages du parcours : partager la compréhension et lancer la discussion,
raconter une histoire avec les émotions vécues, repérer les manques et les
opportunités.

Assistant : modèle `assets/modeles/parcours.md`. Dans un produit existant,
parcours le vrai chemin dans le code ou l'interface pour remplir les étapes,
et note pour chaque rupture d'où vient l'information (observé, rapporté,
supposé).

---

## 3. Techniques de créativité

La créativité est un processus, parfois long. Une fois la question créative
posée, on génère beaucoup d'idées sous un angle conceptuel et visuel, puis on
les affine avec des techniques plus ciblées. Varie les techniques et les
personnes selon le besoin.

### Génération de concepts (une demi-journée)

1. **Questionner** : « Et si… ? » pour déplacer le sujet dans un autre domaine
   (« et si réserver un coiffeur était aussi simple que de commander un
   café ? »).
2. **Produire** : outils visuels (Crazy 8, planche d'humeur) ou conceptuels
   (carte heuristique, brainstorming, raisonnement par l'absurde,
   brainwriting).
3. **Premières idées** : s'il n'y en a pas assez, recommencer l'étape 2 avec
   d'autres outils.
4. **Affiner** : en visuel, le collage ; en conceptuel, **SCAMPER**
   (Substituer, Combiner, Adapter, Modifier, Proposer d'autres usages,
   Éliminer, Réorganiser), le **portrait chinois** (« si ce produit était un
   lieu, ce serait… »), la carte mentale.

### Crazy 8 (8 minutes)

Huit esquisses en huit minutes, une par minute, autour du besoin de
l'utilisateur. Puis on en discute. Assistant : huit variantes très
différentes, une ligne chacune, avant d'en développer deux.

### Brainstorming (environ une heure)

Rassembler toutes les idées d'une réunion. Simple et accessible, mais
définis bien les contours pour ne pas t'éparpiller.

### Carnet de croquis (en continu)

Noter et dessiner tout ce qui passe par la tête, à tout moment. Assistant :
garde un fichier de notes de projet où tu consignes idées et décisions.

### Carte heuristique (environ une heure)

Un schéma qui part d'un terme et suit le chemin associatif de la pensée. Il
dégage les thèmes principaux et les regroupements d'idées. Assistant : liste
imbriquée ou schéma Mermaid `mindmap`.

### Carte d'empathie (environ une heure)

Autour du persona : ce qu'il **pense et ressent**, ce qu'il **entend**, ce
qu'il **voit**, ce qu'il **fait**, ses **motivations**, ses **freins**. En
atelier, on joue le persona et le groupe l'interroge sans connaître ses
objectifs. But : des idées opérationnelles et des besoins affinés.

### Cas d'usage en six cases (15 minutes)

1. Le contexte.
2. L'utilisateur.
3. à 5. Le fonctionnement de la proposition, étape par étape.
6. Les arguments clés qui complètent la compréhension et l'intérêt.

En multipliant ces mini cas d'usage, on analyse tout ou partie d'un concept.
Modèle dans `assets/modeles/concepts.md`.

---

## 4. Expression des concepts

Le storyboard illustre le moment où les utilisateurs rencontrent le produit
ou le service dans son contexte social, environnemental et technique. Il crée
de l'empathie et sert à communiquer un positionnement.

1. Une histoire simple, selon le message et le public visé.
2. Un personnage tiré du persona, dans un contexte réel (temps, lieu, milieu
   social) : son comportement, son apparence, ses attentes, ses pensées.
3. Des actions découpées en **trois à six cases**, une idée centrale chacune.
4. Un texte par case (récit, bulle, légende), surtout si l'image seule ne
   suffit pas, ou pour mettre en avant des verbatims.

Conseils : de vrais humains dans de vrais contextes ; montrer les émotions,
aux moments qui posent problème comme à ceux qui marchent.

Formes possibles : dessins (rapides, compris par tous, idéaux pour tout type
de concept), photos et photomontages (réalistes), vidéo (pour un produit
tangible ou un service, quand un prototype semi-fonctionnel existe).

Assistant : un storyboard en texte, case par case, ou une page HTML simple
avec des vignettes schématiques. Pas d'images générées.

---

## 5. Développement des concepts

Le design allie **fonctionnalité** (l'ergonomie, qui suppose de comprendre les
utilisateurs, leurs usages et leurs interactions) et **esthétique** (traitée
ensuite, en phase 3). L'organisation du contenu doit suivre le **modèle mental
de l'utilisateur**. On valide ici avec le client la cohérence et l'équilibre
des éléments, pour une navigation la plus intuitive possible.

Conseil du livret : ne perds pas de temps à dessiner des wireframes
sophistiqués ; un croquis rapide exprime mieux une idée au début.

### Architecture de l'information (environ 30 minutes)

Organiser le contenu et les informations de manière claire : séparer chaque
partie d'une interface (texte, image, action) et mettre à plat la navigation
entre les grandes parties. Elle donne une version simplifiée du produit et
fait passer les fonctionnalités avant l'esthétique.

Assistant : un arbre des écrans (ou des commandes, pour un outil en ligne de
commande ; des intentions, pour une interface vocale), avec pour chaque nœud
ce qu'on y fait. Vérifie que les mots de l'arbre sont ceux des utilisateurs,
pas ceux de l'équipe ou de la base de données.

### Wireframe (environ une heure)

Spatialiser le contenu : mettre à plat les écrans et les liens entre eux pour
voir comment ils s'organisent. Il clarifie la navigation et structure les
écrans de façon schématique.

Assistant : wireframes en HTML gris, sans couleur ni image, ou en blocs de
texte pour les cas simples. Une seule action principale par écran, visible
sans chercher. Voir `references/maquettes.md`.
