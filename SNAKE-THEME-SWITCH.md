# Passaggio opzionale light/dark

Solo dopo che il workflow genera **entrambi** gli SVG sul branch `output`, sostituisci l'`<img>` nella sezione snake con:

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/annarivalta/annarivalta/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/annarivalta/annarivalta/output/github-snake.svg" />
  <img src="https://raw.githubusercontent.com/annarivalta/annarivalta/output/github-snake.svg" alt="Anna's GitHub contribution snake" width="100%" />
</picture>
```
