# Faire et faire valider les maquettes

Règle maison : aucune ligne de code d'interface avant qu'une maquette ait été
montrée et validée. La maquette coûte quelques minutes à changer ; le code,
des heures. Elle sert aussi à parler du même objet : l'utilisateur valide ce
qu'il voit.

## Le niveau de détail selon le moment

| Moment | Forme | But |
|---|---|---|
| Phase 2, structure | Wireframe : blocs gris, vrais textes, aucune couleur | Valider l'organisation et le parcours |
| Phase 3, aspect | Maquette fidèle : couleurs, typographies, icônes réelles | Valider le rendu final |
| Petite correction | La zone concernée, avant et après | Valider le changement sans refaire l'écran |

## La forme selon le support

- **Web et applications** : une page HTML statique, un seul fichier, sans
  outil de construction, que l'utilisateur ouvre dans son navigateur. Pars de
  `assets/maquettes-comparaison.html`. Montre la largeur téléphone (environ
  390 pixels) et la largeur ordinateur si le produit vit sur les deux, et le
  mode sombre s'il existe.
- **Application mobile native** : même principe, cadre de téléphone, en
  imitant les composants de la plateforme (ne pas inventer un sélecteur de
  date iOS).
- **Outil en ligne de commande** : des transcriptions de terminal dans un bloc
  de code : la commande tapée, la sortie, le code de sortie.
- **Interface vocale ou conversationnelle** : des scripts de dialogue, tour
  par tour.
- **Objet physique, borne** : un storyboard et un schéma des états ; l'écran à
  sa taille réelle si l'objet en a un.
- **Si un outil de maquette est disponible** (un connecteur Figma, Canva, un
  outil de pages publiées, un compagnon visuel dans le navigateur), utilise-le
  plutôt qu'un fichier local, à condition que l'utilisateur puisse le voir.

## Deux ou trois options, vraiment différentes

Propose deux ou trois options qui diffèrent sur un choix qui compte (la
structure, la place de l'action principale, le ton, le nombre d'étapes), pas
trois variations de couleur. Pour chaque option :

- un nom court (« A. Tout sur un écran », « B. Trois étapes ») ;
- ce qu'elle privilégie et ce qu'elle sacrifie, en une ou deux lignes ;
- ta recommandation, en premier, avec sa raison.

Mets les options côte à côte, dans la même page, à la même échelle.

## Ce que doit contenir une maquette

- Les **vrais textes**, dans la langue du produit. Le texte fait partie du
  design ; un faux texte cache les problèmes de longueur et de clarté.
- Des **données réalistes** : des noms, montants, dates plausibles, et un cas
  long (un nom de quarante caractères, une liste de cent lignes).
- Les **états** qui comptent : vide, erreur, chargement, succès.
- Les **règles maison** : pas d'emojis (des icônes réelles, par exemple en SVG
  de la bibliothèque Lucide), pas de dégradés violets, voir
  `regles-visuelles.md`.
- Si le projet a déjà une charte : ses couleurs, polices et composants. Lis
  les jetons dans le code (variables CSS, fichier de thème) plutôt que de les
  deviner.

## Faire valider

1. Donne le chemin du fichier (ou le lien) et dis comment l'ouvrir.
2. Résume en trois lignes ce que montre chaque option.
3. Pose une question fermée : « Quelle option gardes-tu : A, B ou C ? »,
   avec ta recommandation.
4. Attends la réponse. Un silence n'est pas un accord.
5. Note la décision (dans le document de conception du projet, s'il y en a
   un) avec les remarques de l'utilisateur.

Si l'utilisateur demande un changement, refais la maquette et revalide ; ne
corrige pas directement dans le code « pour gagner du temps ».

## Après la validation

- Le code suit la maquette validée. Si une contrainte technique oblige à
  s'en écarter, dis-le avant de coder, et propose l'écart en maquette s'il se
  voit.
- Une fois construit, compare l'écran réel à la maquette (capture côte à
  côte) avant de dire que c'est fini.
- Garde les maquettes validées dans le projet (par exemple
  `docs/maquettes/`) : elles font foi pour la suite.
