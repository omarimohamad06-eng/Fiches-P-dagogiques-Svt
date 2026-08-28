# جذاذات SVT — Générateur de fiches pédagogiques

Application web **autonome** (un seul fichier `index.html`, aucun serveur, aucune connexion
internet, aucune bibliothèque externe) pour préparer et imprimer des **جذاذات / fiches de
préparation de cours** de SVT.

Application conçue par **Pr. Omari Mohammed**, professeur de Sciences de la Vie et de la Terre,
et développée avec Claude (Anthropic). Son monogramme sert de logo dans l'en-tête et d'icône
d'onglet (tracé vectoriel intégré, sans fichier externe). Elle est utilisable telle quelle par n'importe quel
professeur : l'en-tête est vierge au départ et se renseigne en quelques clics.

## Utilisation

1. Télécharger `index.html`.
2. L'ouvrir par double-clic dans n'importe quel navigateur (Chrome, Edge, Firefox).
3. Saisir la fiche : tout est enregistré automatiquement dans le navigateur.
4. Bouton **Imprimer / PDF** → dans la fenêtre du navigateur choisir :
   *Destination* « Enregistrer au format PDF », *Format* A4, *Orientation* **Paysage**,
   *Marges* « Aucune », et cocher **« Graphiques d'arrière-plan »**.

## En-tête de votre établissement

- L'**académie régionale** se choisit dans une liste des **12 AREF** du Royaume ; la
  **direction provinciale** se choisit ensuite dans la liste des directions de cette académie
  (**82 directions** au total). L'intitulé officiel complet est inséré automatiquement, en
  français ou en arabe selon la langue du document, et reste modifiable.
- Renseignez une fois l'académie, la direction, l'établissement, votre nom et votre logo, puis
  cliquez sur **« Mémoriser comme défaut »** : toutes vos prochaines fiches en hériteront.
  Ces informations restent sur votre ordinateur.

## Assistant « programme officiel »

Le programme national de SVT (sections internationales, option français — MEN, avril 2015) est
**intégré dans l'application**, en français et en arabe : **18 unités, 72 leçons et 213 contenus**
pour les 5 niveaux.

1. Choisir le **niveau** → la liste des unités du programme se met à jour.
2. Choisir l'**unité** puis la **leçon** (avec son enveloppe horaire officielle).
3. Cocher ce qu'il faut remplir puis cliquer sur **« Remplir la fiche »** : unité, titre du cours,
   durée, prérequis officiels, objectifs (contenus du programme) et **tableau des étapes**
   entièrement pré-rempli.

Trois modèles d'étapes sont proposés :

| Modèle | Résultat |
|---|---|
| Squelette standard (4 phases) | Mise en situation · Construction des apprentissages · Synthèse / Trace écrite · Évaluation |
| Une étape par contenu du programme | Une ligne du tableau par contenu officiel de la leçon |
| Une étape par leçon de l'unité | Fiche de planification de toute l'unité, une ligne par leçon avec son horaire |

Tout le programme est **bilingue (français / arabe)** : titres des unités, titres des leçons,
prérequis et **les 213 contenus détaillés**. Le remplissage suit la langue du document, ce qui
permet de préparer une jadhadha entièrement en arabe comme entièrement en français.

## Banques de formulations

Le bouton **＋** placé à côté de chaque champ ouvre une liste de formulations prêtes à cocher,
en français et en arabe : objectifs, compétences, activités du professeur, activités de l'élève,
moyens et supports (microscope, loupe binoculaire, data-show, Anagène, cartes géologiques…),
modalités d'évaluation et amorces de situations de départ.

## Fonctionnalités

- **Thème clair / sombre** : le bouton 🌓 de la barre supérieure alterne entre le thème du
  système, le thème clair et le thème sombre ; le choix est mémorisé. La fiche imprimée reste
  toujours sur fond blanc, quel que soit le thème.
- **Bilingue arabe / français** : bascule de l'interface avec passage RTL ↔ LTR automatique.
  La langue du document peut suivre l'interface ou être fixée fiche par fiche.
- **En-tête officiel modifiable** : ministère, Académie Régionale, Direction Provinciale,
  établissement et **logo** (image locale, redimensionnée puis stockée dans le navigateur).
  Bouton « Mémoriser comme défaut » pour réutiliser ces informations dans les fiches suivantes.
- **Identification** : niveau (TCS, 1BAC SE, 1BAC LSH, 2BAC PC, 2BAC SVT — ou niveau libre),
  matière, unité/module, titre du cours, durée, professeur, numéro de fiche, année scolaire
  (calculée automatiquement).
- **Rubriques** : « Pré acquis » et « Objectifs d'apprentissage » côte à côte, plus une
  situation de départ facultative. Une ligne de saisie = un paragraphe ; les rubriques vides
  ne sont pas imprimées.
- **Tableau des axes** reprenant la mise en page de référence : **Axes · Objectifs ·
  Activités (Professeur / Apprenant) · Support · Évaluation**, en-tête sur deux niveaux,
  colonne « Compétences » disponible en option. Chaque axe reçoit une **couleur** et peut
  être suivi d'une bande **« Le contenu de la section : … »** sur toute la largeur.
  Axes déplaçables, duplicables et supprimables.
- **Verbes d'action en gras** : le verbe en tête de ligne (Mettre, Connaître, Propose,
  Décrit, يحدد, يقارن…) est mis en gras automatiquement à l'impression.
- **Aperçu en direct** au format A4 paysage, avec zoom et ajustement automatique.
- **Pagination automatique** : les étapes qui ne tiennent pas passent à la page suivante avec
  répétition des en-têtes de colonnes ; option de répétition de l'en-tête officiel.
- **Remplissage de la page** : les lignes (ou les rubriques) sont étirées pour occuper toute la
  hauteur utile — pas de grands espaces vides en bas de page.
- **Mise en page réglable** : en-tête officiel avec logo (optionnel), pied de page à
  3 colonnes *Niveau / Année scolaire / Pr : …* avec numérotation **« Page X / Y »**, et
  ligne de clôture en fin de fiche — chacun activable ou non.
- **Plusieurs fiches** enregistrées localement (`localStorage`) : créer, dupliquer, renommer,
  supprimer, rechercher ; sauvegarde automatique à chaque modification (Ctrl+S force la
  sauvegarde).
- **Export / import JSON** pour la sauvegarde de secours ou le transfert vers un autre ordinateur.

## Remarques

- Les données restent sur le poste de travail : rien n'est envoyé sur internet. Vider les
  données du navigateur efface les fiches → penser au bouton **Exporter**.
- Pour une utilisation sur plusieurs postes, copier simplement le fichier `index.html`.
- Aucune information personnelle n'est incluse dans le fichier : chaque professeur saisit son
  propre en-tête, qui n'est enregistré que dans son navigateur.
- Source du programme intégré : « Programmes des sections internationales du baccalauréat
  marocain — Option français — Discipline : Sciences de la Vie et de la Terre », Ministère de
  l'Éducation Nationale et de la Formation Professionnelle, 29-30 avril 2015. Les niveaux couverts
  sont TCS, 1BAC SE, 1BAC LSH, 2BAC SVT et 2BAC PC.
