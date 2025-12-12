---
icon: material/backspace
---

# Caractères d'échappement

Pour afficher des caractères qui ont une signification spéciale en Markdown, vous devez les échapper avec un backslash (`\`).

## Syntaxe

```markdown
Use backslash to escape: \* \_ \# \` \\ \[ \] \( \) \{ \} \. \! \+ \-
```

## Caractères à échapper

Les caractères suivants ont une signification spéciale en Markdown :

| Caractère | Signification normale | Comment l'échapper |
|:---------:|----------------------|-------------------|
| `*`       | Italique/Gras        | `\*`              |
| `_`       | Italique/Gras        | `\_`              |
| `#`       | Titre                | `\#`              |
| `` ` ``   | Code                 | `` \` ``          |
| `\`       | Échappement          | `\\`              |
| `[`       | Lien                 | `\[`              |
| `]`       | Lien                 | `\]`              |
| `(`       | Lien                 | `\(`              |
| `)`       | Lien                 | `\)`              |

## Exemples

### Sans échappement

```markdown
*ceci sera en italique*
```

*ceci sera en italique*

### Avec échappement

```markdown
\*ceci ne sera pas en italique\*
```

\*ceci ne sera pas en italique\*

## Cas pratiques

### Afficher des symboles mathématiques

Pour écrire : 2 \* 3 = 6

```markdown
2 \* 3 = 6
```

### Afficher du code Markdown

Pour montrer comment créer un titre :

```markdown
\# Ceci est un titre
```

Résultat : \# Ceci est un titre

### Prix en dollars

Prix: \$19.99

```markdown
Prix: \$19.99
```

## Bonnes pratiques

- N'échappez que quand nécessaire
- Dans les blocs de code, l'échappement n'est généralement pas nécessaire
- Pour afficher un backslash littéral, utilisez `\\`
- Dans les titres et le texte normal, la plupart des caractères n'ont pas besoin d'être échappés
