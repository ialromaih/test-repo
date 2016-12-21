###To search for a package
  ```
  a <- available.packages()
  head(rownames(a),3)
  ```

### To install a package
*  `install.packages("devtools")`
*  `install.packages(c("slidify", "ggplot2", "devtools"))`
  
### To load a package
*  `library(ggplot2)` without quotes

### To use a package
  ```
  library(ggplot2)
  search()
  ```
  
### Find working directory
* `getwd()`
* `dir()` shows the contect of the current working directory
