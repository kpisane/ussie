
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ussie

<!-- badges: start -->
<!-- badges: end -->

The goal of ussie is to let you work with European football data. (the
REAL goal is that I am learning about package development, this is a
test/toy package)

## Installation

You can install the development version of ussie from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("kpisane/ussie")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(ussie)
spain <- uss_make_matches(engsoccerdata::spain, "Spain")
head(spain)
#> # A tibble: 6 × 8
#>   country tier  season date       home               visitor     goals…¹ goals…²
#>   <chr>   <fct>  <int> <date>     <chr>              <chr>         <int>   <int>
#> 1 Spain   1       1928 1929-02-10 Arenas de Getxo    Atletico M…       2       3
#> 2 Spain   1       1928 1929-02-10 Espanyol Barcelona Real Union        3       2
#> 3 Spain   1       1928 1929-02-10 Real Madrid        CE Europa         5       0
#> 4 Spain   1       1928 1929-02-10 Real Sociedad      Athletic B…       1       1
#> 5 Spain   1       1928 1929-02-12 Racing Santander   FC Barcelo…       0       2
#> 6 Spain   1       1928 1929-02-17 FC Barcelona       Real Madrid       1       2
#> # … with abbreviated variable names ¹​goals_home, ²​goals_visitor
```
