# Contributing to Project Terra

Project Terra is a shared learning, experimentation, and development laboratory.

The goal is not only to build an application, but also to learn the technologies and scientific methods required to build it.

## Basic Workflow

1. Pick an experiment, task, or learning objective.
2. Create a branch.
3. Work and experiment locally.
4. Document important findings.
5. Add tests when appropriate.
6. Open a pull request.
7. Review the changes with the team.
8. Merge after the work is ready.

## Branches

Use descriptive branch names.

Examples:

- `experiment/modis-temperature`
- `experiment/mann-kendall`
- `feature/backend-api`
- `feature/map-visualization`
- `fix/data-validation`
- `docs/dataset-mod11a2`

## Experiments

Experimental code belongs in `experiments/`.

Do not worry about making experimental code perfect.

If an experiment becomes useful and validated, refactor the reusable parts into `src/`.

## Notebooks

Use `notebooks/` for exploration, visualization, and learning.

Important findings should be documented in `docs/`.

## Data

Do not commit large raw NASA datasets.

Use:

- `data/raw/` for local raw datasets
- `data/processed/` for local processed datasets
- `data/samples/` for small reproducible datasets

## Pull Requests

A pull request should explain:

- What was changed
- Why it was changed
- What was tested
- Important findings or limitations

## Learning

Questions are encouraged.

Project Terra is a collaborative learning environment. Team members should share useful resources, explanations, mistakes, and discoveries.