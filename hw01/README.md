# STAT545-hw01-Rodriguez-Arelis-Alexi
# Homework 01: Edit `README.md` and Use R Markdown

This is the folder corresponding to Homework 1.

I made all the changes using my repository local version on RStudio, i.e.: pull, edit locally, save, commit, push to github.com.

Now, I'm trying some features on the `README.md` file:

- *Italics*.
- **Bold**.
- ~~Strikeout.~~
  + Nested bullets.
    * Even more nested.

### Links

- [Main STAT545 webpage.](http://stat545.com)

- [Link to the `md` file for Gapminder exploration.](hw1_gapminder.md)

### My R Code
    
This a function I use for handling my simulation databases:
```R
get.N.RMSE <- function(results, Type ,Approach, Software)
{
  results <- cbind(results, c(rep(Type, nrow(results))),
                   c(rep(Approach, nrow(results))), 
                   c(rep(Software, nrow(results))))
  colnames(results)[6:ncol(results)] <- c("N_RMSE", "Type", "Approach", "Software")
  results <- results[, c(1:3, 6:ncol(results))]
  return(results)
}
```

### Image

![alt text](f_function_2d.png "2-d Franke's Function")


### Reflections on the GitHub Workflow and R Markdown

The workflow went smoothly throughout all the assignment. I didn't have any issues when pulling, committing and pushing while I was editting the files locally.

Furthermore, the `.md` file for the Gapminder exploration is a really useful tool for `R` outputs.
