------------------------------------------------------------------------

------------------------------------------------------------------------

My first adventure into programming languages was a project in BASIC in
5th grade. I made one pixelated number “bump” on screen into another
pixelated number to create its sum. At the time, I thought that was the
coolest thing I’d ever gotten to do in school. I didn’t jump back into
computer programming until college. I took courses in C and C++. Later,
in graduate school, I tackled SAS and R.

## R vs. Other Programming Languages

As someone who thrives on structure, I didn’t mind how syntactically
strict C, C++, and SAS are. I think that made them easier to master in a
short time. R, on the other hand, has lots of flexibility in syntax.
This means R code is easily readable, a huge win over other programming
languages. The only downside to this syntactic Wild West is R has a
steeper learning curve than other programming languages. R users have to
put in the time and effort to safely sail the seemingly endless ocean of
libraries to find–and then learn the unique syntax for–the right one. Do
you need previous experience with a programming language to learn R? No,
but I think it would be more difficult. By learning C and C++ first, I
was already comfortable with concepts like object-oriented programming,
functions, pointers, loops, and logic. I can imagine how difficult it
would be to learn these general programming concepts and navigate R
syntax at the same time.

Once you learn R, you can see how functional it truly is. While not a
broad, general programming language like C++, R excels at for what it
was designed: data science. It wasn’t designed by computer engineers; it
was designed by statisticians for statistical inference. So it’s harder
for those outside of data science to understand the value R has. They
complain that R is “slow” and “lacks scalability”. That may be true in
some sense, but as open-source software, R is free (unlike its
commercial competition SAS), evolving, and perfect for collaborating.
And for someone who’s worked with pointers in C++, R is a breath of
fresh air: no memory corruption issues. Also, you can create custom
operators in R; you can’t do that in C++.

## Example R Markdown Output

``` r
plot(trees)     # A plot of the dataset "trees"
```

![](../images/unnamed-chunk-1-1.png)<!-- -->

## Code Used to Generate This Blog Post

``` r
render("_Rmd/2021-9-13-Programming-Background.Rmd", output_format = "github_document", output_dir = "_posts", output_options = list(html_preview = FALSE))
```
