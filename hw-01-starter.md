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

``` r
earthquakes %>%
  count(richter, sort = TRUE) %>%
  slice_max(n, n = 5)
```

    ## # A tibble: 6 × 2
    ##   richter     n
    ##     <dbl> <int>
    ## 1     7.3    13
    ## 2     6.8    11
    ## 3     7.5    10
    ## 4     7       9
    ## 5     6.9     7
    ## 6     7.1     7

``` r
arrange(earthquakes, richter, .by_group = TRUE)
```

    ## # A tibble: 123 × 7
    ##     year month      day richter area                region             deaths
    ##    <dbl> <chr>    <dbl>   <dbl> <chr>               <chr>               <dbl>
    ##  1  1986 October     10     5.5 <NA>                El Salvador          1000
    ##  2  1923 March       25     5.7 Torbat-e Heydariyeh Iran                 2200
    ##  3  1931 April       27     5.7 Border              Armenia-Azerbaijan   2800
    ##  4  1960 February    29     5.7 Agadir              Morocco             12000
    ##  5  1903 May         28     5.8 Gole                Turkey               1000
    ##  6  1951 August       2     5.8 Cosiguina           Nicaragua            1000
    ##  7  1946 May         31     5.9 Ustukran            Turkey               1300
    ##  8  1969 July        25     5.9 Guangdong           China                3000
    ##  9  1998 February     4     5.9 Hindu Kush          Afghanistan          2323
    ## 10  1931 March       31     6   Managua             Nicaragua            2500
    ## # … with 113 more rows

This dataset is now arranged by the Richter Scale (earthquake
intensity).

### Exercise 5

Remove this text, and add your answer for Exercise 5 here.

### Exercise 6

Remove this text, and add your answer for Exercise 6 here.

### Exercise 7

Remove this text, and add your answer for Exercise 7 here.
