# Project-1
/Coursera


getwd()
setwd("C:/Users/Shalu/Desktop/coursera_R")
df <- read.table("HW1_data.csv", header = T, sep = ',')
mean_col <- cal_mean(df)
cal_mean <- function(y, remove_na = TRUE) {
  nc <- ncol(y)
    means <- numeric(nc)
  for (i in 1:nc) {
    means[i] <- mean(y[,i], na.rm = remove_na)
  
  }
  means
}
print( mean_col )

Temp_70 <- temp_70(df)
temp_70 <- function(y) {
  n_c <- ncol(y)
  ncount <- numeric(n_c)
  for (i in 1:n_c) {
    ncount[i] <- (y[,4] )
    if(ncount[i] == 70) { 
      
    }
  } 
    
} 
  
 
  

  
  
  

