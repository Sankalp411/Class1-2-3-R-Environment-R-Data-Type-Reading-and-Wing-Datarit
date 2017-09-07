# Class1-2-3-R-Environment-R-Data-Type-Reading-and-Wing-Datarit
Exercises for getting acquainted to R environment &amp; Reading Data Types.
## Overview of the R Studio IDE
## Various sections and their utility

## How to run a command in R?
# Option 1 : Use the Run botton
# Option 2 : Go to the line -> Press Ctrl + Enter

## Where are the results seen in R?
# Ans : The R console
5+7
2+3



## What Version of R are we using?
R.Version()
sessionInfo()



############# Setting up the Working Directory  #################

## Get the Current Working Directory
getwd()

## Set the Working Directory



setwd("C:\\Ram\\General 20150804 v1\\Trainings\\R Programming for Data Science")
## Notice the direction of the slash (/)
setwd("C:/Ram/General 20150804 v1/R Training NAB/Day 1")

getwd()




#############   Interacting with R objects ######################

## Create an object

a <- 16

a <- 4; b <- 5

c <- 14+3


## NOTE 1 : An object is assigned a value using the <- operator
## NOTE 2 : Different commands can be marked by either a new line 
##        or a semicolon(;)

A

a+A

a <- 'MOdi'

## Use the objects
a<- 4
b <- 5
a + b
c <- a*b

23/7

d <- 23/7

d = 23/7


## REMEMBER : R is case - sensitive
A

## View objects present in the environmement
ls()

## Remove an object
rm(b)
remove(z)
b
z

?rm

help("rm")

aa <-  ls()

head(aa,10)

tail(aa,2)

?head

## Remove all objects from the environment
rm(list=ls()) # be careful


##################   R Libraries  ###############################

## Overview of R Packages -- how are they useful

mypackages <- head(installed.packages(),2)

head(mypackages)

head(installed.packages(),2)

## View what packages that are already installed
package_list <- data.frame(installed.packages())

## Install a package
install.packages("plyr","cars")

## After installation we need to load a package to use it in our work
## Loading the package
library(party)

## An alternative method
require(party)

## Help on library
library(help=party)

?ctree

help(ctree)


###################   Closing Comments ############################


## Get help on a function
?plyr
## OR
help(plyr)


## Clear the console
## Use ctrl + L

## Quit the R Session
quit()
## OR
q()

write.csv("ram.packages.csv",package_list)
