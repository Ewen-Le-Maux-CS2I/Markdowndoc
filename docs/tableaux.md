---
icon: material/table
---

# Tableaux

Les tableaux permettent d'organiser des données en lignes et colonnes.

## Syntaxe de base

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data     | Data     |
| Row 2    | Data     | Data     |
```

## Rendu

| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data     | Data     |
| Row 2    | Data     | Data     |

## Alignement

Vous pouvez aligner le texte dans les colonnes :

```markdown
| Gauche | Centre | Droite |
|:-------|:------:|-------:|
| A      | B      | C      |
| 1      | 2      | 3      |
```

### Rendu

| Gauche | Centre | Droite |
|:-------|:------:|-------:|
| A      | B      | C      |
| 1      | 2      | 3      |

## Exemple pratique

| Langage    | Extension | Usage principal      |
|:-----------|:---------:|---------------------:|
| Python     | .py       | IA, Data Science     |
| JavaScript | .js       | Web Development      |
| Java       | .java     | Applications métier  |
| C++        | .cpp      | Systèmes, Gaming     |

## Bonnes pratiques

- Utilisez des espaces pour aligner les colonnes (améliore la lisibilité du code source)
- Évitez les tableaux trop larges ou complexes
- Pour les données complexes, envisagez d'autres formats (listes, sections)
- Les tirets dans la ligne de séparation peuvent être de n'importe quelle longueur (minimum 3)
