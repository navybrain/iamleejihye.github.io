---
layout: post
title:  "두번째 테스트중"
subtitle: "R 분서 결과 포스팅 내맘대 테스트"
type: "Analysis"
blog: true
text: true
author: "Hojae Han"
post-header: true
order: 2
---

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

엠포스에서 빅데이터 분석을 해봤습니다<sub>~</sub><http://http://www.emforce.co.kr>

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

    ## 'data.frame':    50 obs. of  2 variables:
    ##  $ speed: num  4 4 7 7 8 9 10 10 10 11 ...
    ##  $ dist : num  2 10 4 22 16 10 18 26 34 17 ...

Including Plots
---------------

You can also embed plots, for example:

<img src="index_files/figure-markdown_github/pressure-1.png" style="display: block; margin: auto;" />

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

``` r
require(ggplot2)
```

    ## Loading required package: ggplot2

``` r
require(plotly)
```

    ## Loading required package: plotly

    ## 
    ## Attaching package: 'plotly'

    ## The following object is masked from 'package:ggplot2':
    ## 
    ##     last_plot

    ## The following object is masked from 'package:stats':
    ## 
    ##     filter

    ## The following object is masked from 'package:graphics':
    ## 
    ##     layout

``` r
hhj_theme <- theme_classic(base_family="NanumGothic") +
  theme(#axis.text.x = element_text(angle = 45),
    strip.background = element_rect(colour = "white", fill = "white"), 
    axis.line = element_line(colour = "#EBEBEB"), 
    panel.spacing = unit(1, "lines")
  )

theme_set(hhj_theme)
```

------------------------------------------------------------------------

> plot result

``` r
p <- ggplot(pressure, aes(temperature, pressure, color = "")) +
  geom_point()

p
```

<img src="index_files/figure-markdown_github/unnamed-chunk-3-1.png" style="display: block; margin: auto;" />

Conclusion
----------

엠포스의 빅데이터 분석을 통해 마케팅 분야의 ...
