
## Historique

| Version | Date | Auteur | Description |
|---------|------|--------|-------------|
| 1.0 | 2026-07-08 | Designer | Création du document |
| 1.0.1 | 2026-07-08 | Designer | Simplification rédactionnelle, suppression des anticipations et clarification des règles |

---
title: UI Components
version: 1.0.0
status: Official
repository: brand
author: VestigiumLabs Designer
reviewer: Laboratory Director
---

# UI Components

## Introduction

Les composants présentés dans ce document constituent la bibliothèque officielle de VestigiumLabs.

Ils doivent être réutilisés tels quels afin de garantir :

- une interface cohérente ;
- une maintenance simplifiée ;
- une expérience utilisateur homogène ;
- une implémentation prévisible.

Les composants ne doivent pas être recréés lorsqu'un composant existant répond déjà au besoin.

---

# Principes généraux

Tous les composants respectent les règles suivantes.

## Cohérence

Les couleurs proviennent exclusivement du Design System.

Les espacements suivent la grille de 8 px.

Les typographies sont définies dans `01-Design-System-v1.md`.

---

## Accessibilité

Chaque composant doit être utilisable :

- au clavier ;
- à la souris ;
- au tactile.

Les états Focus doivent toujours être visibles.

Les composants interactifs possèdent une zone cliquable minimale de 44 × 44 px.

---

## Responsive

Les composants s'adaptent à la largeur disponible.

Ils ne changent jamais de comportement.

Seule leur disposition évolue.

---

# Button

## Objectif

Déclencher une action.

Les actions sont généralement réalisées avec un bouton. La navigation est généralement réalisée avec un lien.

---

## Anatomie

```
┌─────────────────────┐
│  Icône   Texte      │
└─────────────────────┘
```

Éléments :

- Conteneur
- Libellé
- Icône (optionnelle)

---

## Dimensions

Hauteur :

48 px

Padding horizontal :

24 px

Radius :

8 px

---

## Variantes

### Primary

Usage :

Action principale de la page.

Couleurs

Fond :

Accent Blue

Texte :

White

Maximum :

Par défaut, une section comporte une seule action principale.

---

### Secondary

Usage

Action secondaire.

Fond transparent.

Contour bleu.

---

### Ghost

Utilisé dans les interfaces très chargées.

Pas de contour.

Fond transparent.

---

### Danger

Utilisé uniquement pour :

- supprimer
- réinitialiser
- effacer

Jamais pour une action normale.

---

## États

Default

Hover

Focus

Pressed

Disabled

Loading

Chaque état possède une différence visuelle identifiable.

---

## Icône

Les icônes sont placées :

avant le texte

ou

après le texte

Jamais seules sauf pour un Icon Button.

---

## Bonnes pratiques

✔ Utiliser un verbe.

✔ Maximum trois mots.

✔ Une action = un bouton.

---

## À éviter

✘ OK

✘ Cliquez ici

✘ Plus

✘ Bouton sans libellé

---

## Accessibilité

Focus visible.

Contraste AA.

Navigation clavier.

---

## Implémentation

Un bouton ne contient jamais un lien HTML.

Une balise `<button>` déclenche une action.

Une balise `<a>` change de page.

---

# Card

## Objectif

Présenter un contenu autonome.

Une Card représente toujours un objet.

Exemples :

- Projet
- Article
- Recherche
- Agent
- Documentation

---

## Structure

```
┌──────────────────────────┐
│ Image                    │
│                          │
│ Titre                    │
│ Description              │
│                          │
│ Tags                     │
│                          │
│ Action                   │
└──────────────────────────┘
```

---

## Dimensions

Padding

24 px

Radius

16 px

---

## Variantes

Project Card

Research Card

Documentation Card

Article Card

Agent Card

Toutes partagent la même structure.

---

## Hover

Élévation légère.

Les animations éventuelles doivent rester discrètes et améliorer la compréhension de l'interface.


---

## Bonnes pratiques

Une seule action principale.

Titre court.

Description concise.

---

## À éviter

Deux boutons principaux.

Paragraphes très longs.

Images décoratives.

---

# Badge

## Objectif

Afficher un état.

Exemples

Stable

Experimental

Archived

New

---

## Style

Fond discret.

Texte contrasté.

Radius

999 px

---

## Couleurs

Success

Vert

Warning

Orange

Error

Rouge

Info

Bleu

Neutral

Gris

---

# Tag

## Objectif

Catégoriser un contenu.

Exemple

Blockchain

OSINT

Python

Rust

Docker

---

Un Tag n'est jamais cliquable sauf si un filtrage est proposé.

---

# Input

## Objectif

Saisir une donnée.

---

## Structure

```
Label

┌───────────────────────┐
│                       │
└───────────────────────┘

Helper Text
```

---

## États

Default

Focus

Disabled

Error

Success

---

## Dimensions

Hauteur

48 px

Radius

8 px

---

## Placeholder

Le placeholder n'est jamais utilisé comme label.

Le label est obligatoire.

---

## Messages

Helper Text

Informations complémentaires.

Error

Explique clairement le problème.

Jamais :

"Erreur"

Toujours :

"Le champ Email est obligatoire."

---

# Checkbox

Usage

Choix multiples.

Jamais utilisée seule.

Toujours accompagnée d'un libellé.

---

# Radio

Usage

Choix unique.

Toujours présentées en groupe.

---

# Toggle

Utilisé uniquement pour :

Activer

Désactiver

Jamais pour confirmer une action.

---

# Search

Champ spécialisé.

Toujours précédé d'une icône.

---

# Avatar

Utilisé uniquement pour :

- agents IA
- contributeurs
- auteurs

Jamais décoratif.

---

# Divider

Permet de séparer deux groupes.

Épaisseur :

1 px

Couleur :

Border Default

---

# Empty State

Chaque page vide possède :

- une illustration simple
- un titre
- une explication
- une action

Jamais une page blanche.

---

# Loading

Deux composants autorisés :

Spinner

Skeleton

Le choix dépend du contexte d'utilisation.

---

# Principes d'évolution

Tout nouveau composant doit :

répondre à un besoin réel ;

être documenté ;

être réutilisable ;

respecter les fondations du Design System.

Aucun composant ne doit être ajouté uniquement pour répondre à un besoin ponctuel.
