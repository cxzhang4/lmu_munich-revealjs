# LMU-themed Revealjs Extension For Quarto

A [quarto extension](https://quarto.org/docs/extensions/) featuring an [LMU-inspired theme](https://www.lmu.de/de/die-lmu/struktur/zentrale-universitaetsverwaltung/kommunikation-und-presse/lmu-brand-guide/designgrundsaetze/farben/) for the [reveal.js format](https://quarto.org/docs/presentations/revealjs/).

# Credit for development goes to James Balamuta and any other developers of the Illinois theme. (Also, being able to refer to Kat Hoffman's similar changes made this easier.

# The following is essentially copied from the [original README](https://github.com/coatless-quarto/illinois-revealjs)

[![](title-slide-quarto-lmu_munich.png)](http://quarto.thecoatlessprofessor.com/illinois-revealjs/)

See the included [template.qmd](template.qmd) file for an example of the theme and integration into Quarto or explore the rendered version of the base version [here](http://quarto.thecoatlessprofessor.com/illinois-revealjs/).

## Installing

You can obtain a copy of the extension by using:

```bash
quarto use template cxzhang4/lmu_munich-revealjs
```

This will install the extension and create an example qmd file that
you can use as a starting place for your presentation slides.

## Using

Once the extension is installed, you can use the extension by setting the `format` inside of the document header to `lmu_munich-revealjs`.

```markdown
---
title: A title
subtitle: A subtitle
format:
  lmu_munich-revealjs: default
author:
  - name: Your Name
    orcid: 0000-0000-0000-0000
    email: alias@email.com
    affiliations: Your Institution
date: last-modified
---
```

If you wanted to use other [reveal.js features in quarto](https://quarto.org/docs/presentations/revealjs/), add the options under the `lmu_munich-revealjs` format. For example, we can use the [`chalkboard`](https://quarto.org/docs/presentations/revealjs/presenting.html#chalkboard) feature by setting:

```yaml
format:
  lmu_munich-revealjs:
    chalkboard: true
```

## Developer Notes

We created the quarto extension for the revealjs format by using:

```sh
quarto create extension format:revealjs
```

From there, we incorporated a modified version of the [Beamer Metropolis](https://github.com/matze/mtheme) that was ported into a [Quarto theme](https://codeberg.org/pat-s/quarto-metropolis) by [Patrick Schratz](https://pat-s.me/) ([Post](https://pat-s.me/quarto-metropolis-theme/)).

## Acknowledgements

This theme is built ontop of the design and implementation work of [Matthias Vogelgesang](https://bloerg.net/) ([Beamer Metropolis](https://github.com/matze/mtheme)) and [Patrick Schratz](https://pat-s.me/) ([Quarto Metropolis theme](https://codeberg.org/pat-s/quarto-metropolis)).

We also appreciate for [Shafayet Khan Shafee](https://github.com/shafayetShafee) for making available an alternative port known as [`metropolis-revealjs`](https://github.com/shafayetShafee/metropolis) based on the gist containing [`metropolis.css`](https://gist.github.com/vhodges/e37893eecde3f3333150) by [Vince Hodges](https://github.com/vhodges).

Additionally, we relied upon the following documentation:

- [Quarto Documentation: Custom Formats](https://quarto.org/docs/extensions/formats.html)
- [Quarto Revealjs Clean Theme](https://github.com/grantmcdermott/quarto-revealjs-clean) by [Grant McDermott](https://github.com/grantmcdermott)
