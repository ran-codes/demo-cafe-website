# Sandbox Cafe

Demo repo for the UHC Sandbox session **"GitHub and Agents — a match made in heaven"** (2026-10-20).

A tiny cafe-menu website that non-coders change through GitHub:

**issue → agent opens PR → humans review → merge → site auto-publishes**

Live site: https://ran-codes.github.io/demo-cafe-website/

## How to play

1. [File an issue](https://github.com/ran-codes/demo-cafe-website/issues/new) describing what you want on the menu.
2. An agent picks it up, opens a branch, and submits a pull request.
3. Humans review the PR and merge it.
4. The site rebuilds and publishes within about two minutes.

The `main` branch **is** the cafe. Whatever is on `main` is what the chefs cook.

## Layout

- `quarto/` — the whole website. See [`quarto/README.md`](quarto/README.md).
- `.github/workflows/quarto.yml` — `quarto-check` renders every PR; `quarto-deploy` publishes `main` to `gh-pages`.
- `CLAUDE.md` — rules for the agent.

Content is modeled on the [Panama City cupcake cafe](https://github.com/SALURBAL-Climate/panama-city-workshop-cafe-demo). CI/CD and layout are copied from `Drexel-UHC/cdc-correctional-facilities-hcv`.
