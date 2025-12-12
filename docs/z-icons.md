---
icon: material/emoticon-happy
---

# Icônes

Zensical supporte plusieurs sources d’icônes : Lucide, Material, FontAwesome. Les icônes peuvent être utilisées dans le thème, la nav et le front‑matter des pages.

## Icônes Lucide (thème et toggles)

Utilisez la syntaxe `lucide/<nom>` :

- `lucide/sun`
- `lucide/moon`
- `lucide/book-open`
- `lucide/github`

Exemple pour le toggle des palettes :

```toml
[[project.theme.palette]]
scheme = "default"
toggle.icon = "lucide/sun"
```

## Icônes Material (front‑matter des pages)

Ajoutez une icône près du titre de la page et dans la nav en définissant le front‑matter :

```yaml
---
icon: material/format-title
---
```

Choisissez l’icône sur le catalogue Material (noms en kebab‑case).

## FontAwesome (liens sociaux)

Ajoutez des icônes sociales dans la section `extra` :

```toml
[[project.extra.social]]
icon = "fontawesome/brands/github"
link = "https://github.com/user/repo"
```

## Bonnes pratiques

- Restez cohérent dans le style (évitez de mélanger trop de familles)
- Utilisez des icônes explicites et accessibles
- Vérifiez le contraste et la taille pour la lisibilité
