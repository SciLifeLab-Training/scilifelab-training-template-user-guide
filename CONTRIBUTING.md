# Contributing

Thank you for helping to improve the SciLifeLab Training Webpage Template
User Guide. This guide explains how to report a problem, how to make a
change, and how the User Guide is written, so that it stays consistent and
easy to follow for beginners.

## Reporting a problem or suggesting an improvement

Open an issue in the repository your problem or idea is about:

| About | For example | Where |
|---|---|---|
| The User Guide | A step that is unclear, a screenshot that is out of date, a broken link, or a missing explanation | [Issues of the User Guide](https://github.com/SciLifeLab-Training/scilifelab-training-template-user-guide/issues) |
| The template | A website that doesn't build, an error message, or a feature you'd like | [Issues of the template](https://github.com/SciLifeLab-Training/scilifelab-training-template/issues) |

Not sure which one? Either is fine: we move issues to the right repository
if needed. You can also email us at
[training@scilifelab.se](mailto:training@scilifelab.se).

For an issue about the User Guide, say which chapter and step it is about,
what you expected, and what happened instead. A screenshot often helps.

## Making a change

1. Fork the repository, or create a branch if you have write access.
2. Edit the `.qmd` file of the chapter. The order of the chapters is set in
   `_quarto.yml`.
3. Preview the User Guide with `quarto preview`, and check that pages,
   links, images and formatting look as expected.
4. Open a pull request against `main`, with a short description of the
   change.

Changes merged into `main` are published automatically. Don't edit the
`gh-pages` branch: it holds the published website, and is overwritten with
every publish.

If your change follows a change in the template, mention the template pull
request or release, so the two can be checked together.

## How the User Guide is written

The User Guide is written for trainers with no experience of Git, Python
or Quarto. Please keep to these conventions.

### Language

- **Plain language:** short sentences, everyday words, and *you* for the
  reader. Explain a technical term the first time it appears.
- **Names on screen in bold:** buttons, menus and tabs, for example
  **Sync now** or **Settings → Webhooks**.
- **File names, folders, fields and commands in code:** for example
  `data/course.yml`, `version_doi` or `quarto preview`.
- **Chapters by name, not by number:** write *see
  [Training instances](training-instances.qmd)*, not *see chapter 6*.
  Chapter numbers change when chapters are added.
- **Branches by their full name**, for example **main** or
  **release-2706**, and say which branch each step happens on.

### Examples

The User Guide uses one example training throughout: **Introduction to R**,
with the training instances **release-2706** (June 2027) and
**release-2711** (November 2027). Use these in new examples, so the
screenshots and text match.

### Structure of a chapter

- **An introduction** that says what the chapter is about, followed by a
  list of what the reader will learn, linking to its sections.
- **A "Before you start" box** in every chapter about editing files, with
  the rows **Where** (branch and files), **How** (a link to Regular
  workflow) and **For experts** (a link to the cheat sheet). Copy it from
  an existing chapter, and keep the **How** row word for word the same.
- **Numbered steps** for anything the reader does, one action per step.
- **A cheat sheet** at the end of chapters about editing files.

### Headings

- Give a heading an explicit id when it contains punctuation, code or
  special characters, or when other pages link to it:
  `## What is FAIR and why should I care? {#what-is-fair-and-why-should-i-care}`.
- Use `{.unnumbered}` for `###` headings, so only the main sections are
  numbered.
- Don't change an existing id: other chapters may link to it.

### Callouts

| Callout | Use it for |
|---|---|
| `callout-important` | Something that can go wrong, or can't be undone. Keep it open. |
| `callout-note` | Background information. Usually collapsible, with `collapse="true"` and a `title`. |
| `callout-tip` | Help when something doesn't work, or a quicker way. Usually collapsible. |

Use collapsible callouts for information that only some readers need, so
the main steps stay short. Quarto has no `callout-info`.

### Images

- Put images in `images/`, named after the chapter, a number and a short
  description: `fair-17-doibadge.png`. The prefixes in use are `index`,
  `setup`, `workflow`, `structure`, `landing`, `instance`, `ipdatafiles`,
  `ipcontent` and `fair`.
- Give every image alt text with `fig-alt` that describes what it shows,
  for readers who can't see it: `![](images/fair-17-doibadge.png){fig-alt="…"}`.
- Inside a numbered list, indent an image 3 spaces, with a blank line
  above it, so it stays part of its step.
- Take screenshots from the Introduction to R example, and leave out
  personal information.

## Credit and citation

The authors of the User Guide are listed in `CITATION.cff` and
`.zenodo.json`. These files are edited by hand.

If you contribute and would like to be credited, add yourself to both files
in your pull request, or ask us to add you. Also update the Citation section
of `README.md`.

Before each release of the User Guide, update `version` and
`date-released` in `CITATION.cff`, and `version` in `.zenodo.json`.

## Licence

By contributing, you agree that your contributions are made available under
the licence of this repository: CC BY 4.0. See [LICENSE](LICENSE.md).
