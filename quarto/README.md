# `quarto/`

The whole website lives here. Every page is plain markdown; nothing is executed.

```bash
cd quarto
quarto render     # builds _site/ (gitignored)
quarto preview    # live reload while editing
```

```
quarto/
  _quarto.yml      website config, navbar, theme
  index.qmd        home          → /
  food/index.qmd   food menu     → /food/   (pizza.qmd, pancakes.qmd)
  drinks/index.qmd drinks menu   → /drinks/ (empty, audience fills it)
  code/index.qmd   R scripts shown as code blocks → /code/
```

To add a menu item: add `food/<slug>.qmd` or `drinks/<slug>.qmd` with a `title:`, then link it from that section's `index.qmd`.
