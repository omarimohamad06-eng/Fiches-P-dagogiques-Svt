# جذاذات SVT — Générateur de fiches pédagogiques

Application web **autonome** (un seul fichier `index.html`, aucun serveur, aucune connexion
internet, aucune bibliothèque externe) pour préparer et imprimer des **جذاذات / fiches de
préparation de cours** de SVT.

Contexte pré-rempli : **Pr : Omari Mohammed** — Lycée Qualifiant Tilmi — Direction Provinciale
de Tinghir — AREF Drâa-Tafilalet.

## Utilisation

1. Télécharger `index.html`.
2. L'ouvrir par double-clic dans n'importe quel navigateur (Chrome, Edge, Firefox).
3. Saisir la fiche : tout est enregistré automatiquement dans le navigateur.
4. Bouton **Imprimer / PDF** → dans la fenêtre du navigateur choisir :
   *Destination* « Enregistrer au format PDF », *Format* A4, *Orientation* **Paysage**,
   *Marges* « Aucune », et cocher **« Graphiques d'arrière-plan »**.

## Fonctionnalités

- **Bilingue arabe / français** : bascule de l'interface avec passage RTL ↔ LTR automatique.
  La langue du document peut suivre l'interface ou être fixée fiche par fiche.
- **En-tête officiel modifiable** : ministère, Académie Régionale, Direction Provinciale,
  établissement et **logo** (image locale, redimensionnée puis stockée dans le navigateur).
  Bouton « Mémoriser comme défaut » pour réutiliser ces informations dans les fiches suivantes.
- **Identification** : niveau (TCS, 1BAC SE, 1BAC LSH, 2BAC PC, 2BAC SVT — ou niveau libre),
  matière, unité/module, titre du cours, durée, professeur, numéro de fiche, année scolaire
  (calculée automatiquement).
- **Rubriques** : compétences et objectifs visés, prérequis, situation de départ /
  situation-problème. Une ligne de saisie = une puce ; les rubriques vides ne sont pas imprimées.
- **Tableau des étapes** : Objectifs · Compétences · Activité du professeur · Activité de
  l'élève · Moyens et supports · Évaluation (+ colonne « Étape » facultative). Étapes
  déplaçables, duplicables et supprimables.
- **Aperçu en direct** au format A4 paysage, avec zoom et ajustement automatique.
- **Pagination automatique** : les étapes qui ne tiennent pas passent à la page suivante avec
  répétition des en-têtes de colonnes ; option de répétition de l'en-tête officiel.
- **Remplissage de la page** : les lignes (ou les rubriques) sont étirées pour occuper toute la
  hauteur utile — pas de grands espaces vides en bas de page.
- **Pied de page sur chaque page** : 3 colonnes *Niveau / Année scolaire / Pr : …* et
  numérotation **« Page X / Y »**.
- **Plusieurs fiches** enregistrées localement (`localStorage`) : créer, dupliquer, renommer,
  supprimer, rechercher ; sauvegarde automatique à chaque modification (Ctrl+S force la
  sauvegarde).
- **Export / import JSON** pour la sauvegarde de secours ou le transfert vers un autre ordinateur.

## Remarques

- Les données restent sur le poste de travail : rien n'est envoyé sur internet. Vider les
  données du navigateur efface les fiches → penser au bouton **Exporter**.
- Pour une utilisation sur plusieurs postes, copier simplement le fichier `index.html`.
