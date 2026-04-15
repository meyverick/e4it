# Guide d'Étude Structuré : Architecture et Terminologie `HTML` & `CSS`

## Niveau 1 : Fondamentaux du Web, Architecture et Protocoles

*Comprendre comment les navigateurs, les serveurs et les moteurs de recherche échangent l'information.*

* **`Client/Server Environment`** : Modèle d'architecture où l'ordinateur de l'utilisateur (le client) demande des ressources, et un ordinateur distant (le serveur) les fournit.
* **`HTTP Protocol` & `Transaction HTTP`** : Le `HTTP Protocol` est l'ensemble des règles standardisées permettant le transfert de fichiers sur le web. Une `Transaction HTTP` désigne le cycle complet et asynchrone d'une requête envoyée par le client et de la réponse retournée par le serveur.
* **Méthodes de requête** :
  * **`GET Method`** : Demande le téléchargement d'une information depuis un serveur en lecture seule (sans modifier les données distantes).
  * **`POST Method`** : Soumet des données sécurisées (souvent via un formulaire) pour modifier l'état ou enregistrer des informations sur le serveur distant.
* **`URL` (Universal Resource Locator)** : L'adresse unique spécifiant le protocole et le chemin exact pour localiser une ressource spécifique sur le réseau.
* **Langages et Standards** :
  * **`SGML` (Standard Generalized Markup Language)** : L'ancêtre abstrait des langages de balisage, séparant la structure de la présentation visuelle.
  * **`HTML` (Hypertext Markup Language) & `HTML5`** : Le `HTML` est le langage déclaratif de base sérialisant la sémantique et la structure du contenu web. `HTML5` est son évolution moderne, incluant des balises sémantiques natives et des API multimédias puissantes.
  * **`CSS3`** : L'évolution moderne du langage de mise en forme, apportant des capacités avancées comme les animations et les grilles de mise en page.
  * **`Standardization`, `W3C` & `WHATWG`** : Le processus de `Standardization` garantit que le code fonctionne de manière identique sur tous les navigateurs. Le `W3C` et le `WHATWG` sont les consortiums qui définissent ces règles officielles.
* **Moteurs et Indexation** :
  * **`Search Engine` & `Indexing`** : Un `Search Engine` agrège et classe les pages web. L'`Indexing` est le processus d'analyse sémantique permettant d'enregistrer ces pages dans ses bases de données.
  * **`Robot` & `robots`** : Un `Robot` est un programme automatisé explorant le web. La directive `robots` permet de lui interdire d'indexer certaines pages.
* **`WYSIWYG`** (What You See Is What You Get) : Interface de création permettant de construire une page web visuellement, le logiciel générant automatiquement le code sous-jacent.

## Niveau 2 : Structure de Base `HTML` et Sémantique du Texte

*Les éléments de construction fondamentaux pour créer l'arbre du document (`Document Object Model`).*

* **Syntaxe et Structure Globale** :
  * **`Document Structure` & `Root Element`** : L'organisation hiérarchique invisible de la page, dont le `Root Element` (généralement la balise `<html>`) est le conteneur principal.
  * **`Tag` (Balise)** : Unité lexicale (souvent entre chevrons) qui indique le début et la fin d'un élément.
  * **`Nesting`** : Le principe d'imbrication stricte, consistant à insérer un élément entièrement à l'intérieur d'un autre.
  * **`Attribute`** : Métadonnée ajoutée dans la balise d'ouverture (ex: `title`) pour configurer l'élément.
  * **`Indentation` & `Comments`** : L'`Indentation` est l'espacement visuel du code source. Les `Comments` (ex: `<!-- Note -->`) sont des notes ignorées par le navigateur.
  * **`case-sensitive`** : La règle imposant la distinction stricte entre majuscules et minuscules, fondamentale en développement.
* **Conteneurs et Texte Principal** :
  * **`div` & `span`** : `div` est une boîte générique (bloc) sans signification sémantique, tandis que `span` est un conteneur microscopique utilisé au sein d'une ligne de texte.
  * **`h1 to h6`** : Titres hiérarchiques structurant l'importance de l'information, du plus important (`h1`) au sous-titre (`h6`).
  * **`p (paragraph)`** : Un bloc contenant un flux textuel séquentiel et cohérent.
  * **`br` & `wbr`** : `br` force un saut de ligne immédiat. `wbr` suggère un point de coupure optionnel pour les mots très longs.
* **Mise en Forme et Emphase sémantique** :
  * **`strong` & `em`** : `strong` indique une importance majeure (souvent en gras), tandis qu'`em` indique une emphase rhétorique (souvent en italique).
  * **`i (italic)`, `u (underline)`, `s (strikethrough)`** : `i` marque une distinction linguistique (terme technique ou étranger), `u` une ambiguïté (erreur d'orthographe), et `s` indique qu'une information est devenue obsolète.
  * **`sub`, `sup`, `small`, `mark`** : `sub` et `sup` gèrent les indices et exposants. `small` est utilisé pour les mentions légales périphériques. `mark` sert de surbrillance visuelle.
  * **`del` & `ins`** : Signalent respectivement un texte supprimé ou récemment inséré, utile pour les suivis de modification.
* **Éléments Spécialisés** :
  * **Citations** : **`blockquote`** (longue citation externe), **`q (quote)`** (citation courte en ligne), **`cite`** (source de la citation).
  * **Informatique** : **`code`** (code source), **`samp`** (résultat d'un programme), **`kbd`** (touche du clavier), **`var`** (variable mathématique), **`dfn`** (première définition d'un terme).
* **Listes** : **`ul`** (liste non ordonnée), **`ol` / `Ordered List`** (liste ordonnée), **`li`** (élément individuel de la liste).
  * **Listes de Définitions** : **`dl`** (conteneur de liste de définitions), **`dt`** (terme défini), **`dd`** (description textuelle du terme).
  * **Typographie asiatique** : **`ruby`, `rt`, `rp`** servent à afficher de petites annotations de prononciation au-dessus des idéogrammes.
  * **Anciens éléments (Obsolètes)** : **`center`** et **`xmp`** étaient autrefois utilisés pour centrer ou afficher du code brut, aujourd'hui remplacés par le CSS.

## Niveau 3 : Hyperliens, Images et Multimédia

*Connecter les documents et y intégrer des ressources graphiques ou sonores.*

* **Liens Hypertextes** :
  * **`Anchor` & `Hypertext Link`** : L'élément d'ancrage créant un pont interactif cliquable.
  * **`href`** : L'attribut indispensable contenant l'adresse de destination (`URL`).
  * **`Internal Link` / `External Link`** : Lie vers une autre section de la même page/site, ou vers un site totalement externe.
  * **`target`** : Directive permettant d'ouvrir le lien dans un nouvel onglet (ex: `target="_blank"`).
  * **`alink`, `vlink`** : Attributs colorimétriques obsolètes pour les liens actifs ou visités.
* **Images et Cartographies visuelles** :
  * **`img`, `src`, `GIF/JPEG`** : `img` intègre une image matricielle (comme un `GIF/JPEG`) située à l'adresse définie par l'attribut `src`.
  * **`Image Mapping` (`map`, `area`, `usemap`, `coords`, `shape`)** : Technique permettant de définir de multiples zones cliquables (grâce à `coords` et `shape` dans une balise `area`) sur une seule image référencée via `usemap`.
* **Multimédia (HTML5)** :
  * **`audio`, `source`** : Lecteur sonore natif. `source` permet de proposer plusieurs formats de fichiers pour que le navigateur choisisse le meilleur.
  * **`object`, `embed`, `param`** : Éléments historiques permettant d'incruster des applications externes ou plugins, configurés via `param`.

## Niveau 4 : Architecture de Base `CSS` et Principes de Style

*Séparer le design de la structure et comprendre l'application des règles visuelles.*

* **Intégration du Style** :
  * **`Cascading Style Sheets (CSS)`** : Le langage déclaratif dictant l'apparence visuelle de la page web.
  * **`Cascading` & `Inheritance (CSS)`** : Le `Cascading` (cascade) est l'algorithme résolvant les conflits de règles selon leur priorité. L'`Inheritance` (héritage) permet aux éléments enfants d'adopter automatiquement certaines propriétés de leurs parents (ex: la police de texte).
* **Méthodes de Déclaration** :
  * **`style` & `Inline Styles`** : Styles définis directement sur la balise. Ils possèdent la priorité maximale mais brisent la réutilisabilité modulaire du code.
  * **`Embedded Styles`** : Règles placées dans l'en-tête (head) du document HTML.
  * **`Linked Styles` & `link`** : Fichiers externes attachés au document HTML via la balise `link`.
  * **`Imported Styles` & `@import`** : Permet à une feuille de style d'importer dynamiquement une autre feuille de style.
* **Sélecteurs Fondamentaux** :
  * **`ID Selector`** : Cible un élément unique via son identifiant strict (ex: `#MainNavigation`).
  * **`Class Selector`** : Identifiant réutilisable pour styliser de multiples éléments simultanément (ex: `.Card`).
* **Couleurs** :
  * **`color`** : Gère l'intensité spectrale (la couleur) du texte.
  * **`Hexadecimal Color`** : Code alphanumérique (base-16) définissant la couleur.
  * **`RGB Code / RGBA`** & **`HSLa`** : Formules (Rouge-Vert-Bleu / Teinte-Saturation-Luminosité) permettant d'instruire l'écran sur la couleur, incluant le canal "a" (`Alpha`) pour gérer l'opacité.

## Niveau 5 : Modèle de Boîte (`Box Model`) et Mise en Page de Base

*Comprendre comment les dimensions et l'espacement sont calculés pour chaque élément.*

* **`Box Model`** : Le paradigme géométrique selon lequel chaque élément web est une boîte rectangulaire composée d'un contenu, d'un espace interne, d'une bordure et d'un espace externe.
* **Dimensions** :
  * **`width` & `height`** : La largeur et la hauteur du contenu.
  * **`min-width`, `max-width`, `min-height`, `max-height`** : Les contraintes de dilatation et de rétrécissement, servant de barrières de sécurité visuelles.
* **L'Espacement et les Limites** :
  * **`Padding`** (`padding-top`, `padding-right`, `padding-bottom`, `padding-left`) : L'aire d'éloignement interne empêchant le contenu de toucher les bords.
  * **`Border`** (`border-top`, `border-color`, `border-width`, etc.) : L'anneau géométrique visible délimitant l'élément.
  * **`Margin`** (`margin-top`, `margin-right`, `margin-bottom`, `margin-left`) : La zone d'exclusion externe et invisible qui repousse les éléments adjacents.
* **Affichage et Visibilité** :
  * **`display`** : Détermine le comportement du composant dans le flux du document (en bloc, en ligne, caché, etc.).
  * **`visibility`** : Rend l'élément transparent, tout en conservant son espace vide pour ne pas détruire la mise en page.
  * **`opacity`** : Module la transparence globale de l'élément et de son contenu (de 0 à 1).

## Niveau 6 : Tableaux de Données et Formulaires Interactifs

*Structurer des données en grille et concevoir des interfaces de saisie pour l'utilisateur.*

* **Tableaux de Données** :
  * **`Table (Nested Tables)`** : Architecture matricielle. Un tableau peut être imbriqué dans un autre (`Nested`).
  * **`Row` & `Cell`** : La `Row` est la ligne horizontale contenant des cases de données (`Cell`).
  * **`thead`, `tbody`, `tfoot`** : Structuration sémantique de l'en-tête, du corps de données central, et de la ligne des totaux ou de conclusion.
  * **`th` & `td`** : `th` est une cellule d'en-tête décrivant la colonne/ligne, `td` est une cellule de donnée classique.
  * **`Rowspan` & `Colspan`** : Permettent à une cellule de s'étirer pour englober plusieurs lignes (`rowspan`) ou plusieurs colonnes (`colspan`).
  * **`caption` & `caption-side`** : Légende descriptive du tableau et son positionnement.
  * **Attributs obsolètes** : `Cellpadding`, `Cellspacing`, `valign`, `hspace`, `vspace`.
* **Formulaires et Interfaces d'Entrée** :
  * **`Form` & `method`** : Conteneur encapsulant les champs de saisie. La `method` détermine le type de transaction (`GET` ou `POST`).
  * **`Input Field` (`input`, `type`, `name`, `value`)** : Le champ de saisie atomique. Son attribut `type` modifie radicalement son apparence et comportement. `name` l'identifie pour le serveur, `value` contient la donnée soumise.
  * **`Checkbox` & `Radio Button`** : La `Checkbox` permet une sélection multiple, tandis que le `Radio Button` force une sélection unique parmi un groupe. L'attribut `checked` pré-coche l'option.
  * **Menus Déroulants** : **`select` / `Select List`** est le menu conteneur, **`Option`** représente un choix individuel. `multiple` autorise des choix multiples, et `size` définit la hauteur du menu.
  * **`fieldset` & `legend`** : Regroupent visuellement et logiquement des champs liés. `legend` est le titre de ce groupe.
  * **`label`** : Texte cliquable associé formellement à un champ de saisie pour améliorer l'accessibilité.
* **`Form attributes` (Validation et Aide)** :
  * `placeholder` (indice textuel fantôme), `required` (champ obligatoire), `pattern` (règle stricte de format), `autocomplete` (remplissage automatique), `novalidate` (désactive la validation), `dirname`, `step` (incrément strict), `min` & `max` (limites numériques).

## Niveau 7 : Sémantique `HTML5` et Hiérarchie du Document

*Remplacer les boîtes génériques (`div`) par des conteneurs porteurs de sens pour les moteurs de recherche.*

* **`Semantic Tags`** : Balises modernes décrivant explicitement la fonction de chaque zone du document.
  * **`header`** : Section introductive ou bannière d'en-tête.
  * **`nav`** : Graphe dirigeant principal du routage (le menu de navigation).
  * **`main`** : Contenu central et unique de la page.
  * **`section`** : Regroupement thématique générique.
  * **`article`** : Contenu textuel autonome et auto-suffisant (ex: un article de blog).
  * **`aside`** : Informations sémantiquement périphériques (barre latérale).
  * **`footer`** : Clôture logique de la page, contenant souvent mentions légales et liens de bas de page.
  * **`figure` & `figcaption`** : Un média illustratif (`figure`) et sa légende explicative propre (`figcaption`).

## Niveau 8 : `CSS` Intermédiaire : Typographie et Arrière-plans

*Ajuster l'esthétique du texte et orchestrer des décors graphiques sophistiqués.*

* **Typographie Avancée** :
  * **`font`, `Font-family`, `font-size`, `Font-weight`, `font-style`, `font-variant`** : Règlent la police de caractères, la taille, l'épaisseur (gras), l'inclinaison (italique), etc.
  * **`@font-face`** : Règle permettant d'importer et d'utiliser une ressource typographique personnalisée externe.
  * **`text-align`, `text-decoration`, `text-transform`** : Gèrent l'alignement (gauche, centre), l'ornement (soulignement), et la modification forcée de la casse (majuscules).
  * **`text-indent`, `letter-spacing`, `word-spacing`** : Contrôlent les décalages, l'écartement des lettres et l'espace entre les mots.
  * **`word-wrap`, `text-overflow`** : Protègent l'interface en coupant brutalement un mot trop long ou en insérant des points de suspension élégants si le texte déborde.
  * **`text-shadow`** : Filtre projetant une ombre calquée exactement sur la forme des lettres.
* **Arrière-plans et Décoration** :
  * **`list-style`** : Détermine la forme des puces (points, numéros) dans une liste.
  * **`background-color`, `background-image`** : Appliquent une couleur unie ou une image sur la couche d'arrière-plan du composant.
  * **`background-position`, `background-repeat`, `background-attachment`, `background-size`, `background-origin`, `background-clip`** : Un vaste cluster déterminant respectivement l'alignement, le carrelage (répétition), le défilement (fixe ou mobile), l'échelle d'adaptation, le point de départ de l'image, et la limite visuelle de l'arrière-plan par rapport aux bordures.
  * **`border-radius`** : Arrondit mathématiquement les coins géométriques de la boîte.
  * **`box-shadow`** : Génère une réplique ombrée de la boîte pour donner une illusion de profondeur tridimensionnelle.
  * **`linear-gradient`, `radial-gradient`** : Fonctions d'interpolation dessinant de fluides dégradés de couleurs linéaires ou circulaires.
  * **`cursor`** : Remplace l'apparence matérielle de la souris (ex: main cliquable) au survol de l'élément.

## Niveau 9 : Mises en Page `CSS` Avancées et Ordonnancement Spatial

*Briser le flux documentaire standard pour concevoir des architectures bidimensionnelles complexes.*

* **Positionnement Spatial (`Positioning`)** :
  * **`Relative Positioning`** : Décale un élément visuellement sans que sa position d'origine ne soit remplie par d'autres éléments.
  * **`Absolute Positioning`** : Retire totalement l'élément du flux normal pour le placer à des coordonnées précises par rapport à son parent positionné.
  * **`Z-index`** : Le scalaire de profondeur résolvant les conflits de chevauchement en décidant quel élément passe visuellement par-dessus l'autre.
* **Mise en page classique et Flottants** :
  * **`float` & `clear`** : `float` permet à un élément de flotter sur un bord, le texte s'enroulant autour. `clear` annule cet effet en forçant l'élément suivant à se placer en dessous du bloc flottant.
* **Architectures Modernes** :
  * **`Flexbox`** : Algorithme unidimensionnel fluide (`flex-direction`, `justify-content`, `align-items`, `flex-wrap`, `flex-grow`, `flex-shrink`, `flex-basis`, `order`) permettant de distribuer dynamiquement l'espace et d'aligner parfaitement des éléments sur un axe.

  ```css
    .FlexContainer {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  ```

  * **`Grid Layout`** : Système de quadrillage bidimensionnel puissant orchestrant le placement visuel en colonnes et lignes abstraites.
  * **Multicolonnes** : **`column-count`, `column-width`, `column-gap`, `column-rule`** fracturent le texte d'un long paragraphe en plusieurs colonnes à la manière d'un journal.
* **Éléments Obsolètes** : `box-flex`, `box-orient`, `box-ordinal-group`, ainsi que la division archaïque des fenêtres via **`Frame`**, **`Frameset`** et **`iframe`**.

## Niveau 10 : Sélecteurs Avancés et Pseudo-classes

*Cibler précisément des éléments selon leur comportement interactif ou leur relation hiérarchique.*

* **`Attribute selectors` (`[attr^="val"]`, `[attr$="val"]`, `[attr*="val"]`)** : Ciblent des balises en fonction de la correspondance de texte présente dans leurs paramètres de configuration.
* **Combinaisons de proximité** :
  * **`Adjacency combinator (+)`** : Sélectionne l'élément qui suit immédiatement et directement l'élément de référence.
  * **`Adjacency combinator (~)`** : Sélectionne tous les éléments frères qui suivent l'élément de référence dans le même conteneur.
* **`Pseudo-class` (États contextuels et logiques)** :
  * `:root` (le document de base), `:target` (l'élément visé par l'URL), `:empty` (les boîtes sans aucun contenu textuel ou visuel).
  * Formulaires : `:checked`, `:valid`, `:invalid` modifient le design en temps réel selon la validation de la donnée entrée.
  * Hiérarchie structurale : `:first-of-type`, `:last-of-type`, `:only-child`, **`nth-child`**, **`nth-last-child`** appliquent une logique mathématique séquentielle pour cibler un élément récurrent (ex: 1 sur 2).
* **`Pseudo-element`** : Insèrent virtuellement des éléments graphiques inexistants dans le code source.
  * **`first-letter` & `first-line`** : Modifient uniquement la première lettre ou la première ligne du texte.
  * **`content`** : Utilisé via un `Pseudo-element` (comme `::before`) pour injecter du texte ou des icônes décoratives.

## Niveau 11 : `Responsive Web Design` (RWD) et Mathématiques Appliquées

*Créer des interfaces s'adaptant automatiquement à tous les écrans, des téléphones aux grands moniteurs.*

* **Adaptation au Matériel** :
  * **`Viewport` (`<meta name="viewport">`)** : Directive vitale calibrant l'échelle d'affichage du navigateur mobile avant tout calcul de présentation.
  * **`Media Queries` / `@media`** : Règles logiques permettant au CSS d'inspecter les dimensions de l'écran et d'appliquer ou non des styles spécifiques.

  ```css
    @media (min-width: 1024px) {
      body { background-color: gray; }
    }
  ```

* **Unités Relatives Flexibles** :
  * **`vw`, `vh`, `vmin`, `vmax`** : Unités vectorielles représentant respectivement un pourcentage de la largeur (`vw`) ou de la hauteur (`vh`) totale de l'écran visible.
  * **`rem`** : Multiplicateur scalaire basant la taille des composants strictement sur la dimension typographique racine de la page.
* **Opérateurs Algébriques** :
  * **`calc()`** : Résout des équations mathématiques mélangeant différentes unités (ex: `100% - 50px`) pour définir une dimension dynamique.
  * **`min()` & `max()`** : Forcent un élément à sélectionner automatiquement la dimension la plus petite ou la plus grande parmi une liste de valeurs de sécurité.

## Niveau 12 : Animations, Transformations, Transitions et Filtres

*Orchestrer le mouvement temporel, l'interaction fluide et le traitement d'images complexe en temps réel.*

* **`Transition`** :
  * `transition-property`, `transition-duration`, `transition-timing-function`, `transition-delay` : Automatisent l'adoucissement progressif lors du passage d'un état visuel à un autre (ex: au survol de la souris).
* **`Transform`** :
  * Manipule mathématiquement la géométrie d'un élément sans perturber les éléments adjacents. Permet de faire pivoter (**`rotate`**), déplacer (**`translate`**), agrandir/rétrécir (**`scale`**), ou incliner (**`skew`**) l'élément.

  ```css
    .InteractiveBox { transform: translate(50px, 20px) rotate(15deg); }
  ```

* **`Animation`** :
  * **`@keyframes`** : Définit avec précision le plan descriptif des étapes de cheminement d'une séquence animée.
  * Paramètres (`animation-name`, `animation-duration`, `animation-iteration-count`, `animation-direction`, `animation-fill-mode`, `animation-play-state`, `animation-delay`) orchestrent la chorégraphie temporelle complexe.
  * **`cubic-bezier`** : Formule mathématique sophistiquée pour manipuler la courbe d'accélération d'une transition ou d'une animation.
* **Filtres Visuels (`filter`)** :
  * Un groupe d'instructions vectorielles asynchrones modifiant l'image au niveau du pixel final : **`blur`** (flou), **`brightness`** (luminosité), **`contrast`**, **`grayscale`** (noir et blanc), **`hue-rotate`** (rotation spectrale des couleurs), **`invert`** (couleurs négatives), **`saturate`** (vivacité chromatique), **`sepia`** (vieillissement cuivré).

## Niveau 13 : API Modernes du Web, Interactivité et Métadonnées

*Les capacités d'interfaces avancées gérées nativement par le navigateur.*

* **Métadonnées et Scripts** :
  * **`metadata`, `keywords`, `title`** : Informations abstraites (souvent dans l'en-tête) vitales pour les moteurs de recherche, la description thématique et l'onglet du navigateur.
  * **`script`, `noscript`** : `script` injecte et exécute les langages de programmation (JavaScript). `noscript` est la balise de secours si le script est désactivé ou bloqué.
  * **`async`** : Optimise le chargement réseau en demandant que l'exécution d'un fichier script externe ne bloque pas l'affichage de la page.
* **Composants Interactifs Natifs** :
  * **`details` & `summary`** : Le système de panneau pliable naturel de l'ordinateur où cliquer sur `summary` révèle le contenu enfermé dans `details`.
  * **`datalist`** : Une boîte invisible de suggestions liées à un champ de saisie offrant un menu d'auto-complétion natif.
  * **`meter` & `progress`** : `meter` est une jauge mesurant une quantité statique, `progress` est la barre de chargement animée d'une tâche continue.
  * **`output`** : L'écran digital exposant le résultat calculé d'un processus scripté de l'utilisateur.
  * **`time`** : Encode une date lisible par l'humain dans une norme informatique précise lisible par les robots.
* **Composants Graphiques de Haute Performance** :
  * **`canvas`** : La surface de dessin vierge permettant à l'ordinateur de construire des rendus bitmaps interactifs très complexes manipulés par script.
  * **`svg`** : Langage déclaratif mathématique (vecteurs) pour créer des tracés nets et redimensionnables à l'infini sans pixellisation.
* **Attributs Comportementaux Spéciaux** :
  * **`contenteditable`** : Rend n'importe quel texte de la page éditable directement par l'utilisateur comme un traitement de texte.
  * **`draggable` & `dropzone`** : Rendent l'élément physiquement préhensible pour les interactions tactiles ou souris de glisser-déposer.
  * **`download`** : Attribut forçant un lien à télécharger physiquement le fichier sur le disque dur au lieu de l'afficher.
