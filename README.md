# week-2-c-scatter-plot
Names <- c("pragna","swathi","lohitha","Nithya","bhuvana")
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
OUTPUT:
> #scatter plot
> Names <- c("pragna","swathi","lohitha","Nithya","bhuvana")
> Rollno <- c("Y20CS093","Y20CS123","Y20CS095","Y20CS127","Y20CS130")
> Gender <- c("Female","Female","Female","Female","Female")
> Marks <-c(2,4,6,8,10)
> Fee <-c(69400,57892,58903,69400,67390)
> Section <-c("C","C","C","B","B")
> rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
> rvrstudents
    Names   Rollno Gender Marks   Fee Section
1   pragna Y20CS093  Female     2 69400       C
2   swathi Y20CS123 Female     4 57892       C
3  lohitha  Y20CS095 Female     6 58903       C
4  Nithya  Y20CS127 Female     8 69400       B
5   bhuvana Y20CS130   Female    10 67390       B
> write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)
> a <- read.csv("Rvr_Students.csv")
> plot(rvrstudents$Fee,
+      rvrstudents$Marks,
+      main="RVRJCCE",
+      xlab="students fee",
+      ylab="students marks",
+      col="blue",
+      las=1)
> cor(rvrstudents$Fee,rvrstudents$Marks)
[1] 0.8986413
