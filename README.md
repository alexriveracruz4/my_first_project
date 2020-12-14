# This is the README file for my_first_project
The folders in this project are: 

* _data_ - is the folder where you will put all the data you have collected or been \
given to analyze. 
* _figures_ - is where you will put plots, data pictures, and other images you have \
created to show data to other people. 
* _code_ - is where you will create code files for collecting, cleaning up, or analy\
zing data. 
* _products_ - this is the place where you will place any reports, presentations, or\
 products you create for sharing with other people.
 
dim(airquality)
unique(airquality$Day) 
length(unique(airquality$Day)) 
median(airquality$Wind) 
 
iris
any(iris$Sepal.Length>5.5)
sum(iris$Species == "setosa" & iris$Petal.Width<=1.5)
mean(iris$Sepal.Length > 5 | iris$Petal.Length >5)
(iris$Sepal.Length == 5.0) | (iris$Sepal.Length == 5.1)
a <- (iris$Sepal.Length == 5.0) | (iris$Sepal.Length == 5.1)
a==!(iris$Sepal.Length == 5.0 | iris$Sepal.Length == 5.1)
a==(iris$Sepal.Length == 5.0 | !iris$Sepal.Length == 5.1)
a==(iris$Sepal.Length >= 5.0) & (iris$Sepal.Length <= 5.1)
a==!(iris$Sepal.Length %in% c(5,5.1))
identical((iris$Sepal.Length == 5.0) | (iris$Sepal.Length == 5.1),!(iris$Sepal.Length == 5.0 | iris$Sepal.Length == 5.1))
identical((iris$Sepal.Length == 5.0) | (iris$Sepal.Length == 5.1),(iris$Sepal.Length == 5.0 | !iris$Sepal.Length == 5.1))
identical((iris$Sepal.Length == 5.0) | (iris$Sepal.Length == 5.1),(iris$Sepal.Length >= 5.0) & (iris$Sepal.Length <= 5.1))

any(iris$Sepal.Width<1.3)
