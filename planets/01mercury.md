Wolfman and Dracula measure really cool variable and unique space stuff.

    knitr::opts_chunk$set(fig.path = '../figures/')

    # ggplot2 examples

    library(ggplot2) 

    ## Warning: package 'ggplot2' was built under R version 3.3.2

    # create factors with value labels 
    mtcars$gear <- factor(mtcars$gear,levels=c(3,4,5),
        labels=c("3gears","4gears","5gears")) 
    mtcars$am <- factor(mtcars$am,levels=c(0,1),
        labels=c("Automatic","Manual")) 
    mtcars$cyl <- factor(mtcars$cyl,levels=c(4,6,8),
       labels=c("4cyl","6cyl","8cyl")) 

    # Kernel density plots for mpg
    # grouped by number of gears (indicated by color)
    qplot(mpg, data=mtcars, geom="density", fill=gear, alpha=I(.5), 
       main="Mercury is Awesome", xlab="Unique Space Stuff", 
       ylab="Really Cool Variables")

![](../figures/01mercury-1.png)
