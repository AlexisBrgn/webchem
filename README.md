
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Webchem

<!-- badges: start -->

[![status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
[![CRAN](https://www.r-pkg.org/badges/version/webchem)](https://CRAN.R-project.org/package=webchem)
[![R build
status](https://github.com/ropensci/webchem/workflows/R-CMD-check/badge.svg)](https://github.com/ropensci/webchem/actions)
[![Coverage](https://codecov.io/github/ropensci/webchem/coverage.svg?branch=master)](https://codecov.io/gh/ropensci/webchem/branch/master)
[![Downloads](https://cranlogs.r-pkg.org/badges/webchem)](https://cran.r-project.org/package=webchem)
[![Total
Downloads](https://cranlogs.r-pkg.org/badges/grand-total/webchem?color=blue)](https://cran.r-project.org/package=webchem)

<!-- badges: end -->

`webchem` is a R package to retrieve chemical information from the web.
This package interacts with a suite of web APIs to retrieve chemical
information.

The functions in the package that hit a specific API have a prefix and
suffix separated by an underscore (`prefix_suffix()`). They follow the
format of `source_functionality`, with the exception of functions that
retrieve database identifiers which follow the format of
`get_identifier`. e.g.`cs_compinfo` uses ChemSpider to retrieve compound
informations and `get_csid()` retrieves ChemSpider IDs.

## Chemical databases currently accessed by webchem

At least some of the data in the following sources is accesible through
`webchem` functions. To learn more about what is available, browse the
documentation
[here](https://docs.ropensci.org/webchem/reference/index.html).

- [BCPC Compendium of Pesticide Common
  Names](https://pesticidecompendium.bcpc.org) (formerly Alan Wood’s
  Compendium of Pesticide Common Names)
- [ChEBI](https://www.ebi.ac.uk/chebi/)
- [Chemical Identifier Resolver
  (CIR)](https://cactus.nci.nih.gov/chemical/structure)
- [Chemical Translation Service (CTS)](http://cts.fiehnlab.ucdavis.edu/)
- [ChemSpider](http://www.chemspider.com/) (requires an [API
  token](https://developer.rsc.org/))
- [ETOX](http://webetox.uba.de/webETOX/index.do)
- [Flavornet](http://www.flavornet.org)
- [NIST](https://webbook.nist.gov) (currently gas chromatography
  retention indices only)
- [OPSIN](http://opsin.ch.cam.ac.uk/instructions.html)
- [PAN Pesticide Database](https://www.pesticideinfo.org/)
- [PubChem](https://pubchem.ncbi.nlm.nih.gov/)
- [U.S. EPA Substance Registry Service
  (SRS)](https://cdxnodengn.epa.gov/cdx-srs-rest/)
- [Wikidata](https://www.wikidata.org/wiki/Wikidata:WikiProject_Chemistry)

#### API keys

Some ChemSpider functions require an API key. Please register at RSC
(<https://developer.rsc.org/>) to retrieve an API key.

## Installation

#### Install from CRAN (stable version)

``` r
install.packages("webchem")
```

#### Install from Github (development version)

``` r
install.packages("devtools")
library("devtools")
install_github("ropensci/webchem")
```

### Use Cases

Have you used `webchem` in your work? Please let us know by opening an
issue or making a pull request to edit this section!

- Allaway RJ, La Rosa S, Guinney J, Gosline SJC (2018) Probing the
  chemical–biological relationship space with the Drug Target Explorer.
  Journal of Cheminformatics 10:41.
  <https://doi.org/10.1186/s13321-018-0297-4>
- Bergmann AJ, Points GL, Scott RP, et al (2018) Development of
  quantitative screen for 1550 chemicals with GC-MS. Anal Bioanal Chem
  410:3101–3110. <https://doi.org/10.1007/s00216-018-0997-7>
- Brokl M, Morales V, Bishop L, et al (2019) Comparison of Mainstream
  Smoke Composition from CR20 Resin Filter and Empty-Cavity Filter
  Cigarettes by Headspace SPME Coupled with GC×GC TOFMS and Chemometric
  Analysis. Beiträge zur Tabakforschung International/Contributions to
  Tobacco Research 28:231–249. <https://doi.org/10.2478/cttr-2019-0004>
- Münch D, Galizia CG (2016) DoOR 2.0 - Comprehensive Mapping of
  Drosophila melanogaster Odorant Responses. Scientific Reports 6:21841.
  <https://doi.org/10.1038/srep21841>

### Citation

If you use `webchem` in a publication, please cite our paper:

- Szöcs E, Stirling T, Scott ER, et al (2020) webchem: An R Package to
  Retrieve Chemical Information from the Web. J Stat Soft 93:.
  <https://doi.org/10.18637/jss.v093.i13>

### Acknowledgements

Without the fantastic web services `webchem` wouldn’t be here.
Therefore, kudos to the web service providers and developers! Please
remember to acknowledge these data resources in your work using
`webchem`.

### Want to contribute?

Check out our [contribution guide
here](https://github.com/ropensci/webchem/blob/master/CONTRIBUTING.md).

### Meta

- Please [report any issues, bugs or feature
  requests](https://github.com/ropensci/webchem/issues).
- License: MIT
- Get citation information for `webchem` in R with `citation("webchem")`
- Please note that this package is released with a [Contributor Code of
  Conduct](https://ropensci.org/code-of-conduct/). By contributing to
  this project, you agree to abide by its terms.

[![ropensci](https://ropensci.org/public_images/github_footer.png)](https://ropensci.org)
