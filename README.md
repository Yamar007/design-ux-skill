# design-ux

Un skill pour Claude Code qui apporte une vraie démarche de design UX, pour
tout type de projet : site, application web ou mobile, outil interne, jeu,
commerce en ligne, objet connecté, interface vocale, outil en ligne de
commande, API.

Il reprend les trois phases de **« L'UX Design, le livret des méthodes »**
(Digital Design Lab, L'École de design Nantes Atlantique, 2020) :
**comprendre et se positionner**, **conceptualiser et proposer**,
**prototyper et évaluer**.

## Ce qu'il fait

- **Concevoir** un produit, un écran ou une fonctionnalité avant de coder :
  diagnostic, personas, parcours, concepts, wireframes, direction artistique,
  puis maquettes validées. L'effort s'adapte à la demande.
- **Relire** une interface existante (code, captures, interface en
  fonctionnement) : les trois problèmes qui comptent le plus, puis toutes les
  remarques classées par gravité, avec preuve et correction.
- **Vérifier** avec dix-huit listes de contrôle (formulaires, accessibilité
  WCAG 2.2, mobile, éthique, ligne de commande, API, voix, jeu, etc.),
  choisies selon le projet.

Trois règles toujours appliquées : pas d'emojis (des icônes à la place), pas
de dégradés violets ni de « look IA », et les maquettes avant le code (deux
ou trois options avec les vrais textes, validées avant d'écrire
l'interface). Les règles propres à un projet (`CLAUDE.md`, charte, système de
design) passent avant.

## Installation

Dans Claude Code :

```text
/plugin marketplace add Yamar007/design-ux-skill
/plugin install design-ux@design-ux
```

Choisis ensuite la portée : utilisateur (tous tes projets), projet (partagé
avec l'équipe via `.claude/settings.json`) ou locale (ce projet, sur ta
machine seulement). Mise à jour : `/plugin marketplace update design-ux`.

Sans plugin : copie le dossier `skills/design-ux` dans `~/.claude/skills/`
(tous tes projets) ou dans `<projet>/.claude/skills/` (un seul).

## Utilisation

Le skill se déclenche seul dès qu'on parle d'interface, d'écran, de parcours,
d'ergonomie, de maquette, de refonte ou d'audit. Pour l'appeler
directement : `/design-ux:design-ux` (plugin) ou `/design-ux` (copie).

- « Aide-moi à concevoir l'écran de réservation de mon appli, avant de coder. »
- « Relis la page d'inscription et dis-moi ce qui ne va pas. »
- « Quelle checklist UX passer avant la sortie de mon outil en ligne de commande ? »

## Contenu

```text
skills/design-ux/
├── SKILL.md       la démarche et les trois usages
├── references/    les trois phases, l'adaptation par type de projet, les maquettes,
│                  les règles visuelles, la relecture, les listes de contrôle
├── assets/        modèles de livrables, page de comparaison de maquettes
└── evals/         cas de test (format claude plugin eval)
```

## Crédits et licence

Adapté de **« L'UX Design, le livret des méthodes »**, Digital Design Lab,
L'École de design Nantes Atlantique, octobre 2020 (directeur de publication
Christian Guellerin ; responsable de publication Dr Frédérique Krupa), sous
licence Creative Commons BY-NC-SA 4.0.

Modifications : textes reformulés et réorganisés pour un assistant de code ;
ajout de l'adaptation par type de projet, de la procédure de relecture, des
listes de contrôle, des règles visuelles et des modèles.

Ce dépôt est publié sous la même licence, **CC BY-NC-SA 4.0** (voir
`LICENSE`). Il n'est ni affilié à L'École de design Nantes Atlantique ni
approuvé par elle.
