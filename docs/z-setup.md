---
icon: material/wrench-cog
---

# Installation & Setup

## Prérequis

- Python 3.10+
- `pip` installé
- Un éditeur (VS Code recommandé)

## Installer Zensical

```bash
pip install zensical
```

Vérifiez l’installation :

```bash
zensical --version
```

## Initialiser un projet minimal

1. Créez le fichier `zensical.toml` à la racine.
2. Créez le dossier `docs/` et un fichier `index.md`.

Exemple de `docs/index.md` :

```markdown
---
icon: material/home
---

# Bienvenue

Votre documentation Zensical est prête !
```

## Exemple de `zensical.toml`

```toml
[project]
site_name = "Ma Documentation"
site_description = "Guide utilisateur"
site_author = "Équipe Doc"

nav = [
  { "Guide" = [
    { "Accueil" = "index.md" }
  ] }
]

[project.theme]
language = "fr"
```

## Construire et servir le site

En local :

```bash
zensical build
zensical serve
```

- `build` génère le site dans `site/`
- `serve` lance un serveur avec rafraîchissement à chaud

## Bonnes pratiques de structure

```
docs/
  index.md
  guide/
    intro.md
    usage.md
zensical.toml
```

- Groupez par thème dans `docs/`
- Définissez la nav explicitement pour contrôler l’ordre

## Déploiement

- Hébergement statique (GitHub Pages, Netlify, Vercel, S3)
- Publiez le dossier `site/`

Astuce GitHub Pages :

```bash
git subtree push --prefix site origin gh-pages
```
