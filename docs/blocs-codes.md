---
icon: material/code-braces
---

# Blocs de code

Les blocs de code permettent d'afficher du code source avec une mise en forme appropriée et une coloration syntaxique.

## Syntaxe

````markdown
```javascript
function hello() {
  console.log("Hello, world!");
}
```
````

## Rendu

```javascript
function hello() {
  console.log("Hello, world!");
}
```

## Langages supportés

Vous pouvez spécifier le langage pour activer la coloration syntaxique :

### Python

```python
def greet(name):
    print(f"Hello, {name}!")
    
greet("World")
```

### Java

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### HTML

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ma Page</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

### CSS

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 20px;
}
```

## Bonnes pratiques

- Toujours spécifier le langage pour une meilleure lisibilité
- Indenter correctement votre code
- Utiliser des blocs de code pour tout extrait de plus d'une ligne
- Pour du code inline, utilisez les backticks simples : `code`
