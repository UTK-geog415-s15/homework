The purposes of this assignment are get your first exposure to:

- the package management in R
- R's toolkit for reproducible research
    - R markdown
    - the packrat package
- plotting in R with ggpot.

## Why R is awesome

The strength of R there are thousands of packages that users have contributed to the R community. As I write this, there are [6184 packages on the largest repository](http://cran.r-project.org/web/packages/).   Chances are good that - whatever you want to do - someone else has already done it and contributed code for free.  A lot of that code is difficult to  use because 1) they aren't software engineers and 2) they are doing this for free in their own spare time, but hey, it's free, and you can't find it anywhere else.

So that's why R is awesome. It's certainly not because students find it easy to learn.

## Packages

The way all of this awesomeness is distributed is through packages.  Packages typically have a set of functions to do tasks with a particular unified theme.  The user loads up the dozen or so packages that are useful for the task at hand, and leaves the other ten thousand packages alone.

For example, the coolest package for general data visualization is called [ggplot2](http://ggplot2.org/).  In order to use this package, you first have to install the package.  You only have to install the first time.  Installing looks like this:
```R
install.packages(ggplot2)
```

In your code, you load a package into that session with the library command:
```R
library(ggplot2)
```

If you put this at the start of your code then you can use any function with that library.  What functions are there?  Here's the manual:
```R
help(package='ggplot2')
```
## R markdown

One of the coolest features of R in the last five years or so has been the ease of using markdown.  The Rmarkdown package allows you to write documents that intersperse your prose and your code.  When you run the document, the code is run, and the answers, tables, and plots are inserted into your document.  It's really slick.  It guarantees that the numbers in the text actually are what comes from the data.  No more copy and paste errors. Here is a really good blog post that [shows off some of what Rmarkdown can do](http://jeromyanglim.blogspot.com/2012/05/getting-started-with-r-markdown-knitr.html).  There is a lot more you can do... you can write presentations, papers, include references, etc.  My last few papers have been written using Rmarkdown.

We'll get our hands dirty with Rmarkdown in a bit.

## The packrat package

packrat is a new package I am just learning about.  One of the problems with R (or any software for that matter), is that sometimes software updates can break code that used to work.  This is a serious problem for collaboration (collaborators may not have most recent version) and archiving (archiving old code is much more useful if it actually works).  Packrat provides a way to keep tract of what packages and what package versions are used in a project.  When you share your work, packrat will set up the other computer to be just like yours.

Are you ready to put all this together?


# Assignment 0:
