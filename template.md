Simple document
================
Jianing Chen
2024-09-10

I’m an R Markdown document!

# Section 1

Here’s a **code chunk** that samples from a *normal distribution*:

``` r
#this is a comments
samp = rnorm(100)
length(samp)
```

    ## [1] 100

# Section 2

I can take the mean of the sample, too! The mean is -0.0714225.

# Section 3

## Data frame and plot

The code chunk below creats a data frame and generates a plot.

``` r
library(tidyverse)

plot_df = tibble(
  x=rnorm(500, mean=2, sd = 4),
  y=3-4.2*x + rnorm(500)
)
ggplot(plot_df, aes(x=x, y=y))+ geom_point()
```

![](template_files/figure-gfm/plot_example-1.png)<!-- -->

This plot is really great!! It shows a linear relation just as expected.

The data frame has 500 rows.

Here is a list:

- This is my first list item
- lists need at least two items
  - this list has a sub item
- Third list item

## Table

| Col 1 | Col 2 |
|-------|-------|
| a     | b     |
| c     | d     |

> This is a block quote.
