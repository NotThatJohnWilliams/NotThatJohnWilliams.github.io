
URL to Vignette: [Accessing API’s Using R: An Example Using REST
Countries API](https://not-that-john-williams.github.io/vignette-api/)  
URL to Github Repository:
[vignette-api](https://github.com/not-that-john-williams/vignette-api/tree/gh-pages)

This vignette is a simple demonstration on how to retrieve data from an
API using R. It includes 7 functions that query different endpoints of
the [REST Countries API](https://restcountries.com/v2/), allowing the
user to access data by the following:

-   Name or partial name
-   Continent
-   Region
-   Regional bloc
-   Currency
-   Language

All of these functions are bundled together into a single wrapper
function, `countriesAPI`.

After the review of API interaction functions, there are several brief
examples of data analysis using `countriesAPI`. In that exploration, I
discovered a few interesting tidbits:

-   English is the most common official language of countries in the
    world.
-   Twelve countries have English as an official language and the US
    Dollar as an official currency.
-   The majority of countries in the Americas (53%) have no land boarder
    with other countries. These are mostly island nations in the
    Caribbean.
-   Being a member of a regional bloc does not necessarily elevate
    income inequality within a country.
-   The European Union has the lowest mean income inequality of regional
    blocs.
-   The United States has higher income inequality than over half the
    countries in the world.

There were several difficulties encountered while completing this
vignette:

-   I initially wanted to use the [Mars InSight Mission
    API](https://mars.nasa.gov/insight/weather/) for this project. I
    thought creating functions that pull the current weather data on
    Mars would be unique and fascinating. Unfortunately, the data on
    that API is no longer being updated daily.
-   The data retrieved from the REST Countries API is not rectangular.
    It contains data frames nested within data frames and lists nested
    within lists. In the future, I’d like to create a helper function
    that would automatically tidy the data after each API interaction
    using `countriesAPI`.
-   Interacting with Git and Github through RStudio was my biggest
    learning curve. There were several stumbles and falls attempting to
    get the vignette webpage posted.

This project, overall, was beneficial for developing data science skills
even beyond its primary purpose of interacting with an API. I was able
to practice recognizing when to use the `apply` family of functions; I
learned about `grep`, a handy tool for searching for matches of certain
character patterns; and I delve deeply into the inner workings of the
tidyverse, specifically `ggplot`, during the exploratory data analysis.

Finally, here are a few “best practices” to remember when tackling
future data science projects:

-   Don’t jump in without a plan. Look at the whole picture, formulate
    the questions that need answered or express the final objective, and
    create an outline. Time spent on this at the very beginning is well
    worth it.
-   Break big, overwhelming tasks into smaller chunks. Create helper
    functions as needed. You’ll be surprised how many times you may
    reuse a helper function throughout the project which saves you time
    and brain power.
-   Use other’s hard work. There are many stellar resources online.
    Become skilled at seeking (and compiling!) proven packages and
    functions available to complete complex tasks.
-   Comments are your best friend. Don’t just answer why you did
    something but also explain how.

## Code Used to Generate This Blog Post

``` r
rmarkdown::render("_Rmd/2021-10-05-API-Vignette.Rmd", 
                  output_format = "github_document", 
                  output_dir = "_posts", 
                  output_file = "2021-10-05-API-Vignette.md")
```
