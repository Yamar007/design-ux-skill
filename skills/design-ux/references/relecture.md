# Relire une interface existante

Une relecture sert à décider quoi corriger d'abord. Elle vaut par sa justesse
(chaque remarque est vraie et prouvée) et par son ordre (l'essentiel en
premier), pas par sa longueur.

## 1. Situer

Écris en trois lignes, avant de juger :

- **Qui** utilise ce produit (le persona, même provisoire).
- **La tâche principale** qu'il vient accomplir.
- **Le support** et le contexte (téléphone dans le métro, ordinateur au
  bureau, borne dans un hall).

Si tu ne sais pas, déduis-le du produit (textes, données, navigation) et
écris-le comme hypothèse. Une interface ne se juge pas dans l'absolu : un
écran dense est une qualité pour un expert au bureau et un défaut pour un
débutant sur téléphone.

## 2. Parcourir réellement

Selon ce qui est disponible, du plus fiable au moins fiable :

1. **L'interface qui tourne** (si tu as un navigateur ou un émulateur) : fais
   la tâche principale de bout en bout, puis provoque les états (champ vide,
   mauvaise saisie, réseau coupé, liste vide, texte très long). Essaie au
   clavier seul, en petite largeur (320 à 390 pixels), et avec le texte
   agrandi. Fais des captures pour appuyer tes remarques.
2. **Le code** : lis les écrans, leurs textes, leurs états, les attributs
   d'accessibilité, les styles. Cherche les textes en dur, les `onClick` sur
   des `div`, les images sans texte de remplacement, les couleurs isolées.
3. **Des captures ou une description** fournies par l'utilisateur : tu ne vois
   qu'un instant figé ; dis ce que tu ne peux pas juger (comportement,
   clavier, lecteur d'écran).

Note pour toi chaque constat avec sa source exacte au moment où tu le vois.

## 3. Évaluer, dans cet ordre

1. **Le parcours** : la tâche principale réussit-elle ? Où sont les
   ruptures (hésitation, retour en arrière, impasse, abandon probable) ?
2. **L'action principale et la hiérarchie** (L3) : sur chaque écran du
   parcours, sait-on quoi faire ?
3. **Les textes** (L5) : comprend-on sans connaître l'équipe ?
4. **Les états** (L6) : que se passe-t-il quand ça ne se passe pas bien ?
5. **L'accessibilité** (L7) et le **mobile** (L8).
6. **Le visuel et les règles maison** (L9) : emojis, dégradés violets,
   cohérence.
7. **L'éthique** (L11) : pièges, collecte inutile, consentement forcé.
8. Les listes propres au type de projet (`adapter-au-projet.md`).

## 4. Classer par gravité

| Gravité | Signification | Exemple |
|---|---|---|
| **Bloquant** | Empêche une partie des utilisateurs de finir la tâche principale, ou expose à un risque (données, argent, sécurité, loi) | Bouton d'envoi caché sur petit écran ; formulaire inutilisable au clavier |
| **Majeur** | La tâche aboutit, mais au prix d'erreurs, d'hésitation ou d'abandons probables | Erreur de saisie qui vide le formulaire ; libellé « Valider » sur trois boutons différents |
| **Mineur** | Gêne ou incohérence qui ne change pas l'issue | Deux styles de boutons secondaires ; une date au format américain |
| **Confort** | Amélioration souhaitable | Raccourci clavier pour une action fréquente |

Pour décider entre deux niveaux : combien de personnes sont touchées, à quelle
fréquence, et peuvent-elles s'en sortir seules ?

Regroupe les remarques de même cause (« douze boutons à icône sans nom
accessible » est une remarque, pas douze).

## 5. Rédiger chaque remarque

Une remarque complète a cinq parties :

- **Le constat**, factuel : ce qui se passe.
- **La preuve** : fichier et ligne, zone de la capture, ou étape du parcours.
- **Qui est gêné** et comment.
- **La correction** proposée, concrète.
- **L'effort** estimé : petit, moyen, grand.

Exemple :

> **Majeur. L'erreur de carte vide le formulaire de paiement.**
> Preuve : `checkout/Payment.tsx:88`, `reset()` appelé dans le `catch`.
> Qui : tout client dont la carte est refusée ; il doit tout ressaisir, et
> beaucoup abandonnent à ce moment.
> Correction : garder les champs, n'effacer que le cryptogramme, afficher
> l'erreur au-dessus du bouton avec la marche à suivre.
> Effort : petit.

## 6. Rendre le rapport

Utilise `assets/modeles/rapport-relecture.md` :

1. Le contexte (les trois lignes de l'étape 1).
2. **Les trois problèmes qui comptent le plus**, quelle que soit leur
   catégorie, avec la raison de ce choix.
3. Le reste, par gravité.
4. Ce qui marche bien et doit être gardé (une refonte détruit souvent les
   bonnes choses par ignorance).
5. Ce que tu n'as pas pu vérifier.
6. La suite proposée.

## 7. Proposer la suite

- Une correction qui change ce que l'on voit passe par une maquette validée
  avant le code (règle maison).
- Une correction invisible (nom accessible, attribut de formulaire, message
  d'erreur manquant, texte de remplacement) peut se coder directement si
  l'utilisateur le demande.
- Si les problèmes viennent du parcours lui-même, propose une reconception
  (usage 1 du skill) plutôt qu'une liste de rustines.

## Ce qu'il faut éviter

- Juger selon tes goûts : chaque remarque se rattache à un utilisateur gêné ou
  à une règle (liste de contrôle, norme, règle maison).
- Inventer : si tu n'as pas vu l'état d'erreur, ne dis pas qu'il manque ; dis
  que tu n'as pas pu le voir.
- Noyer l'essentiel : un rapport de quarante remarques n'est pas lu.
- Réécrire tout le produit dans la relecture : elle diagnostique, la
  conception vient après.
