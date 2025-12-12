---
icon: material/format-pilcrow
---

# Sauts de ligne

Comprendre comment gérer les sauts de ligne en Markdown est essentiel pour un formatage correct.

## Saut de ligne simple

Pour créer un saut de ligne sans commencer un nouveau paragraphe, terminez la ligne avec deux espaces.

### Syntaxe

```markdown
Première ligne  
Deuxième ligne  
Troisième ligne
```

### Rendu

Première ligne  
Deuxième ligne  
Troisième ligne

!!! warning "Attention"
    Les deux espaces à la fin de la ligne sont invisibles mais nécessaires !

## Nouveau paragraphe

Pour créer un nouveau paragraphe, laissez une ligne vide.

### Syntaxe

```markdown
Premier paragraphe avec du texte.

Deuxième paragraphe avec du texte.

Troisième paragraphe avec du texte.
```

### Rendu

Premier paragraphe avec du texte.

Deuxième paragraphe avec du texte.

Troisième paragraphe avec du texte.

## Différences

### Saut de ligne simple (2 espaces)
Texte plus proche  
Sans espace vertical important  
Comme des lignes dans un paragraphe

### Nouveau paragraphe (ligne vide)

Texte avec plus d'espace vertical

Plus de séparation visuelle

Comme des paragraphes distincts

## Alternatives

Certains éditeurs Markdown supportent aussi :

### Backslash à la fin de ligne

```markdown
Première ligne\
Deuxième ligne
```

### Balise HTML `<br>`

```markdown
Première ligne<br>
Deuxième ligne
```

## Bonnes pratiques

- Utilisez des paragraphes (ligne vide) pour séparer des idées différentes
- Utilisez des sauts de ligne simples (2 espaces) pour des éléments liés
- Dans les listes et les tableaux, les retours à la ligne se comportent différemment
- Soyez cohérent dans votre utilisation des sauts de ligne
- Activez l'affichage des espaces invisibles dans votre éditeur pour voir les deux espaces
