---
title: Layouts
version: 1.0.0
status: Official
repository: brand
author: VestigiumLabs Designer
---

# Layouts

## Introduction

Les layouts définissent la structure des pages de VestigiumLabs.

Ils ne définissent pas le contenu.

Ils définissent :

- l'organisation visuelle ;
- les espacements ;
- la hiérarchie ;
- les largeurs ;
- les comportements responsive.

Chaque nouvelle page du laboratoire doit être construite à partir de ces layouts.

---

# Principes

Les pages suivent toujours le même rythme.

Navigation

↓

Hero

↓

Contenu principal

↓

Sections

↓

Footer

Cette structure ne doit être modifiée que lorsqu'un besoin fonctionnel le justifie.

---

# Largeur

## Full Width

Utilisée uniquement pour :

- Hero
- Bannière
- Footer

Largeur :

100%

---

## Content Width

Toutes les sections utilisent une largeur maximale.

```
max-width : 1280 px
```

Le contenu est toujours centré.

---

## Reading Width

Les articles techniques utilisent une largeur plus faible.

```
max-width : 760 px
```

Cette largeur améliore le confort de lecture.

---

# Espacements

Entre deux sections :

96 px

Entre un titre et son contenu :

32 px

Entre deux composants :

24 px

Entre deux éléments liés :

16 px

Jamais d'espacement arbitraire.

---

# Page d'accueil

## Structure

```
┌──────────────────────────────────────────┐
│ NAVIGATION                               │
├──────────────────────────────────────────┤
│ HERO                                    │
├──────────────────────────────────────────┤
│ DOMAINES D'EXPERTISE                    │
├──────────────────────────────────────────┤
│ PROJETS                                 │
├──────────────────────────────────────────┤
│ RECHERCHES                              │
├──────────────────────────────────────────┤
│ ARTICLES                                │
├──────────────────────────────────────────┤
│ APPEL À CONTRIBUTION                    │
├──────────────────────────────────────────┤
│ FOOTER                                  │
└──────────────────────────────────────────┘
```

---

# Navigation

Hauteur

72 px

Toujours visible.

Logo à gauche.

Menu à droite.

Sur mobile :

Menu hamburger.

---

# Hero

Le Hero utilise la bannière officielle.

Composition :

```
Logo

Titre

Sous-titre

Deux boutons

Illustration
```

Le Hero ne dépasse jamais une hauteur de 720 px.

---

# Section

Toutes les sections suivent la même structure.

```
Titre

Sous-titre

Contenu
```

Le titre est toujours aligné avec le contenu.

---

# Grille Desktop

12 colonnes.

Gouttière :

24 px

Marges :

48 px

---

# Grille Tablet

8 colonnes.

Gouttière :

24 px

---

# Grille Mobile

4 colonnes.

Gouttière :

16 px

---

# Cartes

Desktop

```
4 cartes par ligne
```

Tablet

```
2 cartes
```

Mobile

```
1 carte
```

---

# Articles

Desktop

```
3 colonnes
```

Tablet

```
2 colonnes
```

Mobile

```
1 colonne
```

---

# Documentation

Lecture confortable.

Sommaire fixe.

Largeur réduite.

Bloc de code pleine largeur.

---

# Dashboard futur

Prévu pour :

- agents
- administration
- statistiques

Layout :

Sidebar

+

Content

---

# Footer

Toujours identique.

```
Logo

Navigation

GitHub

Licence

Copyright
```

---

# Responsive

## Desktop

≥1280 px

Disposition horizontale.

---

## Laptop

1024–1279 px

Même structure.

Espacements réduits.

---

## Tablet

768–1023 px

Deux colonnes.

---

## Mobile

≤767 px

Une colonne.

---

# Règles

Jamais plus de :

- 12 colonnes Desktop
- 8 Tablet
- 4 Mobile

Toutes les pages utilisent les mêmes marges.

Aucune page ne définit sa propre grille.

---

# Layouts disponibles

Home

Projects

Research

Documentation

Article

Project

About

Search

404

Legal

Tous ces layouts doivent dériver des mêmes fondations.

---

# Évolution

Toute nouvelle page doit réutiliser un layout existant.

Si ce n'est pas possible, un nouveau layout peut être créé uniquement après validation.

L'objectif est de limiter le nombre de variantes afin de préserver la cohérence du Design System.
