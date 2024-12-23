
<!-- README.md is generated from README.Rmd. Please edit that file -->

# zooper

<!-- badges: start -->
<!-- badges: end -->

The goal of `zooper` is to provide functions used in zooplankton
community composition analysis, as well as a sample data-set to use with
the functions.

The package contains a function called `zoopl()`, which is used to
calculate the number of zooplankton per liter in a sample. In the folder
**data**, there is a practice data-set called **zoop_data.rda** that may
be used with the function. Documentation on the data-set can be found in
the folder **man** under **zooper-package.Rd**.

## Installation

You can install the development version of `zooper` like so:

``` r

devtools::install_github("claireestey", "zooper")
```

## Example

This is a basic example which shows you how to use the function `zoopl`
to calculate zooplankton per liter if your raw count of a species was
223 individuals, your sub-sample size was 10 mL, and the volume of water
filtered through the trap was 30 L:

``` r
library(zooper)
zoopl(count = 223, sample_vol = 20, subsample_vol = 12.5, trap_vol = 30)
#> [1] 11.89333
```
