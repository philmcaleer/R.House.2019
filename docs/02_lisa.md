# Lisa's Notes

## Making Blogs in Blogdown and GitHub

[Happy Git with R](https://happygitwithr.com) is an awesome resource for learning to use version control with your R projects.

### Initial Setup

1. Make [new repository on Github](https://github.com/new)

2. In RStudio, go to File > New Project... and select Version Control > Git

3. Make a file called `.Rprofile` in your user directory (`~`) and put the following line in it:

    ```
    options(blogdown.publishDir = "docs")
    ```
4. Run the following command in the Console window of RStudio.

    ```
    file.create('docs/.nojekyll')
    ```

If you have an existing project and want to add it to a new GitHub repository, follow the instructions at [Happy Git with R](https://happygitwithr.com/existing-github-first.html)

## Fork my Project

Go to [https://github.com/PsyTeachR/R.House.2019] and click on the Fork button in the upper right.


Render the book


```r
bookdown::render_book("index.Rmd", bookdown::gitbook())
```


