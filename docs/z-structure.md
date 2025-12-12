---
icon: material/folder-information
---

# Structure du projet

Cette page explique le rôle des principaux dossiers et fichiers d’un projet Zensical.

## Arborescence type

```
zensical.toml
docs/
  index.md
  images/
  stylesheets/ (optionnel)
  javascripts/ (optionnel)
site/ (généré)
  assets/
  ...
```

## Rôles des dossiers

- **`docs/` : source de contenu**
  - Contient tous les fichiers Markdown (`.md`) de la documentation.
  - Peut être organisé en sous‑dossiers (sections) ; chaque dossier peut avoir un `index.md` pour servir d’aperçu de section (utile avec `"navigation.indexes"`).
  - Les images utilisées dans le contenu peuvent être placées dans `docs/images/` et référencées avec `images/mon-image.png`.
  - Les fichiers additionnels (CSS/JS) référencés via `extra_css` et `extra_javascript` sont relatifs à `docs/`.

- **`zensical.toml` : configuration**
  - Définit le titre du site, la navigation (`nav`), la langue, le thème et les features.
  - Exemple minimal :
    ```toml
    [project]
    site_name = "Ma Doc"
    nav = [ { "Guide" = [ { "Accueil" = "index.md" } ] } ]
    [project.theme]
    language = "fr"
    ```

- **`site/` : sortie du build**
  - Dossier généré par la commande `zensical build`. Il contient le site statique prêt à être publié.
  - Inclut `site/assets/` (CSS/JS/minifiés, workers, etc.).
  - À ne pas modifier à la main. Vous publiez ce dossier tel quel (GitHub Pages, Netlify, Vercel, S3…).

- **`overrides/` (optionnel) : templates personnalisés**
  - À activer via `[project.theme] custom_dir = "overrides"`.
  - Permet de surcharger des partials/blocks du thème pour adapter l’UI.

## Navigation (menu latéral)

- Se définit dans `zensical.toml` via `nav = [ ... ]`.
- Chaque entrée peut être une page (`{"Titre" = "page.md"}`) ou un groupe avec sous‑pages.
- Les icônes des items de nav proviennent du front‑matter des pages (`icon: material/...`).

## Table des matières (On this page)

- Générée automatiquement à partir des titres `##`, `###`, … sur chaque page.
- Options utiles dans `features` : `"toc.follow"` (suivi de l’ancre) et `"toc.integrate"` (intégration à gauche).

## Ressources (CSS/JS personnalisés)

- Ajoutez des fichiers dans `docs/stylesheets/` et `docs/javascripts/`, puis référencez‑les :
  ```toml
  extra_css = ["stylesheets/extra.css"]
  extra_javascript = ["javascripts/extra.js"]
  ```

## Bonnes pratiques

- Écrivez tout le contenu Markdown dans `docs/` ; utilisez des sous‑dossiers pour structurer.
- Ne modifiez pas `site/` manuellement ; reconstruisez avec `zensical build`.
- Définissez la nav explicitement dans `zensical.toml` pour contrôler l’ordre.
- Placez vos images dans `docs/images/` et utilisez des chemins relatifs simples (`images/...`).
- Gardez des titres clairs et des icônes cohérentes via le front‑matter.
