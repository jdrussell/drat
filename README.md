## drat [![Build Status](https://travis-ci.org/eddelbuettel/drat.png)](https://travis-ci.org/eddelbuettel/drat) [![License](http://img.shields.io/badge/license-GPL%20%28%3E=%202%29-brightgreen.svg?style=flat)](http://www.gnu.org/licenses/gpl-2.0.html)

Drat R Archive Template

### Background

The R package ecosystem is one of the cornerstones of the success seen by R.
As of this writing, over 6200 are on [CRAN](http://cran.r-project.org),
several hundred more at [BioConductor](http://www.bioconductor.org) and at
[OmegaHat](http://www.omegahat.org).

Support for multiple repositories is built deeply into R; mostly via the
(default) package `utils`. The
[`update.packages`](http://www.rdocumentation.org/packages/utils/functions/update.packages)
function (along with several others from the `utils` package) can used for these three default
repositories as well as many others with ease. But it seemed that support for
_simple creation and use_ of local repositories was however missing.

Drat tries to help here and support two principal modes:
- *GitHub* by leveraging `gh-pages`
- *Other repos* by using other storage where you can write and provide html access

See the package documentation, or the
[package page](http://dirk.eddelbuettel.com/code/drat.html) for more.

### Getting Started

#### Not yet on CRAN 

One day we may be able to install the package from [CRAN](http://cran.r-project.org) via
`install.packages("drat")` and see the manual pages.

#### In the meantime

For a first installation, do for examples

```{.r}
install.packages("drat", repos="http://eddelbuettel.github.io/drat")
```

After either initial installation, you can add line such as

```
drat:::add("eddelbuettel")
```

to your session or startup files (see `help(Startup)`) and use
`update.packages()` as usual---also reflection the new drat archive.

### Author

Dirk Eddelbuettel 

### License

GPL (>= 2)

