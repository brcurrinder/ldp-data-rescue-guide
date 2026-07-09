# The Living Data Project: Data Rescue Guidebook

This repository contains a Quarto book intended to support interns, graduate student data rescue teams, and other individuals participating in the Living Data Project, an initiative of the Canadian Institute of Ecology and Evolution (CIEE).

## Goals

The guide helps individuals to:

- Assess legacy datasets
- Create high-quality metadata
- Apply reproducible workflows
- Prepare datasets for publication on DataStream and other repositories
- Practice responsible data stewardship

## Repository Structure

- `chapters/` — guide content
- `images/` — figures and screenshots
- `templates/` — downloadable templates
- `_quarto.yml` — Quarto book configuration

### Reproducible R package environments

For chapters that incorporate R code, this guidebook uses `renv` to make the R package environment more reproducible. The package versions needed to run the code are recorded in the project’s `renv.lock` file.

If you clone or download the project repository and open it in RStudio, you can restore the package environment with:

```r
renv::restore()
```

You do not need to run this command when reading the online version of the guidebook. It is only needed if you want to run the code locally in your own RStudio session.

When new packages are added to the project, the project maintainer should update the lockfile with:

```r
renv::snapshot()
```

This helps ensure that the book can be rendered consistently on different computers and in GitHub Actions.

