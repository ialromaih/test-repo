## To search for a package
  ```
  a <- available.packages()
  head(rownames(a),3)
  ```

## To install a package
*  `install.packages("devtools")`
*  `install.packages(c("slidify", "ggplot2", "devtools"))`
  
## To load a package
*  `library(ggplot2)` without quotes

## To use a package
  ```
  library(ggplot2)
  search()
  ```
  
## Find working directory
* `getwd()`
* `dir()` shows the contect of the current working directory

## Read Data
* `read.csv("mydata.csv")`

## Load Functions
* `ls()` lists functions
* `source("mycode.R")`

## Functions
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
* `x <- factor(c("yes","yes","no", "yes", "no"))` creates a factor with values "yes" and "no"
* `table(x)` shows the frequency of the two factors
* `unclass(x)` encodes class in numeric values (integer vector) (e.g. "yes" -> 2, "no" -> 1)
* `x <- factor(c("yes","yes","no", "yes", "no"),levels("yes","no")` creates a factor with values "yes" (level1) and "no" (level2)
* `is.na()` tests for NA and NaN objects
* `is.nan()` tests for NaN values (x/0)
* `x <- data.frame(foo = 1:4, bar = c(T,T,F,F))` creates a table with two columns foo and bar
* `nrow(x)` shows the number of rows, `ncol(x) shows the number of columns
* `names(x) <- c("foo", "bar", "norf")` labels columns in a vector
* `x <- list(a = 1, b = 2, c = 3)` creates a list with column names
* `dimnames(m) <- list(c("a","b"), c("c","d"))` creates a label for each column and row (row1 = a, row2 = b, column1 =c, column2 =d)

## Reading Data
* `read.table()` and `read.csv()` reads from tables
    
      ```
      inital <- read.table("datatable.txt", nrows = 100)
      classes <- sapply(initial, class)
      tabAll <- read.table("datatable.txt",
                            colClasses = classes)
      ```
* `readLines(con, 10)` reads from text files
* `source("data.R")` reads R code files (inverse is `dump()`)
* `dget("y.R")` reads R code files (inverse is `dput()`)
* `load()` reads saved workspaces
* `unserialize()` reads single R objects in binary format

## Writing Data
* `write.table()` and `read.csv()` writes to tables
* `writeLines()` writes to text files
* `dump(c("x","y"), file = "data.R")` writes to R code files (inverse is `dump()`)
* `dput(y, file = "y.R")` writes to  R code files (inverse is `dput()`)
* `save()` writes workspaces
* `serialize()` writes single R objects in binary format

## Connection Interfaces
* `file("foo.txt", "r")` opens a connection to a file (text file)
* `gzfile()` opens a connection to a file compressed with gzip
* `bzfile()` opens a connection to a file compressed with bzip2
* `url()` opens a connection to a webpage

## Validate Input
* `complete.cases(x,y)` returns a vector of T and F (F if either x or y is NA)

## Working with SWIRL
* `library(swirl)`
* `install_from_swirl("R Programming")`
* `swirl()`

