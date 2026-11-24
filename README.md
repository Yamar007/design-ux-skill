# design-ux : un skill de design UX pour Claude Code

Ce skill donne à Claude une vraie démarche de design d'expérience
utilisateur, valable pour tout type de projet : site, application web ou
mobile, outil interne, jeu, commerce en ligne, objet connecté, interface
vocale, outil en ligne de commande, API.

Il s'appuie sur **« L'UX Design, le livret des méthodes »** du Digital Design
Lab de L'École de design Nantes Atlantique (édition 2020), dont il reprend la
démarche en trois phases : **comprendre et se positionner**,
**conceptualiser et proposer**, **prototyper et évaluer**.

## Ce qu'il fait

1. **Concevoir** un produit, un écran ou une fonctionnalité avant de coder :
   diagnostic, personas, parcours utilisateur et ses ruptures, concepts,
   wireframes, direction artistique, puis maquettes montrées et validées.
   La méthode se proportionne à la demande : un libellé ne mobilise pas trois
   semaines de recherche.
2. **Relire** une interface existante (code, captures, interface en
   fonctionnement) : les trois problèmes qui comptent le plus, puis toutes les
   remarques classées par gravité, chacune avec sa preuve et sa correction.
3. **Vérifier** avec dix-huit listes de contrôle (navigation, formulaires,
   textes, états, accessibilité WCAG 2.2, mobile, visuel, performance,
   éthique, international, ligne de commande, API, voix, jeu, objet connecté,
   avant de coder, avant de livrer), choisies selon le projet.

## Les règles maison

Le skill applique toujours trois règles :

- **pas d'emojis**, nulle part : des icônes d'une bibliothèque à la place ;
- **pas de dégradés violets** ni de « look IA » ;
- **les maquettes avant le code** : deux ou trois options, avec les vrais
  textes, validées avant d'écrire une ligne d'interface.

Si un projet a ses propres règles (un `CLAUDE.md`, une charte, un système de
design), le skill les lit d'abord et elles l'emportent.

## Installation

### Depuis GitHub, comme plugin (recommandé)

Dans Claude Code :

```
/plugin marketplace add <compte-github>/design-ux-skill
/plugin install design-ux@design-ux
```

Claude Code demande alors **où l'installer** :

- **pour toi, dans tous tes projets** (portée utilisateur) ;
- **pour ce projet seulement, partagé avec l'équipe** (portée projet,
  enregistré dans `.claude/settings.json`) ;
- **pour ce projet, sur ta machine seulement** (portée locale).

Tu peux ainsi l'activer dans les projets de ton choix. Pour le mettre à jour :
`/plugin marketplace update design-ux`.

### Depuis un dossier local

Avant de le publier, ou pour le modifier :

```
/plugin marketplace add E:\design-ux-skill
/plugin install design-ux@design-ux
```

### Sans plugin, par simple copie

Copie le dossier `skills/design-ux` :

- dans `~/.claude/skills/` pour tous tes projets ;
- ou dans `<ton-projet>/.claude/skills/` pour un seul projet.

## Utilisation

Le skill se déclenche seul quand tu parles d'interface, d'écran, de parcours,
d'ergonomie, de maquette, de refonte ou d'audit. Tu peux aussi l'appeler
directement : `/design-ux` (ou `/design-ux:design-ux` une fois installé
comme plugin).

Exemples :

- « Aide-moi à concevoir l'écran de réservation de mon appli, avant de coder. »
- « Relis la page d'inscription et dis-moi ce qui ne va pas. »
- « Quelle checklist UX passer avant la sortie de mon outil en ligne de
  commande ? »

## Contenu

```
skills/design-ux/
├── SKILL.md                      la démarche et les trois usages
├── references/
│   ├── adapter-au-projet.md      douze types de projets
│   ├── methode-1-comprendre.md   écosystème, veille, parties prenantes, observation, axes
│   ├── methode-2-concevoir.md    personas, parcours, créativité, storyboard, wireframes
│   ├── methode-3-prototyper.md   direction artistique, preuve de concept, maquettes, présentation
│   ├── maquettes.md              faire et faire valider les maquettes
│   ├── regles-visuelles.md       les règles maison en détail
│   ├── relecture.md              la procédure de relecture et l'échelle de gravité
│   └── listes-de-controle.md     les dix-huit listes
├── assets/
│   ├── modeles/                  diagnostic, persona, parcours, observation, concepts, rapport, fiche mémoire
│   └── maquettes-comparaison.html
└── evals/                        trois cas de test (concevoir, relire, vérifier)
```

## Tester le skill

Les cas de test de `skills/design-ux/evals/` suivent le format de
`claude plugin eval`. Depuis le dossier du skill :

```
claude plugin eval . --allow-tools Write,Edit,Bash --scaffold
```

Chaque cas tourne avec et sans le skill ; ce sont de vrais appels au modèle,
donc facturés.

## Crédits et licence

La démarche, les méthodes et leurs descriptions sont adaptées de
**« L'UX Design, le livret des méthodes »**, Digital Design Lab, L'École de
design Nantes Atlantique, octobre 2020 (directeur de publication Christian
Guellerin ; responsable de publication Dr Frédérique Krupa), publié sous
licence Creative Commons BY-NC-SA 4.0.

Modifications apportées : textes reformulés et réorganisés pour un assistant
de code, ajout de l'adaptation par type de projet, de la procédure de
relecture, des listes de contrôle, des règles visuelles et des modèles.

Ce dépôt est donc publié sous la même licence, **CC BY-NC-SA 4.0** (voir
`LICENSE`) : partage et adaptation libres, en citant la source, sans usage
commercial du contenu lui-même, et sous la même licence. Ce dépôt n'est ni
affilié à L'École de design Nantes Atlantique ni approuvé par elle.
