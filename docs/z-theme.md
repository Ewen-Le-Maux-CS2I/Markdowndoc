---
icon: material/palette
---

# Thème & Palette

Zensical fournit un thème moderne configurable et des palettes pour le mode clair/sombre.

## Variante de thème

Dans `[project.theme]`, vous pouvez sélectionner la variante (quand disponible) :

```toml
[project.theme]
# variant = "classic" | "modern"
language = "fr"
```

## Palettes de couleurs

Définissez une ou plusieurs palettes, chacune avec une icône de toggle et un nom :

```toml
[[project.theme.palette]]
scheme = "default"
toggle.icon = "lucide/sun"
toggle.name = "Passer en mode sombre"

[[project.theme.palette]]
scheme = "slate"
toggle.icon = "lucide/moon"
toggle.name = "Passer en mode clair"
```

## Polices

```toml
[project.theme.font]
# text = "Inter"
# code = "Jetbrains Mono"
```

## Icônes du thème

Personnalisez le logo affiché et l’icône du dépôt :

```toml
[project.theme.icon]
logo = "lucide/book-open"
repo = "lucide/github"
```

## Favicon et logo

```toml
[project.theme]
favicon = "images/favicon.png"
```

Placez le fichier dans `docs/images/`.

## Overrides de templates

Pour adapter profondément l’UI, activez les overrides :

```toml
[project.theme]
custom_dir = "overrides"
```

Créez `overrides/` et placez vos templates Jinja/HTML. Utilisez‑les pour modifier des blocs spécifiques sans forker le thème.

## Conseils

- Fournissez des labels de toggle compréhensibles
- Testez la lisibilité des couleurs (contraste AA/AAA)
- Choisissez une police monospaced lisible pour le code
