Data Import
================
Jerri Chen
09/17/2019

## load in a dataset

``` r
## reads in a dataset
litters_data = read_csv(file = "./data/FAS_litters.csv")
```

    ## Parsed with column specification:
    ## cols(
    ##   Group = col_character(),
    ##   `Litter Number` = col_character(),
    ##   `GD0 weight` = col_double(),
    ##   `GD18 weight` = col_double(),
    ##   `GD of Birth` = col_double(),
    ##   `Pups born alive` = col_double(),
    ##   `Pups dead @ birth` = col_double(),
    ##   `Pups survive` = col_double()
    ## )

``` r
litters_data = janitor::clean_names(litters_data)
```

## read in an excel file

``` r
mlb11_data = read_excel(path  = "./data/mlb11.xlsx")
```

## read in SAS

``` r
pulse_data = haven::read_sas("./data/public_pulse_data.sas7bdat")
```
