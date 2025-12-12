---
icon: material/format-list-bulleted
---

# Listes

Markdown supporte les listes ordonnées et non ordonnées, ainsi que les listes imbriquées.

## Listes non ordonnées

### Syntaxe

```markdown
- Item 1
- Item 2
  - Nested item
  - Another nested item
- Item 3
```

### Rendu

- Item 1
- Item 2
  - Nested item
  - Another nested item
- Item 3

!!! tip "Astuce"
    Vous pouvez aussi utiliser `*` ou `+` au lieu de `-` pour les listes non ordonnées.

## Listes ordonnées

### Syntaxe

```markdown
1. First item
2. Second item
3. Third item
   1. Nested item
   2. Another nested item
4. Fourth item
```

### Rendu

1. First item
2. Second item
3. Third item
   1. Nested item
   2. Another nested item
4. Fourth item

## Bonnes pratiques

- Utilisez une indentation de 2 ou 4 espaces pour les éléments imbriqués
- Les numéros dans les listes ordonnées peuvent être tous `1.` - Markdown les numérotera automatiquement
- Laissez une ligne vide avant et après une liste
