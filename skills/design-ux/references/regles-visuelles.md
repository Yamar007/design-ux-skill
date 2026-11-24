# Règles visuelles

Le but : des interfaces sobres, lisibles, qui ont l'air conçues pour leur
sujet, et pas sorties d'un générateur. Ces règles complètent la charte du
projet ; si le projet en a une, elle l'emporte sur les choix par défaut
ci-dessous, mais jamais sur les deux interdits (emojis, dégradés violets).

## Les deux interdits

### Pas d'emojis

Nulle part : interface, textes, boutons, titres, notifications, emails,
messages d'erreur, sorties de terminal, commits, rapports.

Pourquoi : ils changent d'aspect selon le système, se lisent mal par les
lecteurs d'écran (« visage riant aux larmes »), et donnent un air amateur.

À la place : une icône d'une bibliothèque cohérente (Lucide, Material
Symbols, SF Symbols, Phosphor), toujours la même famille, avec un nom
accessible si elle est seule ; ou simplement un mot.

### Pas de dégradés violets, ni le « look IA »

Ce qui est visé : le dégradé violet vers bleu ou rose, les fonds néon, le
verre dépoli appliqué partout, les cartes flottantes à ombre douce empilées,
les blobs flous en arrière-plan, les titres en dégradé, les petites étoiles
« magie » pour signaler l'intelligence artificielle.

Pourquoi : c'est devenu la signature des interfaces produites sans intention ;
elles se ressemblent toutes et ne disent rien du sujet.

À la place : des aplats, une couleur d'accent tirée du sujet, du contraste,
de la typographie. Un dégradé reste possible s'il porte un sens (une jauge,
une carte de chaleur, la lumière d'un ciel dans une illustration) ; jamais
pour décorer un fond ou un bouton.

## Les choix par défaut

### Couleurs

- **Trois couleurs d'identité au plus** (conseil du livret), plus des neutres
  et les couleurs d'état (succès, avertissement, erreur, information).
- Tire la couleur du sujet et de son univers (veille, planche univers), pas
  d'une palette à la mode.
- Définis-les en jetons (variables) et vérifie les contrastes dès le départ :
  4,5:1 pour le texte courant, 3:1 pour le gros texte et les éléments
  d'interface.
- Le mode sombre se conçoit : des fonds sombres pas tout à fait noirs, des
  couleurs d'accent revues pour garder le contraste, et une vérification
  écran par écran.

### Typographie

- Une ou deux familles. Une échelle courte (quatre ou cinq tailles).
- Texte courant à 16 pixels au moins sur le web, lignes de 50 à 75 caractères.
- La hiérarchie vient de la taille, de la graisse et de l'espace, pas de la
  couleur seule.

### Espace et grille

- Une échelle d'espacement régulière (multiples de 4 ou de 8 pixels).
- L'espace regroupe ce qui va ensemble ; plutôt que d'enfermer chaque chose
  dans une carte, sépare par l'espace et les filets.
- Alignements nets : peu d'axes, toujours les mêmes.

### Formes et composants

- Un seul rayon d'arrondi (ou deux, petit et grand), appliqué partout.
- Les boutons ont des états visibles : survol, focus, appui, désactivé,
  chargement.
- Un bouton principal par écran, reconnaissable entre tous.
- Pas de boutons en forme de pilule dans le contenu si le projet ne l'a pas
  choisi ; c'est un tic du « look généré ».

### Images

- Pas d'images générées. Pas de photos de banque qui ne montrent rien du
  produit (mains sur un clavier, poignées de main).
- Préfère les vraies captures du produit, les vraies photos du sujet, ou une
  illustration simple et cohérente.

### Mouvement

- Peu d'animations, courtes (150 à 300 millisecondes), qui aident à
  comprendre (d'où vient un élément, ce qui a changé).
- Coupées si l'appareil demande moins de mouvement.
- Jamais d'animation qui retarde l'accès au contenu.

## Vérifier

Avant de montrer une maquette ou de livrer, passe la liste L9 de
`listes-de-controle.md`. En relecture, chaque emoji ou dégradé violet trouvé
est une remarque (gravité mineure en général, majeure si c'est le texte d'un
bouton ou une information portée seulement par l'emoji).
