
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rbccovideda

<!-- badges: start -->
<!-- badges: end -->

**Milestone1 Link**: <https://github.com/UBC-MDS/rbccovideda>

**Authors**: Lianna Hovhannisyan, John Lee, Vadim Taskaev, Vanessa Yuen

The British Columbia Center for Disease Control (BCCDC) manages a range
of provincial programs and clinics that contribute to public health and
help control the spread of disease in BC. It administers and distributes
the latest daily data on COVID-19 in British Columbia, which it provides
in csv format along case-, lab- and regional-specific features as well
as in comprehensive ArcGIS format via the [COVID-19
webpage](http://www.bccdc.ca/health-info/diseases-conditions/covid-19/data)
(under “Download the data”). This package leverages daily case-specific
COVID-19 data, allowing users to conveniently download the latest case
data, and - per specified date range interval - compute several key
statistics, visualize time series progression along age-related and
regional parameters, and generate exploratory data analysis in the form
of histogram figures supporting on-demand analysis. COVID-19 case detail
parameters extracted using this package:

-   Reported_Date (in YYYY-MM-DD format)
-   HA (provincial health region, e.g., “Vancouver Coast Health”)
-   Sex (M or F)
-   Age_Group (reported along 10-yr age group bins, e.g., “60-69”)
-   Classification_Reported (diagnosis origin, e.g., “Lab-diagnosed”)

## Installation

You can install the development version of `rbccovideda` from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("UBC-MDS/rbccovideda")
```

## Package Functions

-   `getData()`

    -   This function downloads the latest detailed daily case-specific
        COVID-19 from BCCDC’s dedicated [COVID-19
        homepage](http://www.bccdc.ca/health-info/diseases-conditions/covid-19/data).
        It returns a dataframe containing the extracted raw data.

-   `showSummaryStat()`

    -   This function computes summary statistics from the available
        case-specific parameters, such as age-related and regional
        aggregate metrics. It returns a dataframe listing key identified
        summary statistics specified per the time interval queried.

-   `plotLineByDate()`

    -   This function returns a line chart plot of daily case counts,
        based on parameters and grouping selected by the user, per the
        time interval queried.

-   `plotHistByCond()`

    -   This function returns a histogram plot based on parameters and
        grouping selected by the user, per the time interval queried,
        allowing for on-demand exploratory data analysis.

## Usage

(To do)

``` r
#library(rbccovideda)
## basic example code
```

## **Role within Python Ecosystem**

(To modify to match R ecosystem)

## Dependencies

## Contributing

Interested in contributing? Check out the contributing guidelines.
Please note that this project is released with a Code of Conduct. By
contributing to this project, you agree to abide by its terms.

## Contributors

Group 25 Contributors:

-   Lianna Hovhannisyan: @liannah
-   John Lee: @max780228
-   Vadim Taskaev: @vtaskaev1
-   Vanessa Yuen: @imtvwy

## License

The `rbccovideda` project was created by DSCI 524 (Collaborative
Software Development) Group 25 within the Master of Data Science program
at the University of British Columbia (2021-2022). It is licensed under
the terms of the MIT license.

## Credits

[R Packages](https://r-pkgs.org/), DSCI 524 Course Material (UBC MDS)
