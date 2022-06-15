---
title: "Palmer Penguins Initial Analysis"
author: "Ricky Bobby"
format: html
editor: visual
execute:
  keep-md: true
---



## Palmer Penguins

Let's conduct an initial analysis of the Palmer Penguins dataset!


::: {.cell}

```{.r .cell-code}
library(tidyverse)
```

::: {.cell-output .cell-output-stderr}
```
── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──
```
:::

::: {.cell-output .cell-output-stderr}
```
✔ ggplot2 3.3.5     ✔ purrr   0.3.4
✔ tibble  3.1.6     ✔ dplyr   1.0.9
✔ tidyr   1.2.0     ✔ stringr 1.4.0
✔ readr   2.1.2     ✔ forcats 0.5.1
```
:::

::: {.cell-output .cell-output-stderr}
```
── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
✖ dplyr::filter() masks stats::filter()
✖ dplyr::lag()    masks stats::lag()
```
:::

```{.r .cell-code}
library(palmerpenguins)

penguins %>% head()
```

::: {.cell-output .cell-output-stdout}
```
# A tibble: 6 × 8
  species island bill_length_mm bill_depth_mm flipper_length_… body_mass_g sex  
  <fct>   <fct>           <dbl>         <dbl>            <int>       <int> <fct>
1 Adelie  Torge…           39.1          18.7              181        3750 male 
2 Adelie  Torge…           39.5          17.4              186        3800 fema…
3 Adelie  Torge…           40.3          18                195        3250 fema…
4 Adelie  Torge…           NA            NA                 NA          NA <NA> 
5 Adelie  Torge…           36.7          19.3              193        3450 fema…
6 Adelie  Torge…           39.3          20.6              190        3650 male 
# … with 1 more variable: year <int>
```
:::
:::


The `penguins` data set contains physiological measurements of different species of penguins observed on different islands and in different years. We can see the first six rows of the data set above.
