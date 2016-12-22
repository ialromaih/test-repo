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

### Read Data
* `read.csv("mydata.csv")`

### Load Functions
* `ls()` lists functions
* `source("mycode.R")`

### Functions
* `x` prints the value of x
* `print(x)` also prints the value of x
* `x <- 1` assigns the value 1 to variable x
* `x <- 1:20` assigns values 1,2,3,...,20 to a vector x
* `x <- c(0.5,0.6)` concatinates 0.5 and 0.6 into a vector x = [0.5 0.6]
* `x <- vector("numeric", length = 10)` initialize a vecotor of length 10 and default values (zeros)
* `class(x)` shows the data type of x
* `as.numeric(x)` , `as.logical(x)`, `as.character(x)` converts x to different data types.
* `x <- list(1, "a", TRUE, 1 + 4i)` creates a list of different types
* `cbind(x,y)` creates a matrix with x as column 1 and y as column 2
* `rbind(x,y)` creates a matrix with x as row 1 and y as row 2
