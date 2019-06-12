# How-to-merge-two-data-set-and-export-them-in-your-computer-
R_Data merge 

# Merge two data in R 
# First install this packages 
install.packages("plyr")
library("plyr")
# merge two datset 
mydata_final <- merge(Safety.Stock,INV.Growth , by= c("FCST_1_ID")
