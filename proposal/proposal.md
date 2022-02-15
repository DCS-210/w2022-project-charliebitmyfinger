Project proposal
================
charliebitmyfinger

``` r
library(tidyverse)
library(broom)
```

## 1. Introduction

``` r
yt <- readr::read_csv(file = "../USvideos.csv")
```

    ## Rows: 40949 Columns: 16

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr  (7): video_id, trending_date, title, channel_title, tags, thumbnail_lin...
    ## dbl  (5): category_id, views, likes, dislikes, comment_count
    ## lgl  (3): comments_disabled, ratings_disabled, video_error_or_removed
    ## dttm (1): publish_time

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
head(yt)
```

    ## # A tibble: 6 × 16
    ##   video_id    trending_date title  channel_title category_id publish_time       
    ##   <chr>       <chr>         <chr>  <chr>               <dbl> <dttm>             
    ## 1 2kyS6SvSYSE 17.14.11      WE WA… CaseyNeistat           22 2017-11-13 17:13:01
    ## 2 1ZAPwfrtAFY 17.14.11      The T… LastWeekToni…          24 2017-11-13 07:30:00
    ## 3 5qpjK5DgCt4 17.14.11      Racis… Rudy Mancuso           23 2017-11-12 19:05:24
    ## 4 puqaWrEC7tY 17.14.11      Nicke… Good Mythica…          24 2017-11-13 11:00:04
    ## 5 d380meD0W0M 17.14.11      I Dar… nigahiga               24 2017-11-12 18:01:41
    ## 6 gHZ1Qz0KiKM 17.14.11      2 Wee… iJustine               28 2017-11-13 19:07:23
    ## # … with 10 more variables: tags <chr>, views <dbl>, likes <dbl>,
    ## #   dislikes <dbl>, comment_count <dbl>, thumbnail_link <chr>,
    ## #   comments_disabled <lgl>, ratings_disabled <lgl>,
    ## #   video_error_or_removed <lgl>, description <chr>

## 2. Data

## 3. Data analysis plan
