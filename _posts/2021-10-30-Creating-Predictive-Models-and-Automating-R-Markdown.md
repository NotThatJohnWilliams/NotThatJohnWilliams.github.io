
Predictive modeling, a major component of data science, uses statistical
techniques to predict future outcomes. Its goal is to answer the
question: “Based on known past behavior, what is most likely to happen
in the future?” Some real-world applications of predictive modeling are
forecasting patterns in weather, predicting performance in sports,
anticipating buying behavior in retail, and detecting disease in
healthcare. While not foolproof, this method tends to have high accuracy
rates, which is why it is commonly used by data scientists.

In this project, we demonstrate a simple predictive analysis: collecting
data, conducting exploratory data analysis, training predictive models,
and validating the models performance on test data. We used the
`OnlineNewsPopularity` dataset from the [UC Irvine Machine Learning
Repository](https://archive.ics.uci.edu/ml/datasets/). Click the links
below to dive into the analysis:

[Project 2 for ST 558](https://srlmt.github.io/Project-2/)

[Github Repo for Project 2](https://github.com/Srlmt/Project-2)

## Post-Mortem Reflection

### What would you do differently?

I’ll answer the opposite of this question: What would I not do
differently? I’m glad my partner and I set up communication guidelines
and expectations at the very beginning of the project. We agreed that
frequent and clear communication in both e-mails, code comments, and
commit notes were vital to our success. This collaboration would have
been immensely more difficult if we did not communicate as well as we
did.

### What was the most difficult part for you?

Within this project, we automated R Markdown to generate 6 reports. Each
report was a predictive analysis on a subset of the
`OnlineNewsPopularity` dataset. This was my first time attempting
automation. It was where I spent the majority of my time working out the
bugs in the code.

### What are your big takeaways from this project?

Version control made collaboration with a partner easy. I had minimal
issues with merge conflicts and the small problems I did have were great
learning experiences. (Don’t forget to “pull” from the repo before
beginning your work for the day!)

Ensemble prediction methods can be very powerful. Random Forest and
Boosted Tree models quite often outperform Linear Regression models in
predictive accuracy.

## Code Used to Generate This Blog Post

``` r
rmarkdown::render("_Rmd/2021-10-30-Creating-Predictive-Models-and-Automating-R-Markdown.Rmd", 
                  output_format = "github_document", 
                  output_dir = "_posts", 
                  output_file = "2021-10-30-Creating-Predictive-Models-and-Automating-R-Markdown.md")
```
