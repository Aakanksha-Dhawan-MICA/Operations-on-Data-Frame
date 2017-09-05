N <- c("A", "B", "C", "D", "E")
A <- c(23,22,21,25,20)


student <- data.frame(Name= c(LETTERS [1:5]),
                      Age= c(23,22,21,25,20),
                      MM= c(87,86,89,88,79),
                      SM= c(65,87,78,55,93))

#add column
student$total <- student$MM+student$SM
student$percentage <- round(100*student$MM/student$total, digits=2)
#digits= numbers after point

#drop columns or put few coulumns in different sheet
student1 <- student
student2 <- student[,"Name"]
student2 <- student[,c("Name","Age")]
View(student2)

#to check column header names
namestudent <- names(student)
names(student) <- c(letters[1:6])
names(student) <- namestudent

vect1 <- seq(1,10, by=2)
#change value of a vector

vect1[3] <-100

v_col <- names(student)
v_col[3] <- "new_maths"
#change column names
student3 <- student
names(student) <- v_col
View(student3)
names(student3)[3] <-"new_maths"

names(student1)

student$exp_age= exp(student$Age)/mean(student$Age) #divided by mean becuase the number is very huge
student$log_age= log(student$Age)
student$inv_age= 1/(student$Age)
student$srt_age= student$Age*student$Age
View(student)

#changing type of a column
class(student$Name)
student$Name <- as.character(student$Name)
class(student$Name)

nn <- c("XX", "23", 24.5, "78.4")
n.num <- as.numeric(nn)

is.na(n.num) #to find missing values

#to find distinct values of a column 
table(is.na(n.num))

#filter
View(student)
s1<- student$Age>=23 #vector which contains value less than 23
student4 <- student[s1,]
# rows different, same columns
View(student4)
student5 <- student[student$Science>80 & student$new_maths>80,]
View(student5)

?sample
#Sampling
sample_index <- sample(1:nrow(student),3,replace=F) #Take 3 rows from student
sample_index
student6 <- student[sample_index,]
View(student6)

names(student)
student10 <- student[,c(1,3,4,5,6,2,7,8,9,10,11)]
dt.missing <- data.frame(age=c(12,34,56,67,NA,45,78,NA),
           Income=c(76889,65667,767821,76860,NA,765680,236598,NA))
dt.missing$age_missing <-is.na(dt.missing$income)


df$a #calling a vector
df$a = c(101:110)

#Problem1
install.packages("data.table")
installed.packages("dataset")
library("datasets")
women
mean.height <- mean(women$height) #created a vector and putting average in that
mean.weight <- mean(women$weight)
#fins women more than the average hieght and less than average weight
#subset is a function
women_df <- subset(women$height> mean.height & women$weight <mean.weight)
#or
result= women[women$height> mean(women$height) & women$weight <mean(women$weight)]
View (result)

install.packages("xml2")
library(xml2)
#problem2
#first create the html file out of the page
city_link = "http://www.worldatlas.com/articles/the-biggest-cities-in-india.html"
city_file = read_html(city_link)
city_table= html_nodes(city_file, "table")
#Invoke the first table
city_table_final <- html_table(city_table[1], fill= TRUE)
view(city_table_final)
city_data= as.data.frame(city_table_final)
View(city_data)
#write html_ to invoke and see what functions are there

#Hands on exercise 3

normal_income <- rnorm (10, mean=250000, sd= 75000)
View(normal_income)
mean(normal_income)

cust.id<- c(1:100)
income <- rnorm(cust.id, mean = 250000, sd= 75000)
View(income)
sd(income)
#repeat function is used to repeat the same values in a vector
gender <- c(rep("F, 100"))
m <- sample(1:100, 100, replace = FALSE) #It will create 100 integers but not unique if we don't write FALSE
#FOR LoOP- if you have to repeat a condition until the result is met
for(q in 1:100){ if(gender[m(q)]=="F" && q<=40)
  {else (gender [m(q)] <- c("M"))}}
