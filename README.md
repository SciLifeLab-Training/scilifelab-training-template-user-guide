# SciLifeLab Training Webpage Template User Guide

This repository contains the User Guide for the
**[SciLifeLab Training Webpage Template](https://scilifelab-training.github.io/scilifelab-training-template/)**:
a ready-made, SciLifeLab-branded website for your training, built with
Quarto and published with GitHub Pages. With the template, you create,
publish and maintain a FAIR website for your training: findable,
citable and easy to reuse.

## Read the User Guide

The published User Guide is available at:

**[SciLifeLab Training Webpage Template User Guide](https://scilifelab-training.github.io/scilifelab-training-template-user-guide/)**

The guide explains, step by step, how to:

- set up your own copy of the template, and publish it as a website;
- make changes, preview them and publish them;
- understand how the repository is organised;
- fill in the landing page of your training;
- create training instances, and add them to the landing page;
- fill in the website of a training instance, and add your training
  materials and instructor notes;
- make your training FAIR, and optionally publish it on Zenodo.

No experience with Git, Python or Quarto is needed.

## The template

The template itself is maintained in a separate repository:

**[SciLifeLab Training Webpage Template](https://github.com/SciLifeLab-Training/scilifelab-training-template)**

If you want to use the template, start with the published User Guide
rather than the files in this repository.

## Working on the User Guide locally

The User Guide is a [Quarto](https://quarto.org/) book.

After cloning this repository, open its folder, and preview the guide
with:

```bash
quarto preview
```

To render the complete guide without starting a preview, run:

```bash
quarto render
```

The rendered website is created on your computer: don't edit it
directly. Make your changes in the `.qmd` files instead.

## Publishing

The User Guide is published with GitHub Pages.

Changes pushed to the `main` branch are rendered and published
automatically by the GitHub Actions workflow in:

```text
.github/workflows/publish.yml
```

The published website is kept on the `gh-pages` branch. Don't edit the
`gh-pages` branch directly.

## Contributing

To improve the User Guide, edit the relevant `.qmd` files in this
repository.

Before you commit, preview the guide on your computer, and check that
pages, links, images and formatting look as expected.

## Citation

If you reuse the SciLifeLab Training Webpage Template User Guide, please
cite it as:

> Luijten, I. (2026). *SciLifeLab Training Webpage Template User Guide*
> (v1.0.0-alpha). Zenodo. https://doi.org/XX.XXXX/zenodo.XXXXX

## Licence

Unless otherwise stated, the SciLifeLab Training Webpage Template User
Guide is licensed under the
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)
licence.
