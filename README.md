# week-2-c-scatter-plot
Names <- c("Shiva","Manya","Satwika","Nithya","Kiran")
Rollno <- c("Y20CS093","Y20CS123","Y20CS095","Y20CS127","Y20CS130")
Gender <- c("Female","Female","Female","Female","Female")
Marks <-c(2,4,6,8,10)
Fee <-c(69400,57892,58903,69400,67390)
Section <-c("C","C","C","B","B")

rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
rvrstudents
write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)

a <- read.csv("Rvr_Students.csv")
plot(rvrstudents$Fee,
     rvrstudents$Marks,
     main="RVRJCCE",
     xlab="students fee",
     ylab="students marks",
     col="blue",
     las=1)
cor(rvrstudents$Fee,rvrstudents$Marks)
