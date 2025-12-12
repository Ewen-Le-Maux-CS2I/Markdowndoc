---
icon: material/view-list
---

# Navigation

Une bonne navigation aide l’utilisateur à se situer et à parcourir rapidement la doc.

## Navigation explicite (recommandée)

Définissez le menu dans `zensical.toml` pour contrôler ordre et libellés :

```toml
nav = [
  { "Getting Started" = [
    { "Introduction" = "index.md" },
    { "Install" = "setup.md" }
  ] },
  { "Guide" = [
    { "Concepts" = "guide/concepts.md" },
    { "CLI" = "guide/cli.md" }
  ] }
]
```

## Navigation implicite

Si `nav` est absent, Zensical construit le menu depuis l’arborescence `docs/`. Utile pour prototyper, moins pour un site final car l’ordre peut être imprévisible.

## Index de section

Activez `"navigation.indexes"` pour attacher une page d’index à une section. Placez une page nommée `index.md` dans le dossier de la section et référencez-la dans le groupe.

## Table des matières (On this page)

- Générée automatiquement à partir des titres `##`, `###`, …
- Options :
  - `"toc.follow"` pour faire suivre l’ancre active
  - `"toc.integrate"` pour intégrer la toc dans la barre de gauche

## Fils d’Ariane (breadcrumbs)

Activez `"navigation.path"` pour afficher le chemin de navigation au-dessus du titre de page.

## Navigation instantanée

`"navigation.instant"` intercepte les liens internes pour des transitions sans rechargement complet. Ajoutez `"navigation.instant.prefetch"` pour précharger au survol.

## Bonnes pratiques

- Gardez des libellés courts et clairs
- Évitez trop de profondeur (max 3 niveaux)
- Préférez la nav explicite pour la maîtrise de l’ordre
- Ajoutez des pages d’index pour les sections riches
