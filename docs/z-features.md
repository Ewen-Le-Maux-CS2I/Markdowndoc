---
icon: material/flash
---

# Features

Les features se configurent dans `[project.theme]` via la clé `features = [ ... ]`. Elles permettent d’activer des comportements utiles dans la navigation, le code, et l’interface.

## Exemple de configuration

```toml
[project.theme]
features = [
	"navigation.instant",
	"navigation.instant.prefetch",
	"navigation.footer",
	"navigation.top",
	"navigation.tracking",
	"navigation.indexes",
	"navigation.sections",
	"content.code.copy",
	"content.code.select",
	"content.code.annotate",
	"content.tooltips",
	"content.tabs.link",
	"announce.dismiss"
]
```

## Navigation

- **navigation.instant**: transitions de pages sans rechargement complet
- **navigation.instant.prefetch**: précharge la page au survol d’un lien
- **navigation.footer**: liens « précédent/suivant » en bas de page
- **navigation.top**: bouton « retour en haut »
- **navigation.tracking**: met à jour l’URL selon l’ancre active
- **navigation.indexes**: pages d’index de section
- **navigation.sections**: groupes de navigation au‑dessus de 1220px

## Table des matières (toc)

- **toc.follow**: garde l’ancre active visible dans la toc
- **toc.integrate**: intègre la toc dans la barre latérale

## Code

- **content.code.copy**: bouton pour copier le code
- **content.code.select**: sélection de lignes par bouton
- **content.code.annotate**: annotations/astuces sur des lignes de code

## Contenus et UI

- **content.tooltips**: tooltips enrichis
- **content.tabs.link**: synchronise des onglets de contenu de même nom
- **announce.dismiss**: barre d’annonce masquable

## Recommandations

- Activez `navigation.instant` pour une UX fluide
- Ajoutez `navigation.tracking` pour des liens partageables précis
- Servez une doc avec toc intégrée pour les pages longues
