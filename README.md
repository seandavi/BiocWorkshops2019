---
knit: "bookdown::render_book"
title: "The Bioconductor 2019 Workshops Repository"
description: "This book is a central repository for all the workshops submitted to the Bioconductor 2019 Conference"
site: bookdown::bookdown_site
github-repo: Bioconductor/BiocWorkshops2019
documentclass: book
---

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

# Introduction

Author:
    Martin Morgan^[Roswell Park Comprehensive Cancer Center, Buffalo, NY].
    <br/>
Last modified: May 23, 2019

## For Everyone

This book contains workshops used in _R_ / _Bioconductor_
training. The workshops are divided into 3 sections:

- **Learn** (100-series chapters) contains material for beginning
  users of _R_ and _Bioconductor_. The _Bioconductor_-related material
  is relevant even for experienced _R_ users who are new to
  _Bioconductor_.

- **Use** (200-series chapters) contains workshops emphasizing use of
  _Bioconductor_ for common tasks, e.g., bulk RNA-seq differential
  expression, ChIP-seq, single-cell analysis, gene set enrichment, and
  annotation.

- **Develop** (500-series chapters) contains workshops to help expert
  users hone their skills and contribute their domain-specific
  knowledge to the _Bioconductor_ community. These are developer-day workshops.

## For Workshop Authors

To contribute a new workshop, open a [BiocWorkshops issue][] starting with
the `[Workshop]` keyword in the title of the issue. Provide a link to the
repository in the issue message body. You may also include GitHub usernames
of workshop collaborators. For a successful workshop build, adhere to the
following:

1. Package your workshop as an R package. The example package https://github.com/lpantano/dummychapter1 demonstrates all key elements of how your package must be prepared, and also provides an example `.travis.yml` for Continuous Integration against bioc-devel.
2. Include a standard vignette in the vignettes directory
3. Put any extra files (images, .bib) in `inst/vignettes` and reference them
in the vignette using `system.file`
4. Number **3** requires package chapter installation before vignette build or
`build_vignettes=TRUE` when building the package.
5. Use only one top-level section (`#`), for the title of your workshop. All other sections must be second-level (`##`) or lower. You may find the [usage section of the Bookdown documentation](https://bookdown.org/yihui/bookdown/usage.html) helpful for background.

### DESCRIPTION

Update the DESCRIPTION file adding packages utilized in your workshop to
the **Imports** field.

## Deadlines for Bioc2019

Please be aware of the following deadlines for the [Bioconductor 2019 Conference][] in New York

- **Mon May 27:** draft workshop materials submitted as an Issue to this Bioconductor GitHub repo
- **Mon June 10:** complete workshop submitted. Only bugfixes / refinements should be made after this point.
- **Mon June 17:** All workshops complete and building without error. No new commits to contributor repos will be incorporated.

[BiocWorkshops issue]: https://github.com/Bioconductor/BiocWorkshops2019/issues
[Bioconductor 2019 Conference]: https://bioc2019.bioconductor.org/

