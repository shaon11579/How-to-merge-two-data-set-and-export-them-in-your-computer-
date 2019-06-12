# How-to-merge-two-data-set-and-export-them-in-your-computer-
R_Data merge 

# Merge two data in R 
# First install this packages 
install.packages("plyr")
library("plyr")
# merge two dataset 
mydata_final <- merge( mydata4, mydataIG, by= "FCST_1_ID")

# Now export this data in your working directory/ Desktop for future use 
write.table(mydata_final, file = "mydata_final.csv" , sep = ",")
# Spacify the path for where to save the file outside the working directory 
write.table(mydata_final, file = "INPUT Dir Here" , row.names= F sep = ",")

# Merge two data in R, X= your firstdata, Y= 2nd data

mydata_final5 <- merge( GDCGrowth, mydata4, by= c("FCST_1_ID"), all=TRUE)
