HW 01 - Earthquakes
================
Vincent Baker
1/30/23

## Load packages and data

``` r
library(tidyverse)
library(openintro)
```

## Exercises

### Exercise 1

There are 123 earthquakes in the dataset.

### Exercise 2

There are 7 variables in the dataset.

### Exercise 3

``` r
earthquakes %>%
  count(region, sort = TRUE)
```

    ## # A tibble: 39 × 2
    ##    region            n
    ##    <chr>         <int>
    ##  1 Turkey           18
    ##  2 Iran             15
    ##  3 China            14
    ##  4 Japan             8
    ##  5 United States     8
    ##  6 Italy             5
    ##  7 India             4
    ##  8 Chile             3
    ##  9 Nicaragua         3
    ## 10 Pakistan          3
    ## # … with 29 more rows

Turkey, Iran, and China have experienced the most notable earthquakes in
the 20th century.

### Exercise 4

Remove this text, and add your answer for Exercise 4 here.

### Exercise 5

Remove this text, and add your answer for Exercise 5 here.

### Exercise 6

Remove this text, and add your answer for Exercise 6 here.

### Exercise 7

Remove this text, and add your answer for Exercise 7 here.
