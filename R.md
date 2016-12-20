###To search for a package

      ```
      a <- available.packages()
      head(rownames(a),3)
      ```

### To install a package
   * `install.packages("slidify")`
   * `install.packages(c("slidify", "ggplot2", "devtools"))`
  
### To load a package
   * `library(ggplot2)` without quotes
 
### To use a package

      ```
      library(ggplot2)
      search()
      ```
