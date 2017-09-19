HW1 - Gapminder Exploration
================
Alexi Rodriguez-Arelis
18/9/2017

Dataset Exploration
===================

First of all, we need to load the dataset:

``` r
library(gapminder)
```

Now, we can examine the **first** 6 rows of the dataset:

``` r
head(gapminder)
```

    ##       country continent year lifeExp      pop gdpPercap
    ## 1 Afghanistan      Asia 1952  28.801  8425333  779.4453
    ## 2 Afghanistan      Asia 1957  30.332  9240934  820.8530
    ## 3 Afghanistan      Asia 1962  31.997 10267083  853.1007
    ## 4 Afghanistan      Asia 1967  34.020 11537966  836.1971
    ## 5 Afghanistan      Asia 1972  36.088 13079460  739.9811
    ## 6 Afghanistan      Asia 1977  38.438 14880372  786.1134

As well as the **last** 6 rows:

``` r
tail(gapminder)
```

    ##       country continent year lifeExp      pop gdpPercap
    ## 1699 Zimbabwe    Africa 1982  60.363  7636524  788.8550
    ## 1700 Zimbabwe    Africa 1987  62.351  9216418  706.1573
    ## 1701 Zimbabwe    Africa 1992  60.377 10704340  693.4208
    ## 1702 Zimbabwe    Africa 1997  46.809 11404948  792.4500
    ## 1703 Zimbabwe    Africa 2002  39.989 11926563  672.0386
    ## 1704 Zimbabwe    Africa 2007  43.487 12311143  469.7093

We can also get summaries for a specific variable as in:

``` r
# Disabling scientific notation
options(scipen = 999)
# Summary for Population
summary(gapminder$pop)
```

    ##       Min.    1st Qu.     Median       Mean    3rd Qu.       Max. 
    ##      60011    2793664    7023596   29601212   19585222 1318683096
