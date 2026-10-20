# Sandbox Cafe — agent rules

- Edit only `quarto/`. Never touch `.github/workflows/`.
- One issue per branch per PR. Branch name `<type>/<slug>`, e.g. `feat/matcha-latte`.
- PR body includes `Closes #N`.
- Never commit `quarto/_site/` or `quarto/.quarto/`.
- Pages are plain markdown. Show R as plain `r` fenced code blocks, never `{r}` cells. Nothing executes.
- To add a menu item: add `quarto/food/<slug>.qmd` or `quarto/drinks/<slug>.qmd` with a `title:`, then link it from that section's `index.qmd`.
- Keep every page trivially short. Attention stays on the GitHub loop, not the content.
- Before opening a PR, `cd quarto && quarto render` must succeed.
