# doesShinytestWork

This app exists to check that shinytest2 works on your machine!

Clone the repository using RStudio

- Go to “File -> New Project”
- Click on “Version Control: Checkout a project from a version control repository”
- Click on “Git: Clone a project from a repository”
- Fill in the URL of the project https://github.com/jumpingrivers/doesShinytestWork.git

Once the project has opened in RStudio, you will need to install it's dependencies.

```r
# install.packages("renv")
renv::restore()
```

Then check that shinytest2 works by running:

```r
shinytest2::test_app()
```

A single test will run (it doesn't really matter whether the test passes or fails, but if you get
any errors there may be bigger problems afoot).
