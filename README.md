WEEK2-_QUIZ_IS607
=================
Question1


#1, creating numeric vector
 v<-rep(1:5,4)
 v
 [1] 1 2 3 4 5 1 2 3 4 5 1 2 3 4 5 1 2 3 4 5
 Question#2
 #2changing numeric vector into character
 c<-as.character(v)
 c
 [1] "1" "2" "3" "4" "5" "1" "2" "3" "4" "5" "1" "2"
 [13] "3" "4" "5" "1" "2" "3" "4" "5"
 Question #3 changing numeric vector into factor vector
 f<-factor(v)
 f
 [1] 1 2 3 4 5 1 2 3 4 5 1 2 3 4 5 1 2 3 4 5
 Levels: 1 2 3 4 5
 Question#4 number of levels that the vector has
 l<-nlevels(f)
 l
 [1] 5
 Question #5 Creating vector with a formula, sapply
 r<-sapply(v, function(x) 3*x^2-4*x +1)
 r
 [1] 0 5 16 33 56 0 5 16 33 56 0 5 16 33 56 0
 [17] 5 16 33 56
Question#6 least-squares regression
> x=matrix(
+ c(1,1,1,1,1,1,1,1,5,4,6,2,3,2,7,8,8,9,4,7,4,9,6,4),
+ nrow=8,
+ ncol=3) #create matrix 8 by 3
> x
     [,1] [,2] [,3]
[1,]    1    5    8
[2,]    1    4    9
[3,]    1    6    4
[4,]    1    2    7
[5,]    1    3    4
[6,]    1    2    9
[7,]    1    7    6
[8,]    1    8    4
> y=matrix(
+ c(45.2,46.9,31.0,35.3, 25.0,43.1, 41.0, 35.1),
+ nrow=8,
+ ncol=1)# create matrix 8 by 1
> y
     [,1]
[1,] 45.2
[2,] 46.9
[3,] 31.0
[4,] 35.3
[5,] 25.0
[6,] 43.1
[7,] 41.0
[8,] 35.1
> t(y) #transpose matrix of y
     [,1] [,2] [,3] [,4] [,5] [,6] [,7] [,8]
[1,] 45.2 46.9   31 35.3   25 43.1   41 35.1
> t(x)
     [,1] [,2] [,3] [,4] [,5] [,6] [,7] [,8]
[1,]    1    1    1    1    1    1    1    1
[2,]    5    4    6    2    3    2    7    8
[3,]    8    9    4    7    4    9    6    4

> B<-solve(t(b)%*% b)  %*%  t(b) %*% a # find B values
> B
         [,1]
[1,] 3.153126
[2,] 1.983743
[3,] 3.999539

Question #7 Creating a named list
 v=list(gender=c(1,2), status=c("single","married"))
 v
 $gender
 [1] 1 2

$status
 [1] "single" "married"


v[["gender"]]
 [1] 1 2
 v$gender
 [1] 1 2

Question#8 Creating a data frame
 m<-data.frame(matrix(0, ncol=4, nrow =10))
 m
 X1 X2 X3 X4
 1 0 0 0 0
 2 0 0 0 0
 3 0 0 0 0
 4 0 0 0 0
 5 0 0 0 0
 6 0 0 0 0
 7 0 0 0 0
 8 0 0 0 0
 9 0 0 0 0
 10 0 0 0 0
 Question #10, read a csv file
 temperature= read.csv("temperature.csv")

Question #11 read txt file from different directory
 setwd("") # set working directory
 setwd("C:/measurements.txt")
 measurements = read.table("c":/measurments.txt") # read text file 

Question#13
 factorial = function(n) { 
•f =1
•for (i in 1:n)
• f = f*i
•f
•} 
factorial(12) 
 [1] 479001600

Question#19
 seq(from = 20, t0 = 50, by =5)
 [1] 20 25 30 40 45 50
 
 Question#15 Using loop to find the sum of series
> x=rep(1,10)
> for (j in 1:10){
+ x[j]= 2^j
+ }
> x
 [1]    2    4    8   16   32   64  128  256  512 1024
> sum(x)
[1] 2046



Question#20
 rep("example", 10)
  Question#
