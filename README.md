# Collaborative Programming with GitHub

[![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
[![gh actions](https://github.com/klieret/collaborative-programming-github/actions/workflows/deploy.yml/badge.svg)](https://github.com/klieret/collaborative-programming-github/actions)

> **Note**
> 👉 [**Click here for rendered slides!**](https://klieret.github.io/collaborative-programming-github/) 👈

> **Warning**
> This is **not** the playground repository.
> Pull requests that improve the lecture are much appreciated though!

Slides to introduce collaborative programming with github and git.
The first part of the slides makes extensive use of the github web interface
to provide students with more intuition and flatten the learning curve.
The second part then turns to the command line.

> **Note**
> You can use these slides for your teaching, too (see license)! Contributions are very welcome as well.

Slides originally created for the [CoDaS-HEP 2022 school](https://indico.cern.ch/event/1151367/) (PDF version of the slides available in the release).

## 🧰 Local development

The slides are built with [Slidev](https://github.com/slidevjs/slidev).

To start the slide show locally:

- `npm install`
- `npm run dev`
- visit http://localhost:3030

Edit the [slides.md](./slides.md) to see the changes.

Learn more about Slidev on [documentations](https://sli.dev/).

When contributing, please also set up the pre-commit hooks with

```bash
pre-commit install
```

## Lecture content

> **Warning**
> Timings are entire NONSENSE. Part 1 took 1h25 ;)

Total: 81'

### Part I

* [5'] Opening an issue
* [8'] Fork & commit
* [6'] PR
* [4'] Branches theory
* [10'] Branches practice
* [10'] Merge conflicts

Total: 43'

### Part II

* [6'] Init repo
* [6'] First commit
* [4'] Multiple files
* [5'] Branches
* [7'] Merging + merge conflicts

Sub-total: 28'

### Part III

* [5'] Git config
* [5'] Remaining slides

Sub-total: 10'
